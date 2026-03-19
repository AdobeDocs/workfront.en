---
title: Adobe Workfront Planning Access Overview
description: Not all users in the organization have the same access and permissions to use Adobe Workfront Planning. This article describes the access and permissions that users could have to use the capabilities of Adobe Workfront Planning.
author: Alina
feature: Workfront Planning
recommendations: noDisplay, noCatalog
role: User, Admin
exl-id: 99fac041-a235-4991-b826-d19944164bc9
---

# Adobe Workfront Planning access overview

<!--updated for STA on 2026-->

<!--
do not use the snippet for IMPORTANT , as it links to this article
-->

<!--
<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>
-->   
<!--
<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>
-->

>[!IMPORTANT]
>
>The information in this article refers to Adobe Workfront Planning.
>
>Your company must purchase an Adobe Workfront Planning package to access its capabilities. 
>
>For information, see [Get started with Adobe Workfront Planning](/help/quicksilver/planning/general/planning-overview.md).
>For more information, contact your account manager.
>

There are license and sharing permission restrictions to use Adobe Workfront Planning. 

This article describes the access and settings that you need in place to use the capabilities of Workfront Planning. 

## Access requirements 

<!--
do not collapse the access requirements below - this is the main article about Access overview
-->

You must have the following access to use Workfront Planning: 

<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
    <tr>
 <tr>
   <td role="rowheader"><p>Adobe Workfront package</p></td>
   <td>
   <p>Any Adobe Workfront Planning package</p>

   <p><b>NOTE</b></p>

   <p>As disclosed in all Workfront Planning articles, some capabilities are available only in certain packages.</p>
   
   <!--
   <p>For access to connectable record types, you must have:</p>
   <ul><li><p>A Workfront Planning Prime and Ultimate package</p></li></ul>
   <p>For access to global record types, you must have one of the following:</p>
   <ul><li><p>Any Workfront Planning Plus package</p></li>
   <li><p>Any Adobe Workfront Planning Prime and Ultimate package</p></li></ul> </td></tr>
   -->
   
   <tr>
   <td role="rowheader"><p>Adobe Workfront platform</p></td>
   <td>
   <p>Your organization's instance of Workfront Planning must be onboarded to the Adobe Unified Experience to be able to access Workfront Planning.</p>
   <p><b>IMPORTANT</b></p>
   <p>Only users added to the Adobe Identity Management System (IMS) can be granted permissions and added to Planning objects.</p>
   <p>For more information, see <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience for Workfront</a>. </p>
   </td>
  </tr>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront Planning license</p></td>
   <td>
   <p>Contributor or higher</p>
    </td>
  </tr>
  <!--
  <tr>
   <td role="rowheader"><p>Access level configurations</p></td>
   <td> <p>There are no access level controls for Adobe Workfront Planning</p>  
   </td>
  </tr>
  -->
<tr>
   <td role="rowheader"><p>Object permissions</p></td>
   <td>
   You will need permissions to the following Workfront Planning objects to interact with them: 
   <ul>
   <li>Workspaces</li>
   <li>Record types</li>
   <li>Views</li> 
   </ul>
   <!--
   <ul>
   <li><p>View or higher permissions to workspaces, record types and views that you did not create to access them and their objects.</p></li>
   <li><p>Contribute or higher permissions to workspaces and record types that you did not create to edit them and create, edit, or delete record types and records.</p></li>
   <li><p>Contribute or higher permissions to views that you did not create, to edit, delete, and share them</p>
   </li>
    <li><p>System Administrators can manage workspaces they did not create. </p></li>
    <li><p>System Administrators cannot access views they did not create. </p></li></ul>
    -->
   <p>For information about sharing permissions for Workfront Planning objects, see  
   <a href="/help/quicksilver/planning/access/sharing-permissions-overview.md">Overview of sharing permissions in Adobe Workfront Planning</a> 
  </td>
  </tr>
<tr>
   <td role="rowheader"><p>Layout template</p></td>
   <td> 
<p>Planning System Administrators and Planning Standard-license users have the Planning areas enabled by default.</p>

<p><b>NOTE</b></p>
<p> If your organization has an Adobe Workfront or Workflow package, in addition to an Adobe Workfront Planning package, Planning users must also be assigned a layout template that includes the Planning areas.</p>
<p>For information, see <a href="/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md">Create and manage layout templates</a>. 
</td>
  </tr>
 </tbody>
</table>

<!--
I don't think this section is needed for Planning STA - this is not an area they can access: 

## Share the Planning area using a layout template

