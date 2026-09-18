---
content-type: overview
product-area: projects
navigation-topic: plan-a-project
title: Overview of the project Actual Completion Date
description: Projects, tasks, and issues have an Actual Completion Date in Adobe Workfront. This is the date when the project, task, or issue were marked as completed.
author: Alina
feature: Work Management
exl-id: 0baba359-a61d-43d7-8336-1f45c7f34374
TQID: https://experienceleague.adobe.com/MoATj74YM1zoW2SsIGrpKY0gc9dHRKjlDvnPfT-kk2s
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
    internal-label: Work management
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
    internal-label: Administration
subfeature_v2:
  - id: b91c0848-76c4-4da4-8b81-3aade0518dd0
    internal-label: Tasks
  - id: f0dd7b45-76b5-49d4-afe3-39f436b6fbd3
    internal-label: Projects
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
    internal-label: Reporting
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
---
# Overview of the project Actual Completion Date

Projects, tasks, and issues have an Actual Completion Date in Adobe Workfront. This is the date when the project, task, or issue were marked as completed.

## Actual Completion Dates

The Actual Completion Date represents the real date and time when the work is completed. When a task or an issue is marked as Done or Complete, Workfront automatically sets the date of the change in status of the item as the Actual Completion Date of the task or the issue. If that date is not an accurate reflection of when the task or the issue was actually completed, then you can manually edit the Actual Completion Date.

For example, you can mark a task or an issue Done on Monday, but you know that the work was completed the previous Friday. After marking the task or the issue as Done, you can then manually update the Actual Completion Date of the task or issue to the date of the previous Friday to reflect the real completion. 

You cannot manually edit the Actual Completion Date of a project, but you can manually change the status of a project which can trigger a change to its Actual Completion Date. 

The Actual Completion Date of a project is set in the following ways:

* By manually updating the project's status: if the Completion Mode of the project is set to Manual and you manually change the status of the project to Complete, this triggers the Actual Completion Date of the project to be updated to the date and time of the last completed task. 
* Automatically, when the last task of the project completes: if the Completion Mode of the project is set to Automatic and you mark the last task as Complete or update the Actual Completion Date of the last task, the project's Actual Completion Date is also updated with that date. 

  For information about setting the Completion Mode of a project, see the article [Edit projects](../../../manage-work/projects/manage-projects/edit-projects.md).

  >[!NOTE]
  >
  >Workfront uses the Actual Completion Date from the project's task that completed last as the Actual Completion Date for the entire project.

A Workfront or group administrator determines whether Workfront uses today's date or the Planned Completion Date of a task or an issue when these are set to Complete or Closed. For information about setting task and issue preferences, see [Configure system-wide task and issue preferences](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

<!--this statement is confusing, not sure what it is referring to, so I am drafting this for now: The value for the Actual Completion Date is always what is considered the current date and time.-->



## Locate Actual Completion Dates

The Actual Completion Date is located in the following areas of Workfront:

* Project, Task, and Issue Details areas
* Edit Project, Task, and Issue boxes
* Project, Task, and Issue Updates area as a System Update.
* Project, task, or issue lists or reports. 

For more information about creating reports, see the article [Create a custom report](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).
