---
title: Share Workspaces
description: You can share a workspace with others to ensure collaboration when working in Adobe Workfront Planning.
author: Alina
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
exl-id: 475a519d-d3bd-4461-8099-0e296d556d34
---
# Share workspaces

<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

{{planning-important-intro}}

You can share a workspace with others to ensure collaboration when working in Adobe Workfront Planning. 

<!--
This article describes how you can share a view with others. For information about requesting, granting, or denying permissions to a view, see [Request permissions to a view or a workspace](/help/quicksilver/planning/access/request-permissions.md). -->

>[!NOTE]
>
>Granting permissions to a workspace does not give other users permissions to the views on the record type pages. You must grant permissions to individual views in a record type page to share them with other users. For information, see [Share a view](/help/quicksilver/planning/access/share-views.md). 


## Access requirements

+++ Expand to view access requirements.. 

You must have the following access to perform the steps in this article:  

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
<p>Your organization's instance of Workfront must be onboarded to the Adobe Unified Experience to be able to access all the capabilities of Workfront Planning.</p>
<p>Your organization must be onboarded to the Adobe Unified Experience for users to be able to request and grant permissions to a workspace from a permission request. </p> 
<p>For more information, see <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience for Workfront</a>. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront license*</p></td> 
   <td><p> Standard </p>
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
   <td>  <p>Manage permissions to a workspace</p>  </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Layout template</p></td> 
   <td> <p>All users, including Workfront administrators,  must be assigned a layout template that includes the Planning area in the Main Menu. </p> </td> 
  </tr> 
</tbody> 
</table> 

 *For more information about Workfront access requirements, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

 <!--replace the layout template info in the table with this at release: 


<p>In the Production environment, all users including the System Administrators must be assigned to a layout template that includes the Planning areas.</p>
<p><span class="preview">In the Preview environment, Standard users and System Administrators have the Planning area enabled by default.</span></p>

-->

## Considerations about sharing workspaces

* For general information about sharing objects in Workfront Planning, also see [Overview of sharing permissions in Adobe Workfront Planning](/help/quicksilver/planning/access/sharing-permissions-overview.md). 
* You can share workspaces with users, teams, roles, groups, or companies inside your organization.
* In addition to teams, groups, companies, and job roles, you can share only with users that have been added to the Adobe Admin Console. 
* You cannot share workspaces with users outside of your organization. 
* When you share a workspace, all record types, records, and fields associated with the workspaces are also shared.
* When you share a workspace, views are not shared. You must share views separately.

<div class="preview">
 
* Workspace permissions display as Inherited permissions on record types. 

</div>

## Share permissions to a workspace

The following users can share a workspace with other users:

* System administrators can share all workspaces, including the ones that they did not create.
* All other users can share only workspaces for which they have Manage permissions to. 

To share a workspace with others: 

{{step1-to-planning}}

1. Open the workspace you want to share, then click **Share** in the upper-right corner of the screen. 

    ![Share button on workspace top right](assets/share-button-on-workspace-top-right.png)

1. In the **Grant access to this workspace** field, start typing the name of a user, group, team, company, or job role then click it when it displays in the list. 

   ![Sharing UI with groups](assets/sharing-ui-with-groups.png)

1. Select one of the following permission levels from the drop-down menu: 
    * View
    * Contribute
    * Manage

        For information about permission levels and what actions users can perform for each level, see [Overview of sharing permissions in Adobe Workfront Planning](/help/quicksilver/planning/access/sharing-permissions-overview.md).
1. Click **Copy link** to copy a link to the workspace to your clipboard. 
1. Share the copied link with others. Users who receive the link must be active users and log in to Workfront to be able to access the workspace. 
1. Click **Save**.

## Grant permissions to a workspace from a permission request

Users who access a link to a workspace to which they do not have permissions can request permissions to the workspace. All users with Manage permissions to the workspace receive the permission request and can grant or deny the permissions. 

1. (Conditional) If you are are the manager of a workspace, you might receive a request from another user to access the view in the following areas:
   
   * An in-app notification
      ![In-app notification for access request](assets/in-app-notification-for-access-request.png)
   * An email notification
      ![Email notification for access request](assets/email-notification-for-access-request.png)
1. (Conditional) From the notification area in Workfront, click the in-app notification
   Or
   From the email notification, click **View all notifications**, then click the notification in the list.

   The **Pending access requests** box displays. 

      ![Notifications list approval box](assets/notifications-list-approval-box.png)

1. (Optional) For the user whose permissions you want to approve, select one of the following options from the drop-down menu to the right of the user's name: 
   * **View**
   * **Contribute**
   * **Manage**
1. Select the user for whom you want to approve or deny the permission, then click **Approve all** or **Deny all**. 
1. Click the left-pointing arrow to the left of **Pending access requests**, then click **Save**.

   If you approved the request, the users are added to the sharing box of the workspace. The user requesting the permission receives an email confirmation that their request was approved. <!--will they also get an in-app notification??-->


## Remove permissions to a workspace


{{step1-to-planning}}

1. Open the workspace you want to remove permissions to, then click **Share** in the upper-right corner of the screen. 
1. Click the drop-down menu to the right of the name of an entity you're sharing the workspace with, then click **Remove**. 
1. Click **Save**.

   The users removed no longer have access to the workspace or its objects.
