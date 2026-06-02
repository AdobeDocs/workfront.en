---
product-area: projects
navigation-topic: update-work-in-a-project
title: Interactions Between the Commit Date and the Planned Completion Date
description: Both the Planned Completion and the Commit Dates indicate when the task should be completed. But they differ because of who sets each date.
author: Alina
feature: Work Management
exl-id: 1709c60c-ac75-48eb-9226-ec2cf556ebf0
TQID: https://experienceleague.adobe.com/iy-L6-ZnhDgVTJjhEBlqwdRH3TRA5OqT3Gj-LIoEgDA
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
topic_v2:
  - id: bce87dde-a4ab-44c9-8a18-ad66e4ddb377
    internal-label: Customer experience
---
# Interactions between the Commit Date and the Planned Completion Date

<!--
this article has mostly information that is repeated from the articles linked from here. I left it in here for searchability's sake.
-->

Both the Planned Completion and the Commit Dates indicate when the task should be completed. But they differ because of who sets each date.

## Overview of the Commit Date and Planned Completion Date
 
Planned Completion and Commit Dates exist on both tasks and issues.

The following table contains information about the difference between the Commit and Planned Completion dates:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Commit Date</td> 
   <td> <p>The Commit Date is the date by which the person assigned to a task or issue manually estimates that they will have completed the task or issue.</p> <p>For information about Commit Dates, see <a href="../../../manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md" class="MCXref xref">Commit Date overview</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Planned Completion Date</td> 
   <td> <p>The Planned Completion Date shows when the project owner expects the task or issue to be completed. It can be either manually set by the project owner or anyone with Manage permissions to the task or issue or it can be automatically calculated by Adobe Workfront.</p> <p>For more information about Planned Completion dates, see <a href="../../../manage-work/tasks/task-information/task-planned-completion-date.md" class="MCXref xref">Overview of the task Planned Completion Date</a></p> </td> 
  </tr> 
 </tbody> 
</table>

## Interactions between the Commit Date and the Planned Completion Date

When the project owner creates and assigns a task or an issue, the task or issue will have the following:

* A Planned Completion Date
* No Commit Date

The assignee working on the task or issue can manually update the Commit Date or automatically update it by accepting to work on it. This is a visual way to indicate to the project owner when it would be realistic for them to complete the task or the issue.

>[!TIP]
>
>Only the assignee can update the Commit Date of a task or issue.

The assignee changing the Commit Date does not automatically change the Planned Completion Date. The reverse is also true: changing the Planned Completion Date will not change the Commit Date.

When the Commit Date changes, the Project Owner gets notified through a Workfront in-app notification that this change occurred. 

If the Commit Date offered by the assignee is acceptable to the project owner, they must manually update the Planned Completion Date on the task illustrate the impact it might have on the timeline of the project. Changes in the Planned Completion Date of issues do not impact the project timeline. 

For more information, see the following articles:

* [Commit Date overview](../../../manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md) 
* [Update Commit Dates on tasks and issues](../../../manage-work/projects/updating-work-in-a-project/update-commit-date-on-tasks-and-issues.md)
