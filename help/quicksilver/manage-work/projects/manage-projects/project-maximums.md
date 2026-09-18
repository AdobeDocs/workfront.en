---
title: Project Limits Overview
content-type: overview
product-area: projects
navigation-topic: manage-projects
description: Adobe Workfront has limits for how many objects can be associated with a project. Project limits are in place to improve product performance and enhance your experience with Workfront.
author: Alina
feature: Work Management
exl-id: 60576107-89f1-4328-89e2-5b1e5e243fd9
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/t6tfn132hAQe--u8g73CAFAfrJTf2qFi7yOhm4flP58
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
    internal-label: Work management
subfeature_v2:
  - id: f0dd7b45-76b5-49d4-afe3-39f436b6fbd3
    internal-label: Projects
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
topic_v2:
  - id: bce87dde-a4ab-44c9-8a18-ad66e4ddb377
    internal-label: Customer experience
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
    <tr> 
   <td role="rowheader"><p>Convert objects </p></td> 
   <td>Workfront has a 5-minute processing limit when converting objects. If the object has a large number of documents attached to it, it may fail to convert within the 5-minute limit. You might need to remove some of the documents and try again.</td> 
  </tr> 
 </tbody> 
</table>

<!--
 Notes from the table: 
     <p>For tasks limits: (This is NOT TRUE , but the PMs always wanted this to stay the way it is because they don't want customers creating projects bigger than this.)</p>
    <p>For issue limits: (this is true only for some clusters; according to Anna A., some clusters are set to a million.)</p>
    -->
