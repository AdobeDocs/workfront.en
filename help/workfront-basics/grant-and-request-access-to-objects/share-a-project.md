---
filename: share-a-project
title: Share a project
product-area: projects
navigation-topic: grant-and-request-access-to-objects
title: Share a project in Adobe Workfront
description: Your Adobe Workfront administrator can grant you access to view or edit projects when assigning your access level. For more information, see Grant access to projects.
---

# Share a project in Adobe Workfront

Your Adobe Workfront administrator can grant you access to view or edit projects when assigning your access level. For more information, see [Grant access to projects](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md).

Along with the access level that users are granted, you can also grant them permissions to View, Contribute, or Manage specific projects that you have access to share.

Permissions are specific to one item in Workfront and define what actions one can take on that item.

## Considerations about sharing projects

In addition to the considerations below, also see [Overview of sharing permissions on objects in Adobe Workfront](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

<ul> 
 <li> <p>By default, the creator of a project has permissions to manage the project and is also designated as the Project Owner. If the project is assigned to another owner, that user also has permissions to manage the project. When the project creator (or owner) shares the project with other users, they grant certain permissions to those users to control what they can do as they work on the project.</p> <p>However, if a project owner does not have a Planner license, they do not have full access to manage the project. Only a user with a Plan license can have permissions to manage a project. For more information, see <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/how-access-levels-permissions-work-together.md" class="MCXref xref">How access levels and permissions work together</a>.</p> </li> 
 <li>You can share projects individually, or you can share several of them at a time. Sharing projects is identical to sharing other objects. For more information about sharing items in Workfront, see <a href="../../workfront-basics/grant-and-request-access-to-objects/share-an-object.md" class="MCXref xref">Share an object in Adobe Workfront</a>. </li> 
 <li> You can grant the following permissions to a project:&nbsp; 
  <ul>
   <li>View</li>
   <li>Manage</li>
   <li><p> Contribute</p><p><img src="assets/view-on-projects-190x207.png" style="width: 190;height: 207;"><img src="assets/contribute-on-projects-159x243.png" style="width: 159;height: 243;"><img src="assets/manage-on-projects-178x230.png" style="width: 178;height: 230;"><br></p></li>
  </ul></li> 
</ul>

* When you share a project, all the tasks, issues, and documents inherit the same permissions, unless otherwise specified.

  For information about managing the access to tasks and issues on the project based on a user's permissions to the project, see the  section in the article [Edit projects](../../manage-work/projects/manage-projects/edit-projects.md).

  The Workfront administrator can specify whether documents should inherit permissions from higher objects in the user's access level. For more information about restricting inherited permissions on documents, see [Create or modify custom access levels](../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

* You can remove inherited permissions from a project so that the children objects will not inherit them.&nbsp;For more information about removing inherited permissions from objects, see&nbsp; [Remove permissions from objects in Adobe Workfront](../../workfront-basics/grant-and-request-access-to-objects/remove-permissions-from-objects.md).

## Ways to share a project

You can share a project in the following ways:

* Manually by doing one of the following:

  * Adding users to the project team. When you add users to the project team, they automatically obtain View permissions to the project.   
    For more information about adding users to a project team, see the "Adding Users to a Project Team" section in [Project Team overview](../../manage-work/projects/planning-a-project/project-team-overview.md). 
  * Individually or bulk-sharing the projects when using the `Sharing` option.

    Sharing a project is similar to sharing all other objects in Adobe Workfront.

    For information about sharing objects in Workfront, see [Share an object in Adobe Workfront](../../workfront-basics/grant-and-request-access-to-objects/share-an-object.md).

<ul> 
 <li> <p>Automatically, by doing one of the following: </p> 
  <ul> 
   <li> <p>Place a project in a <span class="bold">Portfolio</span> or <span class="bold">Program</span> that is already shared with others. Users gain the same permissions to the project that they have for the portfolio or program. <br>For information about adding a project to a <span class="bold">Portfolio</span>, see <a href="../../manage-work/portfolios/create-and-manage-portfolios/add-projects-to-portfolios.md" class="MCXref xref">Add projects to a portfolio</a>.<br>For information about adding a project to a <span class="bold">Program</span>, see <a href="../../manage-work/portfolios/create-and-manage-programs/add-project-to-program.md" class="MCXref xref">Add a project to a program </a>.</p> <p>For information about viewing inherited permissions on an object, see <a href="../../workfront-basics/grant-and-request-access-to-objects/view-inherited-permissions-on-objects.md" class="MCXref xref">View inherited permissions on objects in Adobe Workfront</a>. </p> </li> 
  </ul> 
  <ul> 
   <li> <p>Add entities to Project Sharing on a template used to create the project. For information about sharing projects from templates, see <a href="../../workfront-basics/grant-and-request-access-to-objects/share-a-template.md" class="MCXref xref">Sharing a template</a>. </p> </li> 
   <li> <p>Define the project access template.</p> <p>To define the project access template, see <a href="../../workfront-basics/grant-and-request-access-to-objects/share-an-object.md" class="MCXref xref">Share an object in Adobe Workfront</a>. </p> <note type="tip">
     When attaching or saving a template, you can clear the Template Project Sharing rules.
    </note> </li> 
   <li> <p>Edit a project and defining the <b>When someone is given access to this project</b> setting.&nbsp;For more information, see <a href="../../manage-work/projects/manage-projects/edit-projects.md" class="MCXref xref">Edit projects</a>. </p> </li> 
  </ul> </li> 
</ul>

<!--
To view what users have inherited the access on the project from a portfolio or a program, do the following: Go to a project whose sharing permissions you want to view. Click the More menu , then click Sharing. Expand the Inherited Permissions list. This list displays the names of users that have access to either the portfolio or the program that the project belongs to and also have permissions to the project.
-->

<!--
Go to a project whose sharing permissions you want for all projects you create from scratch. Click the More menu, then click Sharing. In the Project Access box that displays, near the upper-right corner, click the gear icon , then click Set as my project access template. The entities that are granted permissions on the selected project have the same permissions for all the projects you create from scratch in the future. The project access template overrides the sharing defaults granted to you by the Workfront administrator in your Access Level. For more information about specifying sharing defaults for projects in the Access Level, see Grant access to projects. Click Save.
-->

## Limitations for different license types

* Users with a Worker license don't have&nbsp;permissions to manage projects. For Workers, the highest sharing permission is Contribute. 
* Users with a Request license can view project information, but they have limited project access. 
* An exception to changing the status of a project occurs when a user with View or Contribute permissions is also included in an approval process. They can approve the project, which changes the status of the project, but the status is the predefined status for approval or for rejection. 
* To be able to copy a project, a user must also have access to create projects in their Access Level.

<!--
Configure default permissions for a project As a project owner, you can configure the default permissions for View, Manage, and Contribute access that are used when sharing the project with others. When users share a project, the default permissions are used. Users can then adjust the default permissions when sharing the project, as described in Ways to share a project. To configure the default permissions that are included with each access level: Go to the project where you want to set the default permissions. Click the More menu , then click Edit. Click Access in the list on the left. In the When someone is given access to this PROJECT section, select permissions that you want to be available when users are given access to the project via sharing. Ensure that any permissions that you want to include in the selected access level are selected and deselect any permissions that you do not want to include in the selected permissions level. To view which permissions are available for each level, see Share a project in Adobe Workfront. Note: The Delete access in the Manage permission level determines whether users can delete the project itself. Users with Manage access to the project can delete tasks and issues within the project regardless of whether this option is selected, if they have Manage permissions to the tasks and issues. Click Save Changes.
-->

## Project permission options

The following table lists the permissions that users can grant when sharing a project. For more information about the access users get based on their license, see [Grant access to projects](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md).

<table border="1" cellspacing="15" cellpadding="1"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p><span class="bold">Actions</span> </p> </th> 
   <th> <p><span class="bold">Manage</span> </p> </th> 
   <th> <p><span class="bold">Contribute</span> </p> </th> 
   <th> <p><span class="bold">View</span> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Add Custom Form</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>&nbsp;</p> </td> 
   <td> <p>&nbsp;</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Update Custom Fields</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>&nbsp;</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Add An Approval Process</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>&nbsp;</p> </td> 
   <td> <p>&nbsp;</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Approve a Project</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Approve hours</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓&nbsp;</p> </td> 
   <td> <p>&nbsp;</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Create A Project</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>&nbsp;</p> </td> 
   <td> <p>&nbsp;</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Add Document(s)</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Add Issue(s)</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Add Task(s)</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>&nbsp;</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Copy Project</p> </td> 
   <td> <p>&nbsp;</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>&nbsp;</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Delete Project</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>&nbsp;</p> </td> 
   <td> <p>&nbsp;</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Modify Planned Dates</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>&nbsp;</p> </td> 
   <td> <p>&nbsp;</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Share Project</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Share System-wide</p> </td> 
   <td> <p>&nbsp;</p> </td> 
   <td> <p>&nbsp;</p> </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td> <p>View Project</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Updates/ comments</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Change Status</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>&nbsp;</p> </td> 
   <td> <p>&nbsp;</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Log Hours</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>&nbsp;</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Edit Assignments</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>&nbsp;</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Manage Baseline</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>&nbsp;</p> </td> 
   <td> <p>&nbsp;</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Manage Risks*</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>&nbsp;</p> </td> 
   <td> <p>&nbsp;</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Manage Finance*</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>&nbsp;</p> </td> 
   <td> <p>&nbsp;</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Add/ Edit Expenses*</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>&nbsp;</p> </td> 
  </tr> 
  <tr> 
   <td> <p>View Finance*</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Attach Template</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>&nbsp;</p> </td> 
   <td> <p>&nbsp;</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Save As Template</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Add/ Edit Business Case</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>&nbsp;</p> </td> 
   <td> <p>&nbsp;</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Edit Project Details</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>&nbsp;</p> </td> 
   <td> <p>&nbsp;</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Edit Staffing</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>&nbsp;</p> </td> 
   <td> <p>&nbsp;</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Export to MS Project</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Recalculate Finance/ Timeline*</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>&nbsp;</p> </td> 
   <td> <p>&nbsp;</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Set Queue Properties</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>&nbsp;</p> </td> 
   <td> <p>&nbsp;&nbsp;</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Edit Project in Bulk in a List</p> </td> 
   <td> <p>✓</p> </td> 
   <td>&nbsp;</td> 
   <td>&nbsp;</td> 
  </tr> 
 </tbody> 
</table>

&#42;Users without access to financial data cannot manage risks and finances for projects, even if they have Edit access to projects. For information about access to financial data, see [Grant access to financial data](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).
