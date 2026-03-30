---
user-type: administrator
product-area: system-administration
navigation-topic: business rules
title: Create and Edit Business Rules
description: A business rule allows you to apply validation to Workfront objects and prevent users from creating, editing, or deleting an object when certain conditions are met. Business rules help to improve data quality and operational efficiency by preventing actions that could compromise data integrity.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 780c996c-5cf1-42fe-898d-2cc208bbae7b
---
# Create and edit business rules

<!--

<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

-->

A business rule allows you to apply validation to Workfront objects and prevent users from creating, editing, or deleting an object when certain conditions are met. Business rule validation helps to improve data quality and operational efficiency by preventing actions that could compromise data integrity.

<!--

<div class="preview">

Organizations that have the Workflow Ultimate package can also configure business rules to automate actions for the created, edited, or modified object when certain conditions are met. Available actions include sharing the object or attaching a custom form to the object.  

</div>

-->

A single business rule can be assigned to only one object. For example, if you create a business rule for not editing projects under certain conditions, you can't apply the same rule to tasks. You would have to create a separate business rule with the same conditions for tasks.

Access levels and object sharing have a higher priority than business rules when a user interacts with an object. For example, if a user has an access level or permission that does not allow editing a project, then those would take precedence over a business rule that permits editing a project under certain conditions.

When more than one business rule applies to an object, then the rules are all followed but are not applied in a certain order. For example, you have two business rules. One restricts creating expenses in the month of February. The second prevents editing a project when the project status is Complete. If a user tries to add an expense to a completed project in June, the expense cannot be added because it has triggered the second rule.

Business rules apply to creating, editing, and deleting objects through the API as well as in the Workfront interface.

>[!NOTE]
>
>Because business rules block certain actions, you should always configure your business rules first in a sandbox or preview environment and test them thoroughly before enabling them in production.

## Access requirements

+++ Expand to view access requirements for the functionality in this article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr>
   <td>Adobe Workfront package
   </td>
   <td> <p>Business rule validation:<ul><li><p>Ultimate</p></li><li>
    <p>Workflow Ultimate</p></li></ul></p><p>Business rule automation:<ul><li>
    <p>Workflow Ultimate</p></li><ul></p>
   </td>
  </tr> 
  <tr> 
   <td>Adobe Workfront license</td> 
   <td>Standard</td> 
  </tr> 
  <tr> 
   <td>Access level configurations</td> 
   <td>System administrator</td> 
  </tr>  
 </tbody> 
</table>

For information, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Scenarios for business rules

