---
title: Configure Record Type Business Rules
description: You can configure record type business rules that can enforce certain actions on records according to field values. 
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
---

# Configure record type business rules

{{planning-important-intro}}

<span class="preview">The information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the release to Preview, the same features are also available monthly in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

You can configure business rules for Adobe Workfront Planning record types to indicate that certain fields are required before an action on a record of that type is allowed or prevented. 

Depending on how the rule is formulated, you can allow for the following actions on the records if the defined business rules are met: 

* Edit or not edit a record
* Delete or do not delete a record

## Access requirements

+++ Expand to view access requirements to perform the steps in this article:  

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
</tr>   
<tr> 
   <td role="rowheader"><p>Adobe Workfront package</p></td> 
   <td> 
<ul> 
<li><p>Any Workfront or Workflow with a Planning package</p></li>
Or
<li><p>Any Planning package when purchased as a standalone product</p></li></ul>
   </td> </tr>
  <tr> 
   <td role="rowheader"><p>Adobe Workfront license</p></td> 
   <td><p>Workflow Standard</p>
   </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Adobe Planning license</p></td> 
   <td><p>Planning Standard</p>
   </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Access level configuration</p></td> 
   <td> <p>You must add both a Workflow and a Planning license type to the access level when you have both a Workflow and a Planning package</p>   
</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Object permissions</p></td> 
   <td>   <p>Manage permissions to a workspace and to a record type</p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p>  </td> 
  </tr>  
</tbody> 
</table> 

 For more information about Workfront access requirements, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Considerations when configuring business rules

* Business rules attach a condition to a field change or a record deletion. The rule only comes into play at one specific, deliberate moment: when a field is about to change to a field value you configure in the rule. 

* A rule looks like this in plain language: "Before you can edit this record, the Campaign summary field must have a value".

   If the field is empty, the record edit is blocked and the user receives a clear message explaining what they need to to address before moving forward. Once they update the required field and try again, the change is allowed. 

* Rules don't block record creation. Users can still create  records but they must ensure that the required fields are not empty or contain the specified value. 
* Rules don't automatically edit or delete records. The change must be deliberate and triggered by a user. 
* Rules are not apply retroactively: old records are not affected. The rule check only runs the next time someone tries to edit or delete a record. 
* You cannot add business rules to global record types in their primary or secondary workspaces. 
* You can create a condition for your business rule that references all field types except for the following:  
    * Formula fields 
    * Lookup fields 
    * Reference fields  
* Rules apply to everyone who can edit or delete records. 
* You can have more that one business rule for a record type.  <!--Syuzanna is checking this because it should be just ONE rule per action: one per edit and one per delete - see this: https://workfront.slack.com/archives/C0BHWEUSJCU/p1788281638322049?thread_ts=1787924876.280359&cid=C0BHWEUSJCU; I also logged a bug for this because it released with more than one per action - https://experience.adobe.com/#/@adobeinternalworkfront/so:hub-Hub/workfront/issue/6a99add600001e9aa90435ec181dec3e/overview-->

   All the rules are checked together at the same time. <!-- I have asked Syuzanna and Norayr multiple times HOW are the rules run/ prioritized and I got no answers; when I know, I will update here-->

## Configure business rules

1. Go to a record type page. 
1. From any view, click the **More** menu ![More menu](assets/more-menu.png) to the right of the record type name, then click **Business rules**.

   The Business rules table page opens.
1. Click **New business rule**.
1. In the **New business** rule box, add a name for the business rule in the first available field. This is a required field
1. (Optional) Add a description to define the business rule, then click **Save**.

   The Business rule setup form opens. 

   ![Business rule setup form](assets/business-rule-setup-form.png)

1. In the **If** section of the business rule setup form, choose which actions you would like to restrict or allow based on a specific rule. Choose from the following: <!--check UI text-->
   * **Record edit**: Users will be allowed to edit or not edit the record, if the condition defined in this rule is met. 
   * **Record delete**: Users will be allowed to delete or not delete the record, if the condition defined in this rule is met.
      <!--add screen shot when UI text is final-->
