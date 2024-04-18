---
title: Deactivate or reactivate a user
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
description: As a Workfront administrator, you can deactivate or reactivate a user.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: aba243ba-46c2-4eb7-b704-4368bf0ae3cc
---
# Deactivate or reactivate a user

<!--Audited 2/2024-->

<!--

>[!IMPORTANT]
>
>The procedure described on this page applies only to organizations that have not yet been onboarded to the Admin Console. If your organization has been onboarded to the Adobe Admin Console, you must perform this action through the Adobe Admin Console.
>
>For instructions on deactivating a user in the Adobe Admin Console, see the section "Remove users" in the article [Manage users individually](https://helpx.adobe.com/enterprise/using/manage-users-individually.html) or contact your Adobe Admin Console Administrator.
>
>For a list of procedures that differ based on whether your organization has been onboarded to the Adobe Admin Console, see [Platform-based administration differences (Adobe Workfront/Adobe Business Platform)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

-->

If a user leaves the organization, you might need to remove them from Adobe Workfront. They should not remain active in the system, because this would create confusion for other users when adding them to updates or assigning them work. When you deactivate a user, other users no longer see their name when they search for people in the system.

Administrators can see inactive users in the Setup area.

You can reactivate a user at any time.

>[!IMPORTANT]
>
>We recommend that you deactivate users who have left the organization rather than deleting them. If a user is deleted, all history in Workfront associated with that user is lost. This includes their work assignments, their association with notes, hours, documents, and all other objects they have once created.
>
>Deactivating a user in Workfront removes the user's licenses to both Workfront and digital proofing. Additionally, the user can no longer be assigned work. When a user is deactivated, that user's Workfront license and proofing license become available to be used by another user. All other information in the deactivated user's profile remains unchanged.
>
>For more information about the impact of deleting and that of deactivating users, see [Delete users](../../../administration-and-setup/add-users/create-and-manage-users/delete-a-user.md).

## Access requirements

You must have the following to perform the steps in this article:

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
   <td>  <p>New: Standard </p> <p>Or </p><p>Current: Plan </p>   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>You must have one of the following:</p> 
    <ul> 
     <li> <p>The System Administrator access level. For information, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Grant a user full administrative access</a>. </p> </li> 
     <li> <p><b>Users</b> setting in your access level configured to <b>Edit</b> access, with <b>Create</b> and at least one of the two <b>User Admin</b> options enabled under <b>Fine-tune your settings</b> <img src="assets/gear-icon-in-access-levels.png">. </p> <p>Of these two options, if User <b>Admin (Group Users)</b> is enabled, you must be a group administrator of a group where the user is a member.</p> <p>For more information about the <b>Users</b> setting in an access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Grant access to users</a>.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

## Prerequisites

Before you deactivate a Workfront administrator or Standard or Plan license user, you must associate their objects and activities with another user. 

For more information, see [About deactivating Workfront administrators and Plan license users](#about-deactivating-workfront-administrators-and-plan-license-users) in this article.

## Deactivate a user

Be aware of the following when deactivating a user: 

* The user won't be able to access the system.
* The user will be removed from Frame.io review links, assets, projects, and accounts.
   * Reactivating the user does not automatically add them to the Frame.io items they were previously associated with. You must reassign the user manually to Workfront projects that require Frame.io collaboration.
   * If you reactivate this user, you must manually add them to previously assigned Frame.io items. For more information, see the section [Asset review and approval impact when you reactivate a user](#asset-review-and-approval-impact-when-you-reactivate-a-user).
* All data associated with the user will be retained.
* You can assign a deactivated user's license to another user.

To deactivate a user:

1. Click the **[!UICONTROL Main Menu]** icon ![Main Menu](/help/_includes/assets/main-menu-icon.png) in the upper-right corner of Adobe Workfront, or (if available), click the **[!UICONTROL Main Menu]** icon ![Main Menu](/help/_includes/assets/main-menu-icon-left-nav.png) in the upper-left corner, then click **Users** ![](assets/users-icon-in-main-menu.png). 

1. Select a user, click the **More** icon ![](assets/more-icon.png), then click **Deactivate**.

1. Click **Deactivate** in the box that appears.

## Schedule users for deactivation

As a manager, you may want to mark users for deactivation before they actually leave your organization. For example, if you are working with a user who is contractually bound, they are in your system for a limited period of time and you know their termination date. You can schedule them to become deactivated on that date.

Workfront administrators and Plan license users can see the deactivation date in their user profile.

To schedule a user for deactivation:

1. Click the **[!UICONTROL Main Menu]** icon ![Main Menu](/help/_includes/assets/main-menu-icon.png) in the upper-right corner of Adobe Workfront, or (if available), click the **[!UICONTROL Main Menu]** icon ![Main Menu](/help/_includes/assets/main-menu-icon-left-nav.png) in the upper-left corner, then click **Users** ![](assets/users-icon-in-main-menu.png). 

1. Select the user's name.

   Or

   (Optional) Select multiple users to schedule them for deactivation in bulk.

1. Click the Edit icon ![](assets/edit-icon.png).
1. In the Edit User box that displays, click **Resource Planning** to go to that area.
1. Enable the **Schedule Deactivation** option.  

1. In the calendar that displays, specify the date and the time for the **Scheduled Deactivation Date**.

   >[!NOTE]
   >
   >* In the time box, you can select only whole hour increments, not minutes.
   >* If you select a time for the current day which has passed, Workfront will schedule the deactivation for the following day at 12:00 AM. The time selected matches the computer timezone of the user who is scheduling the deactivation.

1. Click **Save Changes**.

   The user is deactivated on the selected day sometime after the selected time. If you selected multiple users to deactivate in bulk, all selected users are deactivated on the selected day sometime after the selected time.

We recommend that you build a report for users that you have scheduled for deactivation, to keep informed about what users are coming up to be deactivated. There is no confirmation that the deactivation happened after the users become deactivated.

## Reactivate a user

1. Click the **[!UICONTROL Main Menu]** icon ![Main Menu](/help/_includes/assets/main-menu-icon.png) in the upper-right corner of Adobe Workfront, or (if available), click the **[!UICONTROL Main Menu]** icon ![Main Menu](/help/_includes/assets/main-menu-icon-left-nav.png) in the upper-left corner, then click **Users** ![](assets/users-icon-in-main-menu.png). 

1. Select a user, click the More icon ![](assets/more-icon.png), then click **Activate**.

1. Assign a new **Access level**in the drop-down menu, then click **Reactivate**.

### Asset review and approval impact when you reactivate a user

Deactivated users lose access to their assigned Frame.io account as well as assigned projects, assets, and review links. If you choose to reactivate the user, you must manually reassign them. 

### Proofing impact when you reactivate a user

Deactivated users lose their assigned default proofing role and their proof license (if you are on a Workfront Premium Legacy Plan). If you choose to reactivate the user, you must:

* Reassign the license (if you are on a Workfront Premium Legacy Plan). For more information about Workfront proofing plans, see [Access to proofing functionality in Workfront](../../../administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md).
* Verify they have the correct proof role. Reactivated proof users are assigned whatever is specified as the default proof role for new users. See [Configure default proofing roles](../../../administration-and-setup/manage-workfront/configure-proofing/configure-default-proofing-roles.md) for more information.

## About deactivating Workfront administrators and Standard or Plan license users

Before you deactivate a Workfront administrator or a user with a Plan license, it's important to check for Workfront objects and activities involving that person, then associate them with another Workfront administrator or Plan license user as necessary.

These objects and activities might include the following:

* Tasks or issues assigned to the user
* Projects owned by the user
* Reports set up to run with the access rights of the user
* Templates owned by the user
* Projects and templates on which the user was set as a resource manager
* Request queue routing rules on which the Workfront administrator or Plan license user is the Default Assignee
* Approval processes that have a stage including the user (especially if they were the only approver on the stage)
* Timesheets that list the user as an approver
* Timesheet profiles that list the user as an approver
* Proofing Automated Workflows that include the user

## Resource planning impact when you schedule a user for deactivation

When you schedule a user for deactivation, they no longer appear in the Resource Planner as being available for budgeting hours. If they remain part of the Resource Pools, they appear in the Resource Planner, but their availability will be set to zero hours starting with the date of their scheduled deactivation.

The Resource Planner takes into account all the job roles of the users and Planned Completion Dates of the tasks and calculates resources accordingly.

For more information about the Resource Planner, see [Resource Planner overview](../../../resource-mgmt/resource-planning/get-started-resource-planner.md).
