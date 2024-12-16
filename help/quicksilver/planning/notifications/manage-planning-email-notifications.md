---
title: Manage Adobe Workfront Planning Email Notifications
description: When someone tags you in a record comment in Adobe Workfront Planning, you receive an email notification for that tag.
author: Alina
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
exl-id: 3c505b3a-cda7-4e7b-b497-28b820e9bb8f
---

# Manage Adobe Workfront Planning email notifications

<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

{{planning-important-intro}}

You can receive email notifications from Workfront Planning when the following scenarios exist:

* Someone tags you in a record comment
   
   For information about tagging others in a record comment, see [Manage record comments](/help/quicksilver/planning/records/manage-record-comments.md). 
* Someone asks for your permission to access a view or a workspace
* Someone confirms your access has been granted for a view or a workspace <!--Isk confirmed that there is nno email for denying access but did not test-->

<div class="preview">

* You submit a Workfront Planning request. For information, see [Create and manage a request form in Adobe Workfront Planning](/help/quicksilver/planning/requests/create-request-form.md)
* Someone approves or rejects a Workfront Planning request that you submitted. For information, see [Approve a request in Adobe Workfront Planning](/help/quicksilver/planning/requests/approve-request.md)
* The status changes to a Workfront Planning request that you submitted.

</div>


## Access requirements

+++ Expand to view access requirements for Workfront Planning. 

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
<td> 
   <p> Products</p> </td> 
   <td> 
   <ul><li><p> Adobe Workfront</p></li> 
   <li><p> Adobe Workfront Planning<p></li></ul></td> 
  </tr>   
<tr> 
   <td role="rowheader"><p>Adobe Workfront plan*</p></td> 
   <td> 
<p>Any of the following Workfront plans:</p> 
<ul><li>Select</li> 
<li>Prime</li> 
<li>Ultimate</li></ul> 
<p>Workfront Planning is not available for legacy Workfront plans</p> 
   </td> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront Planning package*</p></td> 
   <td> 
<p>Any </p> 
<p>For more information about what is included in each Workfront Planning plan, contact your Workfront account manager. </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>Adobe Workfront platform</p></td> 
   <td> 
<p>Your organization's instance of Workfront must be onboarded to the Adobe Unified Experience.</p> 
<p>The users in your organization receive notifications from Workfront Planning only when your organization is onboarded to the Adobe Unified Experience. </p>
<p>For more information, see <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience for Workfront</a>. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront license*</p></td> 
   <td><p> Standard, Light, or Contributor</p>
   <p>Workfront Planning is not available for legacy Workfront licenses</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Access level configuration</p></td> 
   <td> <p>There are no access level controls for Adobe Workfront Planning</p>   
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Object permissions</p></td> 
   <td>   <p>View or higher permissions to a workspace</a> </p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p> </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Layout template</p></td> 
   <td> <p>All users, including Workfront administrators,  must be assigned a layout template that includes the Planning area in the Main Menu. </p> </td> 
  </tr> 
</tbody> 
</table> 

 *For more information about Workfront access requirements, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--
OLD: 

<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
    <tr>
<tr>
<td>
   <p> Product</p> </td>
   <td>
   <p> Adobe Workfront</p> 
   <p>In order to receive notifications from Workfront Planning and manage notification preferences, your organization's instance of Workfront must be onboarded to the Adobe Unified Experience. For information, see <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience for Workfront</a>.</p></td>
  </tr>  
 <td role="rowheader"><p>Adobe Workfront agreement</p></td>
   <td>
<p>Your organization must be enrolled in the early access stage for Workfront Planning </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront plan</p></td>
   <td>
<p>Any</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront license</p></td>
   <td>
   <p>Any</p> 
  </td>
  </tr>
  
  <tr>
   <td role="rowheader"><p>Access level configuration</p></td>
   <td> <p>There are no access level controls in Workfront Planning. </p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Permissions</p></td>
   <td> <p>View or higher permissions to a workspace</a> </p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p>
</td>
  </tr>

<tr>
   <td role="rowheader"><p>Layout template</p></td>
   <td> <p>Your Workfront or group administrator must add the Planning area in your layout template. For information, see <a href="/help/quicksilver/planning/access/access-overview.md">Access overview</a>. </p>  
</td>
  </tr>
 </tbody>
</table>
-->


## Manage email notifications when someone tags you in a comment

1. (Conditional and optional) After someone tags you in a comment on a record, go to the email notification that informs you of the tag and of the comment. The sender of the email is Adobe Experience Cloud. 

    ![](assets/email-notification-example.png)

1. (Optional) Click the message in the **Workfront** box inside the email. 

   The record details page opens in Workfront. You can make updates to the record, or reply to the comment. 

1. (Conditional) If available, click **View all notifications**. <!--check with Lilit - do non-IMS users have this button??-->
    The **Notifications** page opens in Adobe Experience Cloud. All notifications from all Adobe Experience Cloud applications display. 

## Manage email notifications when requesting and granting permissions

1. (Conditional and optional) After someone requests or grants you permissions to access a view or a workspace, go to the email that informs you of the permission request. The sender of the email is Adobe Experience Cloud. 

1. (Optional) Click the message in the **Workfront** box inside the email. 

   The record details page opens in Workfront. You can make updates to the record, or reply to the comment. 

1. (Conditional) If available, click **View all notifications**. 
    The **Notifications** page opens in Adobe Experience Cloud. All notifications from all Adobe Experience Cloud applications display. 


For information about requesting, granting, or denying permissions to a view or a workspace, see [Request permissions to a view or a workspace](/help/quicksilver/planning/access/request-permissions.md). 

For information about managing your Workfront Planning notifications, see [Manage Adobe Workfront Planning notification preferences](/help/quicksilver/planning/notifications/manage-notification-preferences.md).

## Manage email notifications about submitting, approving, or rejecting Workfront Planning requests

1. (Optional) Go to the email that Workfront sends you 
after you submit a request, or after a request you submitted has been approved or rejected. The sender of the email is Adobe Workfornt.

1. (Optional) Click **Open request**. This opens the request in Workfront Planning. 

1. Click the **Notifications** icon ![](assets/notifications-area-icon-unified-shell.png) in the upper-right corner of the screen to access the **Notifications** page.

   For information about managing your Workfront Planning notifications, see [Manage Adobe Workfront Planning notification preferences](/help/quicksilver/planning/notifications/manage-notification-preferences.md).
