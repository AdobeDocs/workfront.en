---
filename: show-role-allocation-workload-balancer
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: Show role allocation for projects and initiatives in the Workload Balancer
description: Important: Your organization must purchase an additional license for the Adobe Workfront Scenario Planner so that you can view initiative information on a project. For information about obtaining the Workfront Scenario Planner, see Access needed to use the Adobe Workfront Scenario Planner.
---

# Show role allocation for projects and initiatives in the *Workload Balancer*

>[!IMPORTANT]
>
>Your organization must purchase an additional license for the *Adobe Workfront Scenario Planner* so that you can view initiative information on a project. For information about obtaining the *Workfront Scenario Planner*, see [Access needed to use the Adobe Workfront Scenario Planner](../scenario-planner/access-needed-to-use-sp.md).

After you connect projects and initiatives, you can manage their resource allocation side-by-side to ensure they

match. This avoids overallocating or underutilizing them.

This article describes how you can reconcile resources using the Role Allocation panel in *Workload Balancer* of a project.

For general information about reconciling resources between projects and initiatives, including prerequisites, see [Overview of reconciling resource allocations between projects and initiatives](../scenario-planner/overview-reconcile-allocations-between-projects-initiatives.md).

## Access requirements

You need to following: 

<table cellspacing="15"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p><em>Adobe Workfront</em><b> plan*</b> </p> </td> 
   <td><em>Business</em> or higher</td> 
  </tr> 
  <tr> 
   <td> <p><em>Adobe Workfront</em><b> license*</b> </p> </td> 
   <td> <p><em>Review</em> or higher</p> </td> 
  </tr> 
  <tr> 
   <td><b>Product</b> </td> 
   <td> <p>You must purchase an additional license for the <em>Adobe Workfront Scenario Planner</em> to access functionality described in this article.</p> <p>For information about obtaining the <em>Workfront Scenario Planner</em>, see <a href="../scenario-planner/access-needed-to-use-sp.md" class="MCXref xref">Access needed to use the Adobe Workfront Scenario Planner</a>. </p> </td> 
  </tr> <draft-comment>
   <tr data-mc-conditions=""> 
    <td><span class="bold">Access level configurations*</span> </td> 
    <td> <p>View or higher access to Projects </p> <p>Note: If you still don't have access, ask your <em>Workfront administrator</em> if they set additional restrictions in your access level. For information on how a <em>Workfront administrator</em> can change your access level, see <a href="../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
   </tr>
  </draft-comment>
  <tr data-mc-conditions=""> 
   <td><span class="bold">Access level configurations*</span> </td> 
   <td> <p>View or higher access to Projects </p> <p>Note: If you still don't have access, ask your <em>Workfront administrator</em> if they set additional restrictions in your access level. For information on how a <em>Workfront administrator</em> can change your access level, see <a href="../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> <draft-comment>
   <tr data-mc-conditions=""> 
    <td> <p><span class="bold">Object permissions</span> </p> </td> 
    <td> <p>View or higher permissions to the project</p> <p>For information on requesting additional access to a plan, see <a href="https://one.workfront.com/s/document-item?bundleId=the-new-workfront-experience&amp;topicId=Content%2FScenario_Planner%2Frequest-access-to-plan.htm" target="_blank">Request access to a plan in the <em>Workfront</em> <em>Scenario Planner</em></a>.</p> <p>For information about requesting additional access to a project, see <a href="../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects in Adobe Workfront</a>. </p> </td> 
   </tr>
  </draft-comment>
  <tr data-mc-conditions=""> 
   <td> <p><span class="bold">Object permissions</span> </p> </td> 
   <td> <p>View or higher permissions to the project</p> <p>For information on requesting additional access to a plan, see <a href="https://one.workfront.com/s/document-item?bundleId=the-new-workfront-experience&amp;topicId=Content%2FScenario_Planner%2Frequest-access-to-plan.htm" target="_blank">Request access to a plan in the <em>Workfront</em> <em>Scenario Planner</em></a>.</p> <p>For information about requesting additional access to a project, see <a href="../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects in Adobe Workfront</a>. </p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your *Workfront administrator*.

## Show role allocation for projects and initiatives in the *Workload Balancer*

If your company has purchased a *Workfront Scenario Planner* license, you can reconcile the resource allocations between the initiative and the project linked to it in the project-level *Workload Balancer*.

