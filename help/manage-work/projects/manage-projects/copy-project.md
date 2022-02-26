---
filename: copy-project
product-area: projects
navigation-topic: manage-projects
title: Copy a project
description: You can copy a project rather than create a new one from scratch.
---

# Copy a project

You can copy a project rather than create a new one from scratch.

## Access requirements

You must have the following:

<table cellspacing="15"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p><em>Adobe Workfront</em> plan*</p> </td> 
   <td>Any</td> 
  </tr> 
  <tr> 
   <td> <p><em>Adobe Workfront</em> license*</p> </td> 
   <td> <p><em>Plan</em> </p> </td> 
  </tr> <draft-comment>
   <tr data-mc-conditions=""> 
    <td><span class="bold">Access level configurations*</span> </td> 
    <td> <p>Edit access to Projects with ability to Create <span>and Copy</span> projects</p> <p>Note: If you still don't have access, ask your <em>Workfront administrator</em> if they set additional restrictions in your access level. For information on how a <em>Workfront administrator</em> can change your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
   </tr>
  </draft-comment>
  <tr data-mc-conditions=""> 
   <td><span class="bold">Access level configurations*</span> </td> 
   <td> <p>Edit access to Projects with ability to Create <span>and Copy</span> projects</p> <p>Note: If you still don't have access, ask your <em>Workfront administrator</em> if they set additional restrictions in your access level. For information on how a <em>Workfront administrator</em> can change your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> <draft-comment>
   <tr data-mc-conditions=""> 
    <td> <p><span class="bold">Object permissions</span> </p> </td> 
    <td> <p>View permissions or higher to the project</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects in Adobe Workfront</a>.</p> </td> 
   </tr>
  </draft-comment>
  <tr data-mc-conditions=""> 
   <td> <p><span class="bold">Object permissions</span> </p> </td> 
   <td> <p>View permissions or higher to the project</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects in Adobe Workfront</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your *Workfront administrator*.

## Copy a project

<ol> 
 <li value="1">Go to the project that you want to copy.</li> 
 <li value="2"> <p> <draft-comment>
    <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
     Click the 
     <span class="bold">More</span> icon 
     <img src="assets/qs-more-menu.png"> next to the name of the project, then click 
     <span class="bold">Copy</span>. 
    </MadCap:conditionalText>
   </draft-comment><MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
    Click the 
    <span class="bold">More</span> icon 
    <img src="assets/qs-more-menu.png"> next to the name of the project, then click 
    <span class="bold">Copy</span>. 
   </MadCap:conditionalText><br></p> <p> </p> </li> 
 <li value="3"> <p>Specify a name for the project.<br></p> <p>By default, the new name is <span class="bold">Copy of [Original project name].</span></p> </li> 
 <li value="4"> <p>Select the <span class="bold">Status</span> of your new project. </p> <p>By default, the <span class="bold">Status</span> matches that of the original project.</p> </li> 
 <li value="5"> <p>(Optional) Select any of the following options to remove the items from the new project.</p> <note type="important"> 
   <p> The following items are never copied from an existing project to a new one: <br></p> 
   <ul> 
    <li>Issues<br></li> 
    <li>Billing Rates</li> 
    <li>Billing Records<br></li> 
    <li>Notes<br></li> 
    <li>Hours</li> 
    <li>Cross-project predecessors</li> 
   </ul> 
   <p>The following items are always copied from an existing project to a new one:</p> 
   <ul> 
    <li>Tasks</li> 
    <li>Template</li> 
    <li>Risks</li> 
    <li>Queue Setup information</li> 
    <li>Portfolio and Program</li> 
    <li>Scorecard</li> 
    <li>Task Default information (Task Default Approval Process, Task Default Custom Forms)</li> 
   </ul> 
  </note> <p>If you leave any of the following items unselected, they transfer to the copied project by default:</p> 
  <ul> 
   <li><span class="bold">Clear Assignments</span>: Removes all the project and task assignments</li> 
   <li><span class="bold">Clear Progress</span>: Removes the progress on all the tasks.</li> 
   <li> <p><span class="bold">Clear Custom Data</span>: Removes the information from the custom form on the project, as well as the information on the custom forms associated with the following items:</p> 
    <ul> 
     <li>Tasks</li> 
     <li>Expenses</li> 
     <li> <p>Documents</p> </li> 
    </ul> <p>The custom forms will remain attached to the tasks, expenses, documents, and the project, but the information in the custom fields of the forms is not copied to the new project. </p> </li> 
   <li> <p><span class="bold">Clear Documents</span>: Removes everything in the documents tab, including document versions, linked documents, and folders.</p> <p>By default, document <em>proofs</em> and approvals cannot be copied to another project. </p> </li> 
   <li> <p><span class="bold">Clear All Predecessors</span>: Removes all predecessor relationships between the tasks on the project. </p> <note type="tip">
     Cross-project predecessors never transfer to the new project, regardless of whether this is selected or not. 
    </note> </li> 
   <li> <p><span class="bold">Clear Financial Information</span>: Removes the informationin the following areas: </p> 
    <ul> 
     <li>Finance sub-tab of the project</li> 
     <li> Planned Benefit in the Business Case</li> 
     <li>Financial information from all tasks<br></li> 
    </ul> <p>For more information about the project Finance sub-tab, see <a href="../../../manage-work/projects/project-finances/manage-project-finance-area.md" class="MCXref xref">Manage information in the project Finance area</a>.</p> </li> 
  </ul> 
  <ul> 
   <li><span class="bold">Clear Approval Process</span>: Removes all approvals associated with the tasks or the project. </li> 
   <li><span class="bold">Clear Reminder Notifications</span>: Removes the Reminder Notifications associated with the tasks or the project. </li> 
   <li><span class="bold">Clear Expenses</span>: Removes expenses associated with the tasks or the project. </li> 
   <li> <p><span class="bold">Clear Permissions</span>: Removes permissions to all the users on the tasks or the project.</p> <note type="note">
     Permissions are removed from users who are assigned to the copied tasks, even if 
     <span class="bold">Clear Assignments</span> is not selected.
    </note> </li> 
   <li><span class="bold">Select all</span>: Select this option to select all the options above and clear all the fields and objects listed from the new project.</li> 
  </ul> </li> 
 <li value="6"> <p>Click <span class="bold">Copy</span> to create a copy of the project.</p> <p>This creates a new project which is similar to the project you copied.<br></p> <p>You can start making changes to your new copied project, like review task assignments or adjust timelines.</p> </li> 
</ol>

