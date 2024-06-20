---
user-type: administrator
product-area: system-administration
navigation-topic: business rules
title: Create and edit business rules
description: You can select whether you want to receive new Workfront functionality on a monthly or quarterly basis.
author: Lisa
feature: System Setup and Administration
role: Admin
hidefromtoc: yes
hide: yes
recommendations: noDisplay, noCatalog
---
# Create and edit business rules

A business rule allows you to apply validation to Workfront objects and prevent users from creating, editing, or deleting an object when certain conditions are met. Business rules help to improve data quality and operational efficiency by preventing actions that could compromise data integrity.

A single business rule can be assigned to only one object. For example, if you create a business rule for not editing projects under certain conditions, you can't apply the same rule to tasks. You would have to create a separate business rule with the same conditions for tasks.

Access levels and object sharing have a higher priority than business rules when a user interacts with an object. For example, if a user has an access level or permission that does not allow editing a project, then those would take precedence over a business rule that permits editing a project under certain conditions.

A hierarchy also exists when more than one business rule is applied to an object. For example, you have two business rules. One restricts creating expenses in the month of February. The second prevents editing a project when the project status is Complete. If a user tries to add an expense to a completed project in June, the expense cannot be added because it has triggered the second rule.

Business rules apply to creating, editing, and deleting objects through the API as well as in the Workfront interface.

>[!NOTE]
>
>Because business rules block certain actions, you should always configure your business rules first in a sandbox or preview environment and test them thoroughly before enabling them in production.

## Access requirements

+++ Expand to view access requirements for the functionality in this article.

You must have the following to perform the steps in this article:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront plan</td> 
   <td>Ultimate</td> 
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

For more detail about the information in this table, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Scenarios for business rules

Some simple business rule scenarios are:

* Users cannot add new expenses during the last week of February. This formula could be stated as: `IF(AND(MONTH($$TODAY) = 2, DAYOFMONTH($$TODAY) >= 22), "You cannot add new expenses during the last week of February.")`
* Users cannot edit a project that is in Complete status. This formula could be stated as: `IF({status} = "CPL", "You cannot edit this project because it is in Complete status.")`

The syntax for building a business rule is the same as building a calculated field in a custom form. For more information about the syntax, see [Add calculated fields with the form designer](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/add-a-calculated-field.md).

For information about IF statements, see ["IF" statements overview](/help/quicksilver/reports-and-dashboards/reports/calc-cstm-data-reports/if-statements-overview.md) and [Condition operators in calculated custom fields](/help/quicksilver/reports-and-dashboards/reports/calc-cstm-data-reports/condition-operators-calculated-custom-expressions.md).

For information about user-based wildcards, see [Use user-based wildcards to generalize reports](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/use-user-based-wildcards-generalize-reports.md).

For information about date-based wildcards, see [Use date-based wildcards to generalize reports](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/use-date-based-wildcards-generalize-reports.md).

## Add a new business rule



## Activate a business rule

When a business rule is inactive, the Is Active field in the list of business rules displays False. You cannot update the status of the rule in the list view.

To activate a business rule:

1. Select the business rule in the list of rules and click the Edit icon.
1. Select **Yes** for **Is Active** in the business rule dialog.
1. Click **Save**.
