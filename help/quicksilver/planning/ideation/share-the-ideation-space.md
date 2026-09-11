---
title: Share an Ideation Space with Others
description: Adobe Workfront Planning now offers an additional capability to ideate before you launch your campaigns. Leverage the power of AI to create and collaborate on ideas with others before they become planning records. 
author: Alina
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
---

# Share an Ideation space with others

<!--add to TOC and miniTOC-->

<span class="preview">The information on this page refers to functionality not yet generally available. It is available only as part of the **Ideation space Beta** program. </span>   

<span class="preview">For more information, see [Get started with the Ideation space for Adobe Workfront Planning](/help/quicksilver/planning/ideation/get-started-with-planning-ideation.md).</span>

{{planning-important-intro}}

<!--ome of this information is also duplicated in the section for Ideation space permissions in the Access needed to use Ideation space article-->

Workfront Planning record permissions are transferred to the ideation space of a record. 

In addition, you can give other users permissions to use the ideation space and add ideas to it. 

Consider the following: 

* Creators of ideations always have Editor permissions on their own ideations. 

* You must have Editor permissions on an ideation space to create briefs and export them to other applications. 

## Access requirements

+++ Expand to view the access requirements for the functionality in this article. 

<!--
are there additional license restrictions or packages to be purchased to have access to Ideation space?? If yes, update the table below
-->

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
   </td> 

<tr> 
   <td role="rowheader"><p>Additional products</p></td> 
   <td><ul>
   <li><p>Adobe GenStudio for Performance Marketing</p></li>
   <!--
   <li><p>Adobe Customer Journey Analytics</p></li>
   -->
   </ul>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workflow license</p></td> 
   <td><p>Standard</p>
   </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Adobe Planning license</p></td> 
   <td><p>Standard</p>
   </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Access level configuration</p></td> 
   <td> 
   <ul>
   <li><p>You must add both a Workflow and a Planning license type to the access level when you have both a Workflow and a Planning package</p>   </li>
   <li><p>The Disable Ideation space setting in your access level must be deselected</p></li>
</td> 
  </tr>  
   <tr> 
   <td role="rowheader"><p>Object permissions</p></td> 
   <td> <p>Contribute or higher permissions to the workspace and record type where you want to add records </p>
      <p>System Administrators have permissions to all workspaces, including the ones they did not create</p>
      <p>View permissions to Workfront objects to add them to briefs <!--not sure if this is available--></p>
      <p>Editor permissions on the Ideation space to create briefs</p>
   </td> 
  </tr>  
   <tr> 
   <td role="rowheader"><p>Adobe GenStudio for Performance Marketing user roles</p></td> 
   <td><p><ul><li>Any GenStudio user role to access Campaigns, Products, and Personas</li>
   <li>GenStudio System Manager to access Activations <!--and Events--></li></ul>
   For information, see <a href="https://experienceleague.adobe.com/en/docs/genstudio-for-performance-marketing/user-guide/intro/user-roles">User roles and permissions</a>. 
   </p>
  </td> 
  </tr> 
</tbody> 
</table> 

For more information about Workfront access requirements, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++  

## Share an Ideation space

1. Access the Ideation space of a Planning record. 

    For information, see one of the following articles:

    * [Create Planning records from Ideation space briefs](/help/quicksilver/planning/ideation/create-records-in-ideation-space-for-planning.md)
    * [Create briefs in the Ideation space](/help/quicksilver/planning/ideation/create-briefs-in-ideation-space.md)

1. Click **Share** in the upper-right corner, then click the **Settings** icon ![Settings icon](assets/setting-icon.png) in the upper-right corner of the **Share document** box.
1. In the Who has access list, choose from the following: 

    * **Only invited people can access**

        You must add individual users to the Ideation space and give them a permission level. 
    * **Everyone at < your company's Workfront environment > can comment**

        Everyone in your organization that has a Workflow and a Planning license in their access level can find and comment on the ideation. 
    * **Anyone with the link can comment**

        Anyone that you share a link to the ideation can comment on it, including people external to your organization. 

1. Click **Copy link** to generate a link to the ideation and share it with others. The link is added to your clipboard. 
1. Click the back arrow on the Settings box to go back to sharing. 
1. (Conditional) If you selected to share the ideation space with specific people, start typing their name or email address, then select one of the following permission levels: 

    | Ideation space permission  | Capabilities |
    |---|---|
    | **Editor** | Can edit, download and share the ideation space|
    | **Commenter** | Can view and comment on the ideation space|
    | **Viewer** | Can view the ideation space|

1. (Optional) Include a message with your assignment, then click **Invite**. 

    The users invited receives an email notification about their permission assignment. 

1. Click the **X** icon to close the **Share document** box. 