<ol> 
 <li value="1"> <p>(Conditional) Connect a project with an initiative using one of the methods described in the following articles:</p> 
  <ul> 
   <li> <p><a href="https://one.workfront.com/s/document-item?bundleId=the-new-workfront-experience&topicId=Content%2FScenario_Planner%2Fimport-projects-to-plans.htm&_LANG=enus" target="_top">Import projects to plans in the <em>Adobe Workfront</em> <em>Scenario Planner</em></a> </p> </li> 
   <li> <p><a href="https://one.workfront.com/s/document-item?bundleId=the-new-workfront-experience&topicId=Content%2FScenario_Planner%2Fpublish-scenarios-update-projects.htm&_LANG=enus" target="_top">Update or create projects by publishing initiatives in the <em>Adobe Workfront</em> <em>Scenario Planner</em></a> </p> </li> 
  </ul> <note type="important">
   If you make changes to resources on the initiative, you must re-publish the scenario that the initiative belongs to in order for the latest resource information from the initiative to update on the project. 
  </note> </li> 
 <li value="2"> <p>Go to the project where you want to review the allocation of job roles for the project as well as for the associated initiative. </p> </li> 
 <li value="3"> <draft-comment>
   <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click <em>Workload Balancer</em> in the left panel. </p>
  </draft-comment><p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click <em>Workload Balancer</em> in the left panel. </p> <p>You might have to click <span class="bold">Scheduling</span>, then <span class="bold">Switch to <em>Workload Balancer</em></span>. </p> </li> 
 <li value="4"> <p>Do one of the following:</p> 
  <ul> 
   <li> <p>Click <span class="bold">Month</span> to view the <em>Workload Balancer</em> by month, click the drop-down menu next to a month in the timeline <img src="assets/drop-down-next-to-month-month-view-wb.png">, then click&nbsp;<span class="bold">More</span>. </p> </li> 
   <li> <p>Click the <span class="bold">Show role allocation</span> icon <img src="assets/show-role-allocation-icon.png"> in the upper-right corner of the toolbar. </p> </li> 
  </ul> <p>The Role&nbsp;Allocation panel displays.</p> <p> <img src="assets/role-allocation-panel-months-collapsed-350x319.png" style="width: 350;height: 319;"> </p> <p class="warning" data-mc-autonum="<b>Warning: </b>"><span class="autonumber"><span><b>Warning: </b></span></span>Although you can view the Role Allocation panel even if your organization did not purchase a <em>Workfront Scenario Planner</em> license, you cannot view information about initiatives' job roles. </p> </li> 
 <li value="5"> <p>Review the following information in the <span class="bold">Project Totals</span> area of the Role Allocation panel: </p> 
  <table cellspacing="0"> 
   <col> 
   <col> 
   <tbody> 
    <tr> 
     <td role="rowheader">Job&nbsp;Role</td> 
     <td> <p>The names of the job roles associated with any of the following:</p> 
      <ul> 
       <li> <p>tasks on the project</p> </li> 
       <li> <p>issues on the project</p> </li> 
       <li> <p>initiative linked to the project</p> </li> 
      </ul> </td> 
    </tr> 
    <tr> 
     <td role="rowheader">Initiative Hours</td> 
     <td>The number of required hours associated with each job role on the initiative for the total duration of the initiative. </td> 
    </tr> 
    <tr> 
     <td role="rowheader">Planned Hours</td> 
     <td>The number of Planned Hours associated with each job role in the tasks or issues on the project for the total duration of the project. </td> 
    </tr> 
    <tr> 
     <td role="rowheader">Variance</td> 
     <td> <p>The difference between the hours required on the initiative and the planned hours associated with work on the project.&nbsp;<em>Workfront</em> calculates the Variance using this formula:</p> <p><code>Role Allocation Variance = Initiative Hours - Planned Hours</code> </p> <p>When resources are planned for more hours than required on the initiative, the Variance is negative and it displays in red. This means your resources are overallocated. </p> </td> 
    </tr> 
   </tbody> 
  </table> 
  <div class="tip_one-tip-with_bullets" data-mc-autonum="<b>Tip: </b>">
   <span class="autonumber"><span><b>Tip: </b></span></span> 
   <p>Planned Hours from the project do not display in the following scenarios: </p> 
   <ul> 
    <li> <p>When tasks or issues are not assigned to job roles, or users with a job role associated with them.</p> </li> 
    <li> <p>When tasks or issues have a Duration of zero. </p> </li> 
   </ul> 
  </div> <p>&nbsp;</p> </li> 
 <li value="6"> <p>(Optional) If the Variance column shows that your resources are overallocated, adjust one of the following:</p> 
  <ul> 
   <li> <p>Lower the number of Planned Hours for one job role that shows overallocated or add more resources to the tasks and distribute more Planned Hours to the new resources. You can update assignments or the number of Planned Hours on tasks or issues when editing them.&nbsp;For more information see the following articles:</p> 
    <ul> 
     <li> <p><a href="../manage-work/tasks/manage-tasks/edit-tasks.md" class="MCXref xref">Edit tasks</a> </p> </li> 
     <li> <p><a href="../manage-work/issues/manage-issues/edit-issues.md" class="MCXref xref">Edit issues</a> </p> </li> 
    </ul> <note type="note">
     You must have additional access and permissions to edit tasks and issues.
    </note> </li> 
   <li> <p>Increase the number of required hours for role that shows the overallocation on the initiative. For more information, see<a href="https://one.workfront.com/s/document-item?bundleId=the-new-workfront-experience&topicId=Content%2FScenario_Planner%2Fcreate-and-edit-initiatives.htm&_LANG=enus" target="_top"> Create and edit initiatives in the <em>Adobe Workfront</em> <em>Scenario Planner</em></a>. </p> <note type="note">
     You must have additional access and permissions to edit plans. 
    </note> </li> 
  </ul> </li> 
 <li value="7"> <p>(Optional) Click the drop-down icon to expand one of the months in the Role Allocation panel or in the timeline of the <em>Workload Balancer</em>. </p> <p> <img src="assets/month-expanded-highlighted-role-allocation-panel-wb-350x145.png" style="width: 350;height: 145;"> </p> <p>The same type of information displayed in the Project Totals area also displays for each month. </p> <note type="tip">
   The months listed in the Role Allocation panel are the months in the timeline displayed on the screen in the 
   <em>Workload Balancer</em>. Scroll back and forward on the timeline to view additional months. 
  </note> </li> <draft-comment>
  <li value="8" data-mc-conditions="QuicksilverOrClassic.Draft mode"> <p>&nbsp;</p> </li>
 </draft-comment>
 <li value="8" data-mc-conditions="QuicksilverOrClassic.Draft mode"> <p>&nbsp;</p> </li> 
</ol>

&nbsp;
