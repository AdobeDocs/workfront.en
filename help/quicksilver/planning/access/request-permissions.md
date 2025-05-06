---
title: Request Permissions to a View or a Workspace
description: When someone shares a link to a view or workspace that you don't have access to, you can request permissions to be able to open it. This article explains the steps to request access to a view or workspace when you encounter a shared link that you cannot open.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 94dfa36a-801a-4eef-bcf5-4a3fecc5a3d0
---
# Request permissions to a view or a workspace

<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

>[!IMPORTANT]
>
>The functionality described in this article is available only when your organization has been onboarded to the Adobe Unified Experience. 
>
>For more information, see [Adobe Unified Experience for Workfront](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md). 


You can request permissions to a view or a workspace when someone shares a link with you to the view or the workspace to which you do not have access. 

Requesting permissions to a view is similar to requesting permissions to a workspace. 

This article describes how to request access to a view or a workspace when someone shares a link with you and you cannot access the shared page. 

For information about granting permissions to views and workspaces, see the following articles:

* [Share views](/help/quicksilver/planning/access/share-views.md)
* [Share workspaces](/help/quicksilver/planning/access/share-workspaces.md)


## Access requirements

+++ Expand to view access requirements. 

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
<p><b>IMPORTANT</b></p>
<p>The users in your organization can request permissions for views and workspaces only when your organization is onboarded to the Adobe Unified Experience. </p>
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
   <td>  <p>After your request for permission is granted, you could gain the following permissions:</p>
   <ul><li><p>View or Manage for a view</p></li>
   <li><p>View, Contribute, or Manage to a workspace</p></li></ul>  
   <p>Only users with Manage permissions to a workspace and a view can share a view publicly.</p></td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Layout template</p></td> 
   <td> 
   <p>In the Production environment, all users including the System administrators must be assigned to a layout template that includes the Planning areas.</p>
   <div class="preview">
<p> In the Preview environment, users with a Light or Contributor license must be assigned a layout template that includes the Planning option  in the following areas:</p>
   <ul><li>Main Menu</li>
   <li>Left panel of projects, portfolios, and programs</li>
   </ul>
   <p>For more information, see <a href="/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md">Create and manage layout templates</a>.</p>
   <p>Standard users and System Administrators have the Planning areas enabled by default.</p></div>
   </td> 
  </tr> 
</tbody> 
</table> 

 *For more information about Workfront access requirements, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

 +++


## Request permissions to a view or workspace

Requesting permissions to a view is similar to requesting permission to a workspace. 

When someone shares with you a link to a workspace or a view where you do not have access:

1. Click the link shared with you for the view or the workspace. 
    
    A **You have no access** page displays to inform you that you do not have access to the view or the workspace.

    ![Request access to view](assets/request-access-to-view.png)

1. (Conditional) If the link shared is for a view for a workspace where you have access, click **Open with existing view**. If you have permissions to access the workspace, the record type page opens in the default view.

1. (Optional and conditional) If you do not have permissions to view the workspace, add a personalized message in the box available, then click **Request access**. 

    All users with Manage permissions to the view or the workspace receive the following notifications for the access request:
      * An in-app notification
         ![In-app notification for access request](assets/in-app-notification-for-access-request.png)
      * An email notification
         ![Email notification for access request](assets/email-notification-for-access-request.png)
   
1. (Conditional) When the view or workspace manager grants you permissions to the view or workspace, you receive an email notification and an in-app notification with a confirmation that the permission was granted. <!--check this - I was not able to test this, but Isk confirmed.-->