1. In the **Formula field**, add the business rule. Choose an operator for your rule from the **Formula expressions** section in the right panel.
   
   For example, you can choose **IF** from the **Other** fields section, or start typing "IF", then click it when it displays in the suggestion list. 
   
      >[!TIP]
      >
      >Selecting the fields and operators from the suggestion list is recommended, to keep the syntax of the rule correct. 
1. Choose and the field that you want to make mandatory to allow for the records of this record type to be either edited or deleted. 

   For example, you can type the following statement to make the **Campaign summary** field required: 

   ```
      IF(ISBLANK({Campaign summary}),"Campaign summary is a required field. You cannot edit this record without a value for the Campaign summary field.")

   ```
   
      >[!IMPORTANT]
      >
      >We strongly recommend that you include in the rule formula the following information to make it easy for users to understand when an action they are trying to perform on a record is not allowed: 
      >
      >* The exact fields that the rule is set up for. 
      >* The exact consequence if the rule is not met. 

   There are indicators in the **Formula** field when a field or an expression is wrong.  <!--add screen shot?-->

   In the **Then** section of the business rule, you can view an explanation of what the rule does. 

1. Click **Activate** to make the rule active for this record type, then click **Save**.

   Rules are applied immediately after you activate them and all users who have permissions to edit or delete records in the selected record type must follow them. 
1. (Optional and recommended) Click the back arrow to the left of the **Business rules** in the page header to display the record type page and go to a table view or open a record's page, then try editing or deleting a record, to test the rule you just created. 

## Manage business rules

You can edit, delete or deactivate existing business rules. 

Editing an existing rule does not change existing records. The edited rule only applies to existing records when someone attempts to edit or delete them. 

1. Go back to the **Business rules** table page for the record type.
1. Find the rule you want to change.
1. Hover over the rule name, then click the **More** menu ![More menu](assets/more-menu.png), then one of the following options:

   * **Edit**: This opens the business rule setup page and you can edit information about the business rule. 
   * **Deactivate**: <!--check this in the UI: right now, it says Disable--> This stop the rule from triggering but preserves for the future, it needed. 
   * **Delete**: All the information about the rule is deleted. Deleted rules cannot be recovered. 

   The edited rules or the deactivation of rules apply only for future records and they are not applied retroactively. 

   <!--add NEW screen shot below if UI is fixed with Deactivate at release; it was fixed in devTest-->

   <!--![Business rule more menu expanded](assets/business-rule-more-menu-in-table-expanded.png)-->

<!--

***********FROM CLAUDE - BELOW - MUST EDIT*******************


### What business rules actually do

Business rules attach a condition to a **status change**. Instead of enforcing complete data the moment someone creates a record (which would slow everyone down), the rule only kicks in at one specific, deliberate moment: when a status is about to change to a status you've configured.

A rule looks like this in plain language:

> "Before a record can move to **Ready for Execution**, the field **Brand** must have a value."

If the field is empty, the status change is blocked and the person gets a clear message telling them what to fix. Once they fill it in and try again, the change goes through.

A few important things this is *not*:

* **It doesn't block record creation.** People can still create a new record instantly and fill it in over time, exactly like today. 
* **It doesn't auto-fill anything or auto-change statuses.** A person always has to make the status change themselves.
* **It doesn't retroactively flag old records.** Records that are already sitting in the target status aren't affected — the check only runs the next time someone tries to move a record *into* that status.

### Step 1: Open the business rules configuration area

Business rules live alongside your other admin setup — you won't need to hunt for a separate "Planning" panel. From your workflow setup area:

1. Go to the main **workflow setup / admin configuration** area for your workspace.
2. Look for the **business rules** section for the record type you want to configure (for example, "Materials" or "Campaigns").


### Step 2: Choose the record type

Rules are configured per record type, so pick the one you want to add a rule to. For example, if you want to make sure every Materials record has key fields filled in before execution, select **Materials**.

### Step 3: Create a new rule