(***********First, contact your account manager to obtain access to the current Workfront Planning program.*******)

Standard users and System Administrators have the Planning areas enabled by default in the following areas:

* Main Menu
* Left panel of projects, portfolios, or programs

Your system administrator must add the Planning areas to you, if you have any other Workfront license and you need to contribute to Workfront Planning work. 

The administrator can add the Planning option to the following areas by modifying and assigning you to a layout template:

* Main menu
* Landing page
* Left panel for projects, portfolios, and programs
* Pins

To add or remove Workfront Planning areas from users of your Workfront instance: 

1. Log in to **Workfront** as a Workfront administrator.  

1. Go to **Main menu** > **Setup** > **Interface** > **Layout Templates** and open or create a layout template.
    
    For information about customizing a layout template, see [Create and manage layout templates](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).

1. Assign the layout template to the users that you want to have access to Workfront Planning. 

    For information, see [Assign users to a layout template](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/assign-users-to-layout-template.md).

    All users assigned to the template can now access Workfront Planning in their Main Menu. 
    
    Users can start creating workspaces, records types, records, and fields.
-->

## Assign licenses to users

<!--
According to Lilit, we might need sections here for how to assign access levels to users for Planning only vs Planning + WF users; revisit this at launch? 
-->

>[!NOTE]
>
>If your company purchased an Adobe Workfront package, in addition to an Adobe Workfront Planning package, you can assign the following licenses to users when you configure their Access level while editing or creating them:
>
>* Adobe Workfront licenses
>* Adobe Workfront Planning licenses
>
>For information, see [Edit a user's profile](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).
>

Workfront Planning uses the Adobe Workfront's Admin Console to manage user license. You must create users in the Adobe Admin Console before they can use all capabilities for Workfront Planning. 

You can create Planning System Administrators only in the Adobe Admin Console. 

You can assign a user a Planning Standard license in Workfront Planning. You must still add the user to the Admin Console so they can use all the capabilities of Workfront Planning. 

For information, see [Manage users in the Adobe Admin Console](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/admin-console.md). 

To view, assign a user's access level in Workfront Planning or deactivate a user: 

1. Log into Workfront Planning as a System Administrator.
1. Click **Main Menu** ![Main Menu icon](assets/lines-main-menu.png) in the upper-left corner of the screen.
1. Click **Users**.
   
   A list of Planning users opens. 
1. Click the checkbox to the left of a user's name to select them, then click the **Edit** icon ![Edit icon](assets/edit-icon-on-blue.png)  on the blue bar at the bottom of the screen.
1. Click **Access** in the left panel. 
1. (Conditional) If your company purchased an Adobe Workfront or Workflow license in addition to Workfront Planning license, choose between the following licenses for the **Planning access level** field: <!--is this the name of the field?-->

      * Standard. If your company purchased Workfront Planning without a Workfront or Workflow license, this is the only access level available. 
      * Contributor

1. (Optional) Deselect the **User is active** setting to deactivate the user. The user can no longer log into Workfront Planning. 

<!--Hiding for now, per Lilit, to simplify, since there is no access change: 

## Configure access level

There are no Workfront access level controls for Workfront Planning. 

Users with any type of Workfront license can access Workfront Planning. 

<!--
For information about granting access in Workfront, see [Create and modify custom access levels](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).
-->

## Grant permissions

<!--
>[!NOTE]
>
>If your company purchased an Adobe Workfront package, in addition to an Adobe Workfront Planning package, your Adobe Workfront license type works with your Workfront Planning permissions to give you access to view, contribute, or manage Workfront Planning objects.
>
>For information about how license types affect permission levels for Workfront Planning objects, see [License type overview when using Adobe Workfront Planning](/help/quicksilver/planning/access/license-type-overview.md).
-->

You can grant permissions to the following entities in Workfront Planning:

* Workspaces
* Record types
* Views

<!--
move this above Views: * <span class="preview">Records</span>
-->

For more information, see [Overview of sharing permissions in Adobe Workfront Planning](/help/quicksilver/planning/access/sharing-permissions-overview.md).

## Relationship between license types and permissions

Your Adobe Workfront license type works in conjunction with your Adobe Workfront Planning permissions to give you access to Planning objects. 

Depending on which package your organization has purchased, view the following articles to understand the relationship between license types and permissions in Workfront Planning:

* [License type overview when using Adobe Workfront Planning](/help/quicksilver/planning/access/license-type-overview.md)
* [License type overview when using Adobe Workfront Planning with Adobe Workfront](/help/quicksilver/planning/access/license-type-overview-for-workflow-with-planning-users.md)





