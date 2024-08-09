---
title: Delete Users
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
description: When a user leaves your organization, can remove that user from Workfront, though we recommend deactivating users instead of deleting them.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: da57dea3-082b-4a86-ae13-5bf55401122e
---
# Delete users

When a user leaves your organization, you can remove that user from Adobe Workfront.

>[!IMPORTANT]
>
>Deleting a user from the system also deletes information associated with the user that you might want to retain. We recommend deactivating users instead of deleting them. For more information, see [Deactivate or reactivate a user](../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md).
<!--
>* The procedure described on this page applies only to organizations that have not yet been onboarded to the Admin Console. If your organization has been onboarded to the Adobe Admin Console, you must perform this action through the Adobe Admin Console.
>
>Deleting a user from the [!DNL Adobe Admin Console] deactivates the user in [!DNL Workfront], but does not delete them from [!DNL Workfront].
>
>  For instructions on deleting a user in the Adobe Admin Console, see the section "Permanently delete users" in the article [Manage users individually](https://helpx.adobe.com/enterprise/using/manage-users-individually.html) or contact your Adobe Admin Console Administrator.
>
>  For a list of procedures that differ based on whether your organization has been onboarded to the Adobe Admin Console, see [Platform-based administration differences (Adobe Workfront/Adobe Business Platform)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).
>
-->

## Access requirements

+++ Expand to view access requirements for the functionality in this article.

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
   <td>Plan</td> 
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

+++

## Deleting vs. deactivating a user

Deactivating a user causes the following things to happen:

* Removes the user's licenses to both Workfront and Workfront Proof if the Workfront Proof component is associated with your Workfront account. For more information about Workfront Proof, see [Workfront Proof: article index](../../../workfront-proof/workfront-proof.md).
* The user can no longer be assigned work.
* The user can no longer be added to updates.
* The user can no longer be added to teams or groups.
* Objects can no longer be shared with the user.
* Their association with the following objects remains intact:

   * Tasks, issues, projects, portfolios
   * Dashboards

     >[!NOTE]
     >
     >If you deactivate a user and can no longer view the reports or dashboards associated with a user, you may need to update the **Run this report with the Access Rights of:** field.  
     >To learn more, see the [Why can't I access a report owned by a deactivated user?](../../../reports-and-dashboards/reports/tips-tricks-and-troubleshooting/reports-faq.md#why) section of the [Reports FAQs](../../../reports-and-dashboards/reports/tips-tricks-and-troubleshooting/reports-faq.md) article.

   * Documents
   * Updates
   * Hours

* If the user has checked-out documents, the documents remain checked out when you deactivate them. Only a Workfront administrator can check them back in. For more information about checking out documents, see [Check out documents](../../../documents/managing-documents/check-out-documents.md).

Deleting a user causes the following things to happen:

* Removes the user's licenses to both Workfront and Workfront Proof, if the Workfront Proof component is associated with your Workfront account. For more information about Workfront Proof, see [Workfront Proof: article index](../../../workfront-proof/workfront-proof.md).
* The user can no longer be assigned work.
* The user can no longer be added to updates.
* The user can no longer be added to teams or groups.
* Objects can no longer be shared with the user.
* Deletes the association of that user with the following objects:

   * Tasks, issues, projects, portfolio
   * Dashboards

     >[!NOTE]
     >
     >You also lose access to custom sections that contained dashboards associated to the deleted user.  
     >To learn more, see the [How do I access a dashboard that contains a report owned by a deleted user?](../../../reports-and-dashboards/reports/tips-tricks-and-troubleshooting/reports-faq.md#how) section of the [Reports FAQs](../../../reports-and-dashboards/reports/tips-tricks-and-troubleshooting/reports-faq.md) article.

   * Updates
   * Hours

     >[!NOTE]
     >
     >These objects remain in Workfront but the owner of the object is now blank.

* If the user uploaded any documents under the Documents area in the Global Navigation Bar, the documents are also deleted.
* If the user has checked out documents that they own and the documents are uploaded in the main Documents area (accessed from the Main Menu), the documents are deleted with the user. For more information about checking out documents, see [Check out documents](../../../documents/managing-documents/check-out-documents.md).

For more information about deactivating users, see [Deactivate or reactivate a user](../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md).

You can permanently delete users one at a time, or you can permanently delete multiple users simultaneously. When you delete individual users, you must wait for the deletion process to complete prior to moving on to other activities in Workfront. The process of deleting multiple users simultaneously runs as a background process, so you can continue using Workfront as the users are deleted.

## Delete one or more users

{{step-1-to-users}}

1. Select at least one user that you want to delete, click the More menu ![](assets/more-icon.png), then click **Delete**.
1. In the box that appears, click **Delete** to confirm the deletion.

   The process of deleting users runs as a background process, so you can continue using Workfront as the user or users are deleted.

   Depending on the number of users you are deleting, the process can take several minutes or even a few hours.

   After receiving the confirmation in Workfront that the users were deleted, you might continue to see them in the system until the deletion process is complete in the background.

   At a later time, if you discover that one or more users were not successfully deleted, try to delete them one at a time.
