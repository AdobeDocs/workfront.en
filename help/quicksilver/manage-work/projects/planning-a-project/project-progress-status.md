---
content-type: overview
product-area: projects
navigation-topic: plan-a-project
title: Project Progress Status Overview
description: Adobe Workfront determines the Progress Status of a project by looking at the progression of the project across its timeline. You can configure Workfront to determine the Condition of a project based on the value of the Progress Status of the tasks. Learn more about Project Progress Status in this article .
author: Alina
feature: Work Management
exl-id: 922ca4cf-c526-4704-9966-de67b0c36a2a
TQID: https://experienceleague.adobe.com/V9eyzkoYIREb4zUuDxmyDhnQa54YQaYTv2woNTOhq24
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
    internal-label: Work management
subfeature_v2:
  - id: b91c0848-76c4-4da4-8b81-3aade0518dd0
    internal-label: Tasks
  - id: f0dd7b45-76b5-49d4-afe3-39f436b6fbd3
    internal-label: Projects
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
---
# Project Progress Status overview

<!--Audited: 12/2023-->

Adobe Workfront determines the Progress Status of a project by looking at the progression of the project across its timeline. You can configure Workfront to determine the Condition of a project based on the value of the Progress Status of the tasks. For more information about configuring the Condition of the project, see the article [Overview of Project Condition and Condition Type](../../../manage-work/projects/manage-projects/project-condition-and-condition-type.md).

The following are the Progress Statuses of projects in Workfront: 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>On Time</td> 
   <td> The Progress Status of a project is <strong>On Time</strong> if:<ul><li>If both Projected and Estimated Due Dates are earlier than or equal to the project's Planned Completion Date <p> <img src="assets/project-on-time-progress-status-350x69.png" style="width: 350;height: 69;"> </p></li></ul>  </td> 
  </tr> 
  <tr> 
   <td>At Risk</td> 
   <td> The Progress Status of a project is <strong>At Risk</strong> if <strong>all</strong> of the following are true:<ul><li>Both the Estimated and Projected Completion Dates are in the future</li><li> The Estimated Due Date is later than both the Planned Completion Date and the Projected Completion Date <p> <img src="assets/project-at-risk-progress-status-350x67.png" style="width: 350;height: 67;"> </p></li></ul> </td> 
  </tr> 
  <tr> 
   <td>Behind</td> 
   <td> The Progress Status of a project is <strong>Behind</strong> if <strong>all</strong> of the following are true:<ul><li>Both the Estimated and Projected Completion Dates are in the future</li><li> Both the Estimated and Projected Completion Dates are later than the Planned Completion Date of the project</li><li> The Estimated Due Date is not later than Projected Completion Date
   <p> <img src="assets/project-behind-progress-status-350x67.png" style="width: 350;height: 67;"> </p></li></ul>  </td> 
  </tr> 
  <tr> 
   <td>Late</td> 
   <td> 
     The Progress Status of a project is <strong>Late</strong> if <strong>either</strong> of the following are true:<ul><li>The project is complete and the Actual Completion Date is later than the Planned Completion Date <p> <img src="assets/project-late-progress-status-350x66.png" style="width: 350;height: 66;"> </p> </li> 
     <li> <p>The project is not complete and the Planned Completion Date of the project is in the past <p> <img src="assets/project-late-progress-status-incomplete-status-350x66.png" style="width: 350;height: 66;"> </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

Consider the following:

* The Projected Completion Date of the project is driven by the task on the Critical Path with the latest Projected Completion Date.
* The Estimated Due Date of the project is driven by the task on the Critical Path with the latest Estimated Due Date.

For information about the project Critical Path, see [Overview of the project Critical Path](../../../manage-work/tasks/manage-tasks/critical-path.md).

For information about Projected Completion Dates, see [Overview of the Projected Completion Date for projects, tasks, and issues](../../../manage-work/projects/planning-a-project/project-projected-completion-date.md).
