---
filename: remove-users-from-projects
product-area: projects;user-management
navigation-topic: manage-projects
title: Remove users from projects
description: You can remove users from a project when they are no longer involved in completing work on the project. Removing users from projects has implications on task and issue assignments, as well as on project roles.
---

# Remove users from projects

You can remove users from a project when they are no longer involved in completing work on the project. Removing users from projects has implications on task and issue assignments, as well as on project roles.

The users associated with a project are listed in the 

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
People area
</MadCap:conditionalText>
-->

`<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver"> People area</MadCap:conditionalText>` of a project. They represent the Project Team.&nbsp;For more information about the Project Team, see [Project Team overview](../../../manage-work/projects/planning-a-project/project-team-overview.md).

You can assign work to the users on the project in the 

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
People area
</MadCap:conditionalText>
-->

`<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver"> People area</MadCap:conditionalText>` of a project.

## Access requirements

You must have the following access to perform the steps in this article:

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><em>Adobe Workfront</em> plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><em>Adobe Workfront</em> license*</td> 
   <td> <p><em>Plan</em> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Projects</p> <p>Note: If you still don't have access, ask your <em>Workfront administrator</em> if they set additional restrictions in your access level. For information on how a <em>Workfront administrator</em> can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions on the project</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects in Adobe Workfront</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your *Workfront administrator*.

## How removing a user affects existing tasks, issues, and projects&nbsp;

When a user is removed from a project, any tasks or issues assigned to them might be affected, depending on whether the task or issue was in an Active or Complete state when the user was removed:

* `If the item is in an Active state when the user is removed:` The item is re-assigned to a Job Role if a Job Role was already assigned. If the item&nbsp;did not have a Job Role assigned, you must manually re-assign the item. An item in an Active state is any item that has not completed yet.
* `If the item is in a Complete state when the user is removed:` The name of the removed user remains on&nbsp;the item.
* If the user removed is also the creator of a project, the project is not removed from their `Projects I'm On` 

  <!--
  <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
  list
  </MadCap:conditionalText>
  -->

  `<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver"> list</MadCap:conditionalText>` in the Projects area. The project is removed from the lists for all other users that filter for that project by the Entered By field.

## Remove users from a project and Project Team

When you remove a user from the project, the user is also removed from the project team. Likewise, when you remove a user from the project team, the user is also removed from the project.

You can remove users from a project from the People 

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
section
</MadCap:conditionalText>
-->

`<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver"> section</MadCap:conditionalText>`of the project.

  <!--
  <li data-mc-conditions="QuicksilverOrClassic.Quicksilver"><a href="#remove" class="MCXref xref">Remove users from a project from the People area</a> </li>
  -->

* [Remove users from a project from the People area](#remove)

<!--
<h3 data-mc-conditions="QuicksilverOrClassic.Quicksilver"><a name="Remove"></a>Remove users from a project from the People area</h3>
-->

### Remove users from a project from the People area

<ol> 
 <li value="1">Go to the project where you want to remove the users.</li> 
 <li value="2">Click <span class="bold">People</span> <draft-comment>
   <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
    in the left panel
   </MadCap:conditionalText>
  </draft-comment><MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
   in the left panel
  </MadCap:conditionalText>,&nbsp;then select the users you want to remove. <draft-comment>
   <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
    This might be located under the 
    <span class="bold">Show More</span> area. 
   </MadCap:conditionalText>
  </draft-comment><MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
   This might be located under the 
   <span class="bold">Show More</span> area. 
  </MadCap:conditionalText><br></li> 
 <li value="3">Click <span class="bold">Remove</span><draft-comment>
   <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
    <img src="assets/remove-icon---x-in-circle.png" alt="Remove item">
   </MadCap:conditionalText>
  </draft-comment><MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
   <img src="assets/remove-icon---x-in-circle.png" alt="Remove item">
  </MadCap:conditionalText>.</li> 
 <li value="4">Click&nbsp;<span class="bold">Yes, Remove Selected Users</span> to confirm removal.</li> 
</ol>

