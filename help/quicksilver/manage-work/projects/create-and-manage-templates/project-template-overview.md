---
product-area: templates
navigation-topic: templates-navigation-topic
title: Project template overview
description: You can use project templates to capture most of the repeatable processes, information, and settings associated with the projects in your organization.
author: Alina
feature: Work Management
exl-id: cac7662f-f2ae-44f0-a0bb-1569c03d172e
---
# Project template overview

<!-- Audited: 12/2023 -->

You can use project templates to capture most of the repeatable processes, information, and settings associated with the projects in your organization.

You can define tasks, queue topics, custom forms, attach documents in your template.

After creating templates, you can attach them to existing projects, or you can use them to build new projects. All the information on the template transfers to the projects that are created using it.

## Benefits for using templates in Adobe Workfront

The following are some of the benefits of using templates for creating your projects:

* It saves you time and effort when creating new projects that are repetitive.
* You have consistent information across projects that are similar in scope.
* It is helpful when reporting on projects. For example, you can report on projects that share the same template, to compare their progress and find improvements in how they could be completed. 
* In addition to defining the future project settings, you can add the following information for the future project on a template:

   * Tasks
   * Documents
   * Approvals
   * Queue Details
   * Queue Topics
   * Topic&nbsp;Groups
   * Routing Rules
   * Custom&nbsp;Forms
   * Company and Group information

## Best practices for creating templates

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE:this is not an extensive list, but we are updating it as we go.)</p>
-->

Consider the following when creating templates:

* Don't assign users to template tasks.&nbsp;Although you can leave the tasks unassigned, we recommend that you assign job roles to tasks. This will give you an idea what users might be able to be assigned to the tasks when you create the project using the template.
* Always give your template tasks a Duration and Planned Hours value. Every task in the project should be associates with a duration for how long the task can stay open and with a Planned Hour value for how much time will actually take for the task to complete. Tasks without this information cannot be properly budgeted for resources when using resource management tools in Workfront.

  For information about Duration, see the following articles:

   * [Overview of Task Duration and Duration Type](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md) 
   * [Overview of project Duration](../../../manage-work/projects/planning-a-project/project-duration.md)

  For information about Planned Hours, see [Planned Hours overview](../../../manage-work/tasks/task-information/planned-hours.md).

* Add the predecessor relationships between the tasks at the very end, when you have a clear understanding of the future project plan in its entirety. Adding predecessors to template tasks is similar to adding predecessors to tasks on a project.

  For information about adding predecessors to tasks, see [Overview of task predecessors](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md).

* Indicate who the template should be shared with for future use and who the projects that will be created from the template should be shared with. For information about sharing templates, see [Share project templates](../../../manage-work/projects/create-and-manage-templates/share-project-template.md).
* Use global approval processes and add them to your template and template tasks if possible. This will save time when tasks or the future project will need to go through the same approvals.

  For information about creating approvals, see [Create an approval process for work items](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

  For information about associating an approval process to a work item, see [Associate a new or existing approval process with work](../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md).

## Ways to create templates

You can create a new template in the following ways:

* From scratch.  
  For more information about creating a new template from scratch, see [Create a project template](../../../manage-work/projects/create-and-manage-templates/create-template.md).

* From existing projects, by saving a project as a template.  
  For more information about creating templates from existing projects, see [Create template from project](../../../manage-work/projects/create-and-manage-templates/create-template-from-project.md).

* By copying it from another template.  
  For more information about copying an existing template, see [Copy a project template](../../../manage-work/projects/create-and-manage-templates/copy-template.md).

* By using our example templates.   
  For more information about building your templates using our example templates, see [Create project templates from examples](../../../manage-work/projects/create-and-manage-templates/create-templates-from-examples.md).
