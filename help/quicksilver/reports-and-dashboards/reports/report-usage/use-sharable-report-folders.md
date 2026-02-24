---
product-area: reporting
navigation-topic: report-usage
title: Use shareable report folders
description: Use shareable report folders to organize the reports that you create and share those folders with other users in Adobe Workfront.
author: Courtney
feature: Reports and Dashboards
hide: yes
hidefromtoc: yes
exl-id: 65831f2e-9092-4e99-a86b-40df42c713bf
---
# Use shareable report folders

<span class="preview">The information on this page refers to functionality not yet generally available. It is available only in the Preview Sandbox environment.</span>

<!-- This article is linked in the UI -->

You can use shareable report folders to organize reports and share those folders with other users. This feature is designed for teams that manage large volumes of reports and need scalable, consistent access control.

## Access requirements

+++ Expand to view access requirements for the functionality in this article. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront package</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license</td> 
   <td> 
   <p>any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>Edit access to Reports, Dashboards, Calendars</p> <p>Edit access to Filters, Views, Groupings</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to a report</p></td> 
  </tr> 
 </tbody> 
</table>

For more detail about the information in this table, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Understand folder permissions

Shareable report folders use two permission levels:

* **View**: Users can open reports in the folder, but they can't edit folder details, add or remove items, or delete the folder. You can allow users with View access to share the folder by enabling the **Share** setting when you grant access.
* **Manage**: Users can edit folder details and add or move report items. They are also granted Manage access to reports within the folder. You can allow users with Manage access to share the folder or delete folders by enabling the **Share** and **Delete** settings when you grant access.

Additional behavior:

* System administrators can see all folders.
* Other users see only folders they have access to.
* Permissions granted to a parent folder apply to all subfolders and reports within that folder tree.
* Users with access to a subfolder can see its parent folders for navigation, but not sibling folders unless access is granted.

## Create a shareable report folder

Only system administrators can create folders at the top level. After a shareable folder is created, users with Manage access can create subfolders within it.

{{step1-to-reports}}

1. Turn on the **Shareable report folders** toggle.
1. Click **Create folder**.
1. Enter a name for the folder.
1. Click **Create**.

![create a shareable folder](assets/add-sharable-folder.png)

## Create a subfolder in a shareable report folder

You can create up to 3 levels of subfolders within a shareable report folder. Subfolders inherit permissions from the parent folder, but you can also set unique permissions for each subfolder.

{{step1-to-reports}}

1. Find the folder you want to create a subfolder in.
1. Click **More** > **Add subfolder**.
1. Enter a name for the subfolder.
1. Click **Create**.

## Share a report folder with other users

When you share a folder with users, they inherit access to all subfolders in that folder tree. Users must also have access to each report, either through folder permissions or direct report sharing.

{{step1-to-reports}}

1. Find the folder you want to share.
1. Click **More** > **Share**.
1. Add users, teams, roles, groups or companies. 
1. Choose **View** or **Manage** access:
    * View access allows users to open reports in the folder. You can also allow users with View access to reshare the folder by selecting **Share** in the additional settings. 
    * Manage access allows users to edit folder details and add or remove items. You can also allow users with Manage access to delete folders or share the folder by selecting **Delete** and **Share** in the additional settings.
1. Click **Save**.

    ![share a folder and fine-tune access](assets/share-settings-sharable-folders.png)

## Move a report to a shareable folder

To move a report into a folder, you must have **Manage** rights to both the report and the shareable folder.

{{step1-to-reports}}

1. Select the checkbox next to the report you want to move.
1. Click **Move to folder** in the action bar at the bottom of the screen.
1. Find the folder you want to move the report to, then click **Move**. The report tree is collapsed by default, so you may need to expand the folders to find the destination folder.

    ![move a report to a shareable folder](assets/move-to-folder.png)

## Delete a shareable report folder

When you delete a folder, any subfolders within that folder are also deleted. You must have **Manage** access to the folder to delete it. Reports in the folder are not deleted and can still be found in the main report list. 

Report permissions granted through the folder permissions are removed when the folder is deleted. Report permissions granted directly from the report or inherited from a dashboard remain in place.  


{{step1-to-reports}}

1. Click **More** > **Delete**.
1. Click **Yes, delete it** to confirm.


## New list experience for shareable folders

When you access shareable folders in the Reports area, you will see a new list experience that allows you to easily view and manage your folders and reports. For more information about the new list experience, see [Use enhanced lists](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md).