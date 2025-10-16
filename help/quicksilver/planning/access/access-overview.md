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

<!--leave the global record type reference in yellow till Jan 2026-->

<!--do not use the snippet for IMPORTANT , as it links to this article-->

<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

>[!IMPORTANT]
>
>The information in this article refers to Adobe Workfront Planning, an additional capability from Adobe Workfront. 
>
>Your company must purchase an additional package for Workfront Planning to access its capabilities. 
>
>For more information, contact your account manager
>
>For more information about Workfront Planning, see [Adobe Workfront Planning overview](/help/quicksilver/planning/general/planning-overview.md).

There are license and sharing permission restrictions to use Adobe Workfront Planning. 

This article describes the access and settings that you need in place to use the capabilities of Workfront Planning. 

## Access requirements 

<!--do not collapse the access requirements below - this is the main article about Access overview-->

<!--*********ensure that the link ^^^^^^^^below^^^^^^^^ to Workfront Pricing and Packaging now also includes information about Workfront Planning. If not, talk with Lauren S.***************-->

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
   <p>Any Workfront and Planning package</p>
   <p>Any Workflow and Planning package</p>

   <p><b>NOTE</b></p>

   <p>For access to connectable record types:</p>
   <ul><li><p>Any Workfront package and a Planning package</p></li>
   <li><p>Any Workflow and a Planning Prime and Ultimate package</p></li></ul>

   <div class="preview">
   <p>For access to global record types:</p>
   <ul><li><p>Any Workfront package and a Planning Plus package</p></li>
   <li><p>Any Workflow package and a Planning Prime and Ultimate package</p></li></ul> </td></tr>
   </div>
   <tr>
   <td role="rowheader"><p>Adobe Workfront platform</p></td>
   <td>
   <p>Your organization's instance of Workfront must be onboarded to the Adobe Unified Experience to be able to access Workfront Planning.</p>
   <p><b>IMPORTANT</b></p>
   <p>Only users added to the Adobe Identity Management System (IMS) can be granted permissions and added to Planning fields.</p>
   <p>For more information, see <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience for Workfront</a>. </p>
   </td>
  </tr>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront license</p></td>
   <td>
   <ul><li><p>Any, to view Workfront Planning information</p></li>
   <li><p>Standard, to create workspaces and views</p></li></ul>
    </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Access level configurations</p></td>
   <td> <p>There are no access level controls for Adobe Workfront Planning</p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Object permissions</p></td>
   <td>
   <ul>
   <li><p>View or higher permissions to workspaces, record types and views that you did not create to access them and their objects.</p></li>
   <li><p>Contribute or higher permissions to workspaces and record types that you did not create to edit them and create, edit, or delete record types and records.</p></li>
   <li><p>Contribute or higher permissions to views that you did not create, to edit, delete, and share them</p>
   </li>
    <li><p>System Administrators can manage workspaces they did not create. </p></li>
    <li><p>System Administrators cannot access views they did not create. </p></li></ul>
   <p>For information about sharing permissions for Workfront Planning objects, see  
   <a href="/help/quicksilver/planning/access/sharing-permissions-overview.md">Overview of sharing permissions in Adobe Workfront Planning</a> 
  </td>
  </tr>
<tr>
   <td role="rowheader"><p>Layout template</p></td>
   <td> 
<p>Standard users and System Administrators have the Planning areas enabled by default.</p>
<p> Users with a Light or Contributor license must be assigned a layout template that includes the Planning option  in the following areas:</p>
   <ul><li>Main Menu</li>
   <li>Left panel of projects, portfolios, and programs</li>
   </ul>   
</td>
  </tr>
 </tbody>
</table>

For more information, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).  


## Share the Planning area using a layout template

<!--First, contact your account manager to obtain access to the current Workfront Planning program.--> 

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

## Assign licenses to users

You can assign licenses to users when you configure their Access level while editing or creating them. 

For information, see [Edit a user's profiles](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md)

## Configure access level

There are no Workfront access level controls for Workfront Planning. 

Users with any type of Workfront license can access Workfront Planning. 

<!--For information about granting access in Workfront, see [Create and modify custom access levels](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md). -->

## Grant permissions

You can grant permissions to the following entities in Workfront Planning:

* Workspaces
* Record types
* Views

For more information, see [Overview of sharing permissions in Adobe Workfront Planning](/help/quicksilver/planning/access/sharing-permissions-overview.md).

Your Adobe Workfront license type works with your Workfront Planning permissions to give you access to view, contribute, or manage Workfront Planning objects.

For information about how license types affect permission levels for Workfront Planning objects, see [License type overview when using Adobe Workfront Planning](/help/quicksilver/planning/access/license-type-overview.md).