* [Scenarios for business rule validation](#scenarios-for-business-rule-validation)
* [Scenarios for business rule automation](#scenarios-for-business-rule-automation)

### Scenarios for business rule validation

The format of a business rule validation is "IF the defined condition is met, then the user is prevented from the action on the object, and the message is displayed."

The syntax for the properties and other functions in a business rule is the same as the syntax for a calculated field in a custom form. For more information about the syntax, see [Add calculated fields with the form designer](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/add-a-calculated-field.md).

For information about IF statements, see ["IF" statements overview](/help/quicksilver/reports-and-dashboards/reports/calc-cstm-data-reports/if-statements-overview.md) and [Condition operators in calculated custom fields](/help/quicksilver/reports-and-dashboards/reports/calc-cstm-data-reports/condition-operators-calculated-custom-expressions.md).

For information about user-based wildcards, see [Use user-based wildcards to generalize reports](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/use-user-based-wildcards-generalize-reports.md).

For information about date-based wildcards, see [Use date-based wildcards to generalize reports](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/use-date-based-wildcards-generalize-reports.md).

An API wildcard is also available in business rules. Use `$$ISAPI` to trigger the rule only in the API. Use `!$$ISAPI` to enforce the rule only in the user interface and allow users to bypass the rule through the API.

* For example, this rule prohibits users from editing completed projects through the API. If the wildcard was not used, the rule would block the action in both the user interface and the API.

  ```
  IF({status} = "CPL" && $$ISAPI, "You cannot edit completed projects through the API.")
  ```

The `$$BEFORE_STATE` and `$$AFTER_STATE` wildcards are used in expressions to access the object's field values before and after any edits.

* These wildcards are both available for the edit trigger. The default state for the edit trigger (if no state is included in the expression) is the `$$AFTER_STATE`.
* The object creation trigger only allows the `$$AFTER_STATE`, because the before state does not exist.
* The object deletion trigger only allows the `$$BEFORE_STATE`, because the after state does not exist.

Some simple business rule scenarios are:

* Users cannot add new expenses during the last week of February. This formula could be stated as:

  ```
  IF(MONTH($$TODAY) = 2 && DAYOFMONTH($$TODAY) >= 22, "You cannot add new expenses during the last week of February.")
  ```

* Users cannot edit the project name of a project in Complete status. This formula could be stated as:

  ```
  IF({status} = "CPL" && {name} != $$BEFORE_STATE.{name}, "You cannot edit the project name.")
  ```

The system permits one business rule per object per trigger. For example, one edit trigger rule is allowed for issues. However, you can include multiple rules in a formula with nested IF statements.

A scenario with nested IF statements is:

Users cannot edit completed projects and cannot edit projects with a Planned Completion Date in March. This formula could be stated as:

```
IF(
    $$AFTER_STATE.{status}="CPL",
    "You cannot edit a completed project",
    IF(
        MONTH({plannedCompletionDate})=3,
        "You cannot edit a project with a planned completion date in March")
)
```

### Enable localization in a Business Rule

If your organization uses custom localization, you must enable translation of a business rule message in the business rule. If translation is not enabled, the message appears to the reader in English, even if the message text is in the Localization list and the user's browser is set to the appropriate language.

When configuring the rule, insert the word TRANSLATE before the message, and enclose the message in parentheses.

>[!BEGINSHADEBOX]

Example:

This example assumes that the message "You cannot edit completed projects" is included in the localization area of Setup, and that the user's browser is set to the localized language.

* `IF({status} = "CPL", "You cannot edit completed projects.") `
The message appears in English.
* `IF({status} = "CPL", TRANSLATE("You cannot edit completed projects."))`
The message appears in the localized language.

>[!ENDSHADEBOX]

For information on custom localization, see [Configure custom localization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/configure-custom-localization.md).

## Scenarios for business rule automation

>[!NOTE]
>
>Your organization must have a Workflow Ultimate package to use business rule automation.

The format of a business rule automation is "IF the defined condition is met, then the selected automation is triggered."

Business rule automation formulas do not require an error message

To ensure that an automation runs whenever the selected object and action occurs, such as when a project is created, use the following formula:

```
IF(true, true)
```

To share a project only if that's project has been approved, use a formula like the following:

```
IF({status} = "APR", true)
```

You can use wildcards in business rule actions, as described in the section [Scenarios for business rule validation](#scenarios-for-business-rule-validation).


## Add a new business rule

{{step-1-to-setup}}

1. Click **Business Rules** in the left panel.
1. Click **New business rule**.

1. Type the **Name** for the business rule on the rule builder dialog.
1. In the **Is Active** field, select whether the rule should be active when you save it.

   If you select **No**, the rule is saved as inactive, and you can activate it later.

1. (Optional) Enter a **Description** of the business rule and what happens when it is applied.


1. Select the object type to assign the business rule to..

   ![Select an object](assets/object-for-business-rule4.png) 

   You can apply business rules to the following objects:

   * Project
   * Task
   * Issue / Request
   * Portfolio
   * Document
   * Program
   * Expense
   * Company
   * Iteration
   * Billing Record
   * Group
   * Non-labor resource
   * Risk
   * Rate card
   * Assignment
   * User
   * Role
   * Hour
   * Template
   * Time Off
   * Resource Pool
   * Job role
   * Non-labor resource category
   * Resource Pool
   * Time Off
   * Hour
   * Staffing Plan
   * Template
   * Staffing Plan Resource
<!--
   * <span class="preview">Team</span>
-->

1. Type the **Name** for the business rule on the rule builder dialog.
1. In the **Is Active** field, select whether the rule should be active when you save it.

   If you select **No**, the rule is saved as inactive, and you can activate it later.

1. Select a **Trigger** for the business rule. The options are:

   * **Created** The rule is applied when a user attempts to create an object.
   * **Edited** The rule is applied when a user attempts to edit an object.
   * **Deleted** The rule is applied when a user attempts to delete an object.

1. Build the formula in the formula editor, in the center of the business rule dialog.

   The format of a business rule is "IF the defined condition is met, then the user is prevented from the action on the object, and the message is displayed."

   In the formula area, the parts of the business rule you build are the condition, and the message that displays in Workfront when the condition is met.

   * The "object" is the object type you selected when creating the business rule. It is displayed in the heading of the dialog.
   * The "action" is the trigger you selected for the rule: create, edit, or delete the object.
   * Because the object and the action are already defined, you do not include them in the formula.
   * The custom error message <span class="preview">is included only if the rule is for validation, and </span> is displayed to the user when they trigger the business rule. It should provide clear instructions on what went wrong and how to correct the issue.

     You can include a static URL in the error message, to link to documentation or other helpful pages to guide the user on how to modify their action within the constraint of the rule.

     In this example, "Learn more" will link to the URL. `"You are not allowed to add a new project in November.[Learn more](http://url)"` The URL must be in parentheses, but link text in brackets is not required. You can display the full URL and it will be a clickable link.

   ![Add business rule dialog](assets/add-business-rule-new.png) 

   This example is a business rule for projects. If the current month is November, then users are not permitted to create new projects, and the message explains this.
   
   For more examples of business rules, see [Scenarios for business rules](#scenarios-for-business-rules) in this article.

1. (Optional) Use the formula **Expressions** and **Fields** in the right panel to assist with building the rule.
    
    Search for an expression or field to narrow the list of available items.

    The list of available fields is limited to fields related to the object type for the business rule.

1. (Conditional) If you are validating the action, if your organization is on the Workfront Ultimate package, in the Then area, select **Validate the object**.

   For other packages, this option is pre-selected.

1. (Conditional) To automate another action,, select the action. 

   For details on these actions, see the section [Business rule automation options](#business-rule-automation-options) in this article.

   >[!NOTE]
   >
   >Your organization must be on the Workflow Ultimate package to use actions besides validation. If you do not see these other options, your organization is not on the Workflow Ultimate package.

1. Click **Save** when you are finished building the business rule.

>[!NOTE]
>
>After you add a business rule, you should test it by adding, editing, or deleting the associated object to make sure the rule is applied properly.

<div class="preview">

### Business rule automation options

   >[!NOTE]
   >
   >Your organization must be on the Workflow Ultimate package to use actions besides validation. If you do not see these other options, your organization is not on the Workflow Ultimate package.

You can set these actions to automate when the business rule is triggered. Available actions depend on the selected object type.

|Automation|Further configuration|
|---|---|
|Attach a custom form|Select the custom form that you want to add|
|Share the object|Select the people, roles, groups, companies, or access levels that you want to share the object with.|

## Activate a business rule

When a business rule is inactive, the Is Active field in the list of business rules displays False. You cannot update the status of the rule in the list view.

To activate a business rule:

1. Select the business rule in the list of rules and click the Edit icon.
1. Select **Yes** for **Is Active** in the business rule dialog.
1. Click **Save**.

