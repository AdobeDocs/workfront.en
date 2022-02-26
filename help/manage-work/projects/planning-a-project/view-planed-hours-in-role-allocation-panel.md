---
filename: view-planed-hours-in-role-allocation-panel
product-area: projects
navigation-topic: plan-a-project
title: View project Planned Hours in the Role Allocation panel
description: You can view role allocation for all job roles assigned to work items in a project in the Role Allocation panel of the project.
---

# View project Planned Hours in the Role Allocation panel

You can view role allocation for all job roles assigned to work items in a project in the Role Allocation panel of the project.

>[!NOTE]
>
>This article refers to viewing the job roles associated with tasks and issues on a project and their allocated Planned Hours in the Role Allocation panel of a project.&nbsp;For information about reconciling Planned Hours with initiatives hours using the Role Allocation Panel when using the *Adobe Workfront Scenario Planner*, see the following:
>
>* >
>  <!-->
>  <p data-mc-conditions="QuicksilverOrClassic.Quicksilver"><a href="../../../scenario-planner/show-role-allocation-task-list-nwe.md" class="MCXref xref">Show role allocation for projects and initiatives in the task list</a> </p>>
>  -->
>  [Show role allocation for projects and initiatives in the task list](../../../scenario-planner/show-role-allocation-task-list-nwe.md) 
>
>* [Show role allocation for projects and initiatives in the Workload Balancer](../../../scenario-planner/show-role-allocation-workload-balancer.md) 
>
>  You must have a *Scenario Planner* license in order to see initiative hours in the Role Allocation panel.&nbsp;For information about the *Scenario Planner*, see >
>  <!-->
>  <a href="../../../scenario-planner/get-started-with-scenario-planning.md" class="MCXref xref" data-mc-conditions="QuicksilverOrClassic.Quicksilver">Get started with the Adobe Workfront Scenario Planner</a>>
>  -->
>  [Get started with the Adobe Workfront Scenario Planner](../../../scenario-planner/get-started-with-scenario-planning.md) . 
>

## Access requirements

You must have the following:

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><em>Adobe Workfront</em> plan*</td> 
   <td> <p>Any </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><em>Adobe Workfront</em> license*</td> 
   <td> <p><em>Review</em> or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>View or higher access to Projects</p> <p>Note: If you still don't have access, ask your <em>Workfront administrator</em> if they set additional restrictions in your access level. For information on how a <em>Workfront administrator</em> can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View or higher permissions on the project</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects in Adobe Workfront</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your *Workfront administrator*.

## Prerequisites

You must have the following:

<ul> 
 <li> <p>Tasks or issues assigned to job roles or to users associated with a job role. </p> <note type="tip">
   If the tasks or issues are unassigned, assigned to teams, or are assigned to users with no job role, the Planned Hours of the project is zero in the Role Allocation panel. 
  </note> </li> 
 <li> <p>Tasks and issues with a Duration higher than zero. </p> </li> 
</ul>

## View project Planned Hours in the Role Allocation panel

<ol> 
 <li value="1"> <draft-comment>
   <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click the <span class="bold">Main Menu</span> icon <img src="assets/main-menu-icon.png"> in the upper-right corner of <em>Adobe Workfront</em>, then click <span class="bold">Projects</span>.</p>
  </draft-comment><p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click the <span class="bold">Main Menu</span> icon <img src="assets/main-menu-icon.png"> in the upper-right corner of <em>Adobe Workfront</em>, then click <span class="bold">Projects</span>.</p> </li> 
 <li value="2"> <p>Click the name of a project to access it.&nbsp;This opens the Project page. </p> </li> 
 <li value="3"> <draft-comment>
   <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click one of the following in the left panel: </p>
  </draft-comment><p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click one of the following in the left panel: </p> 
  <ul> 
   <li> <draft-comment>
     <p data-mc-conditions="QuicksilverOrClassic.Quicksilver"><span class="bold">Tasks</span> </p>
    </draft-comment><p data-mc-conditions="QuicksilverOrClassic.Quicksilver"><span class="bold">Tasks</span> </p> </li> 
   <li> <draft-comment>
     <p data-mc-conditions="QuicksilverOrClassic.Quicksilver"><em>Workload Balancer</em> </p>
    </draft-comment><p data-mc-conditions="QuicksilverOrClassic.Quicksilver"><em>Workload Balancer</em> </p> <draft-comment>
     <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">You might need to click&nbsp;<span class="bold">Scheduling</span> > <span class="bold">Switch to <em>Workload Balancer</em></span>. </p>
    </draft-comment><p data-mc-conditions="QuicksilverOrClassic.Quicksilver">You might need to click&nbsp;<span class="bold">Scheduling</span> > <span class="bold">Switch to <em>Workload Balancer</em></span>. </p> </li> 
  </ul> </li> 
 <li value="4"> <p>Click the <span class="bold">Show role allocation</span> icon <img src="assets/show-role-allocation-icon.png">. </p> <p>The Role Allocation panel displays.</p> <p> <img src="assets/role-allocation-panel-planned-hours-only-350x316.png" style="width: 350;height: 316;"> </p> </li> 
 <li value="5"> <p>Review the following information in the <span class="bold">Role Allocation</span> panel:</p> 
  <table cellspacing="0"> 
   <col> 
   <col> 
   <tbody> 
    <tr> 
     <td role="rowheader">Job Role</td> 
     <td>Job roles assigned to tasks and issues on the project. These can be job roles assigned directly to tasks and issues or job roles associated with users assigned to tasks and issues on the project. </td> 
    </tr> 
    <tr> 
     <td role="rowheader">Planned Hours</td> 
     <td>The total number of Planned Hours from tasks and issues assigned to job roles or users associated with a job role on the project. </td> 
    </tr> 
   </tbody> 
  </table> </li> 
</ol>

&nbsp;