For each rule, you'll specify three things:

| What you set | Example |
|---|---|
| **Record type** | Materials |
| **Target status** | Ready for Execution |
| **Required field** | Brand |

In other words: "When a Materials record's status is changed to **Ready for Execution**, the field **Brand** must have a value."

You can add more than one rule for the same status. For example, you might require Brand, Therapeutic Area, Indication, and Estimated Launch Date all to be filled in before a record can move to "Ready for Execution" — each is its own rule, and all of them are checked together.

**What fields can you require?**

* Connected record fields (e.g., a linked Brand or Indication record) — the rule passes as soon as at least one record is linked.
* Standard text fields (single-line or paragraph) — the rule passes once there's any value.
* Date fields — the rule passes once a date is set.

**What you can't use yet:** formula fields and lookup fields aren't supported as rule targets in this release, since they're calculated in the background rather than filled in directly by a person.

### Step 4: Write the message people will see

When you create a rule, you'll also provide the message that shows up if someone tries to make the change without the field filled in. Keep it specific and actionable — something like:

> "Brand is required."

You don't need to worry about formatting a whole error banner — the system handles combining messages if multiple rules are violated at once (see below).

### Step 5: Save the rule

Once saved, the rule takes effect **immediately** for everyone in the workspace — no need to log out, refresh, or wait for a deployment. The very next time anyone tries to move a record into that status, the rule is checked.

### What your team will actually experience

Here's what changes for the people using Planning day to day, once a rule is live.

#### If a required field is empty

1. A planner opens a record and changes the status to the gated status (say, "Ready for Execution").
2. The system checks all rules tied to that status.
3. If a required field is empty, the change is **rejected** — the status reverts back to what it was.
4. A toast message appears, naming exactly which field(s) are missing:
   > *"Status change blocked: 'Brand' and 'Estimated Launch Date' must be populated before moving to 'Ready for Execution.'"*
5. The planner fills in the missing field(s) and tries the status change again.
6. This time, the rule passes, and the status updates normally.

#### If everything is already filled in

Nothing changes. The status updates instantly, with no extra steps or popups. Business rules are invisible until they're actually needed.

#### If several fields are missing at once

All the violated rules are checked together, and the message lists every missing field in one go — planners don't have to fix one field, try again, get told about the next one, and repeat.

### Step 6: Edit or remove a rule later

Rules aren't set in stone. To make changes:

1. Go back to the business rules configuration area for the record type.
2. Find the rule you want to change.
3. Edit the required field, target status, or message — or delete the rule entirely.
4. Save. The change applies immediately to future status changes.

Keep in mind: editing or deleting a rule **only affects transitions going forward.** Records that already made it into the target status before the change aren't reevaluated.
3## A few things worth knowing

* **This is separate from locking records after a status change.** Business rules (as described here) only check field completeness *before* a status change goes through. A different, related feature governs whether a record becomes fully locked from edits/deletion once it reaches a certain status — that's not what's covered here.
* **Bulk status changes** (changing status on many records at once) aren't fully defined yet for how they interact with business rules — if your team relies heavily on bulk actions, check with your Adobe contact on current behavior.
* **If a rule can't be evaluated** due to a system error, the transition is blocked rather than silently allowed through — you'll never end up with an incomplete record slipping past a rule because of a backend hiccup.
* **Turning the feature off** doesn't delete your configured rules — they're just paused. Turning it back on restores them exactly as they were, no reconfiguration needed.

### Quick reference: setting up your first rule

1. Confirm the feature is enabled for your tenant.
2. Go to workflow setup → business rules for your record type.
3. Choose the record type (e.g., Materials).
4. Create a rule: target status + required field.
5. Write a clear, specific error message.
6. Save — it's live immediately.
7. Repeat for each field you want to require.
8. Test it yourself: try changing a record's status with the field empty, confirm you see the expected message, fill in the field, and confirm the status change now goes through.

That's it — from here on, anyone converting a record forward will get a clear nudge if something's missing, instead of a downstream project quietly showing up incomplete.

-->