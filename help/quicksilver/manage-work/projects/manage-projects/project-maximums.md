---
title: Project limits overview
content-type: overview
product-area: projects
navigation-topic: manage-projects
description: Adobe Workfront has limits for how many objects can be associated with a project. Project limits are in place to improve product performance and enhance your experience with Workfront.
author: Alina
feature: Work Management
exl-id: 60576107-89f1-4328-89e2-5b1e5e243fd9
---
# Project limits overview

Adobe Workfront has limits for how many objects can be associated with a project. Project limits are in place to improve product performance and enhance your experience with Workfront.

The following objects associated with projects have the following limits:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><p>Tasks</p></td> 
   <td>  <p>The maximum number of tasks per project is 5,000. A warning message displays when the number of tasks approaches this maximum. When the maximum is reached, an error message displays and additional tasks cannot be added to the project.</p> <p>To avoid reaching this maximum, move tasks that are closed to another project designated for closed tasks. Reports on these projects may need to be adjusted.</p> 
   
   <b>IMPORTANT</b>

   For projects where tasks have a lot of dependencies, a performance degradation might occur in calculating the timeline or when working in the project. 
   
   For this reason, we recommend that the number of tasks in projects with complex dependencies should be much lower than the maximum allowed of 5,000 tasks. 
   
   Some examples of task dependencies that might influence or prevent recalculating the project's timeline are:

   <ul><li>Number of children</li>
   <li>Multiple levels of task indentation</li>
   <li>Number of predecessors</li>
   <li>Multiple assignments</li>
   </ul>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Issues</p></td> 
   <td>  <p>The maximum number of issues per project is 10,000. A warning message displays when the number of issues approaches this maximum. When the maximum is reached, an error message displays and additional issues cannot be added to the project.</p> <p>To avoid reaching this maximum, move issues that are closed to another project designated for closed issues. Reports on these projects may need to be adjusted.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Durations</p></td> 
   <td> <p>The maximum duration of a project must be 15 years for Workfront to automatically calculate its timeline. A warning message displays when the project duration approaches the maximum. When the maximum is reached, a warning message displays and the automatic timeline calculations no longer occurs.</p> <p>The automatic timeline calculations will resume as soon as a project's duration is reduced below 15 years by adjusting the dates of the tasks in the project.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Timeline calculations</p></td> 
   <td>Workfront does not perform automatic timeline calculations for projects that haven't been updated in 6 months and will not resume until an update is made.<p>For projects that haven't been updated in 3 months, Workfront performs timeline calculations weekly instead of nightly.</p><p>For information about calculating project timeline, see <a href="../../../manage-work/projects/manage-projects/recalculate-project-timeline.md" class="MCXref xref">Recalculate project timelines</a>. </p></td> 
  </tr> 
 </tbody> 
</table>

<!-- Notes from the table: 
     <p>For tasks limits: (This is NOT TRUE , but the PMs always wanted this to stay the way it is because they don't want customers creating projects bigger than this.)</p>
    <p>For issue limits: (this is true only for some clusters; according to Anna A., some clusters are set to a million.)</p>
    -->