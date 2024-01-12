---
title: Create or edit a status
user-type: administrator
product-area: system-administration
navigation-topic: create-custom-status-and-priority-labels
description: As an Adobe Workfront administrator, you can create custom statuses for projects, tasks, and issues.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 35c804b5-569d-4ba8-84b8-6129f0ffbc7f
---
# Create or edit a status

<!-- Audited: 1/2024 -->

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT THROUGH CONTEXT SENSITIVE HELP LINKS.-->

As an Adobe Workfront administrator, you can create custom statuses for projects, tasks, and issues. These can be for users throughout the entire Workfront system, or for specific groups or subgroups. For more information about statuses, see [Statuses overview](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/statuses-overview.md).

>[!NOTE]
>
>Group administrators can also create their own group statuses, for use only by their groups. For more information, see [Create or edit a group status](../../../administration-and-setup/manage-groups/manage-group-statuses/create-or-edit-a-group-status.md).

## Access requirements

You must have the following access to perform the steps in this article: 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan</td> 
   <td>Any</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license</td> 
   <td>
     <p>New: Standard</p>
     <p>or</p>
     <p>Current: Plan</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>You must be a Workfront administrator.</p>  </td> 
  </tr> 
 </tbody> 
</table>

For more detail about the information in this table, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Create or edit a custom status

You can add a custom status for use by your entire organization or by a single group.

When you create a custom status for the entire organization, you can configure it so that all groups in the system can use it without editing it. Or you can configure it so that group administrators can modify it for their groups, as explained in [Create or edit a group status](../../../administration-and-setup/manage-groups/manage-group-statuses/create-or-edit-a-group-status.md).

1. Click the **Main Menu** icon ![](assets/main-menu-icon.png) in the upper-right corner of Adobe Workfront, then click **Setup** ![](assets/gear-icon-settings.png).

1. In the left panel, click **Project Preferences** > **Statuses**.

1. (Conditional) If you are creating or editing a status for use system wide, ensure that **System Statuses** is selected in the box in the upper-right corner.

   ![](assets/system-statuses-in-upper-rt-corner.jpg)

   Or

   If the status is for a group or subgroup, start typing the name of the group in the upper-right corner, then select it when it appears.

   ![](assets/system-statuses-in-upper-rt-corner-group.jpg)

1. Select the tab of the object type (**Project**, **Tasks**, or **Issues**) that you want to associate with the status.

1. If you are creating a new status, click **Add a New Status**.

   Or

   If you are editing an existing status, hover over it, then click the **Edit** icon that displays to the far-right.

   ![](assets/custom-status-edit.png)

1. Configure the status using the following options:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Status Name</td> 
      <td> <p>Type a name for the status. This is a required field.</p> <p>When you create a status name, be aware that others in the system can create a status with the same name. We recommend using a unique name to avoid confusion when selecting statuses in Workfront.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Description</td> 
      <td>(Optional) Type a description of the status. This communicates its purpose to those who use it.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Color</td> 
      <td> <p>Customize the color of the status by clicking the color field and selecting a color from the swatch panel. You can also enter a hex number in the field.</p> <p>The status color displays in the upper-right corner of Workfront when a user views the object.</p> <img src="assets/status-color.png" style="width: 350;height: 211;"> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Equates With</td> 
      <td> <p>Select one of the options from the list that best describes the function of the status. For example, if the status name is Done, the option it equates with should be Complete.</p> <p>Every status must equate with one of these options because this determines how the status functions.</p> <p>This option cannot be modified after the status is created.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Key</td> 
      <td> <p>If you are creating a new status, type a code or abbreviation for the status or use the one generated for you. This key must be unique in Workfront because it can be used for reporting purposes. If you attempt to specify a key that is already in use in the system, the field turns red.</p> <p>It might be useful to use an abbreviation that is recognizable to those who will use it.</p> <p>This option cannot be modified after the status is created.</p> <p>You cannot change the key code for Planning, Current, and Complete statuses. This is important if you are building a report in text mode.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Hide Status</td> 
      <td> <p>(Project and Task statuses only)</p> <p>Enable this option if you want the status hidden from users. When it is disabled (the default setting), all users in the system can use the status.</p> <p>You can hide an Issue status by disabling all 4 issue types (Bug Report, Change Order, Issue, Request).</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Lock for all groups</td> 
      <td>
       <p>When a status is locked, users throughout the system can see and use it and group administrators cannot customize it for their groups.</p> 
       <p>When a status is unlocked, group administrators can customize it for their individual groups.</p>

      <div>
       <p>You can use both locked and unlocked statuses in a system approval process. If you create a system approval process with an unlocked system status, users throughout the system can attach the approval process to any project, task, or issue in the system.</p>
       <p> In the following scenarios, warning messages display to help you and your users understand outcomes of unlocking a status:</p>
       <ul>
       <li>An administrator unlocks a system-level status that is used in an approval process. A message warns that  might delete the unlocked status for their groups, which would prevent group members from using that approval process properly for objects assigned to their group.</li>
       <li>A user starts to edit an approval process that uses an unlocked status. A message alerts the user about the unlocked status so they can evaluate whether it would be a good idea to re-lock or replace it.</li>
       <li>A system-level approval process with an unlocked status is attached on an object, and the status was deleted for the group assigned to the object. When a group member goes to the Approvals section for the object, a message explains that the approval process can't be initiated for the object.</li>
       </ul>
       <p>For more information about locking statuses, see <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/lock-or-unlock-a-custom-system-level-status.md" class="MCXref xref">Locked and unlocked system-level statuses</a>.</p>
       </div>
      </td>
     </tr> 
    </tbody> 
   </table>

1. Click **Save**.

   For instructions on making this status a default status, see [Use custom statuses as default statuses](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/use-custom-statuses-as-default-statuses.md).

For information about reordering group statuses, see [Reorder system-level and group statuses](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/reorder-system-statuses.md).
