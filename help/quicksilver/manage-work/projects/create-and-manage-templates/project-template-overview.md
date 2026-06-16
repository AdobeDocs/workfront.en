---
product-area: templates
navigation-topic: templates-navigation-topic
title: Project template overview
description: You can use project templates to capture most of the repeatable processes, information, and settings associated with the projects in your organization.
author: Alina
feature: Work Management
exl-id: cac7662f-f2ae-44f0-a0bb-1569c03d172e
TQID: https://experienceleague.adobe.com/9RlRNqkZYIcLjI5-he3f2BMtoXj3R--8MQbVUFmRHqI
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
    internal-label: Work management
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
    internal-label: Administration
  - id: e14a7f57-c82c-4874-a495-5d036cbbdc3d
    internal-label: Resource Management
subfeature_v2:
  - id: b04e3dc0-3a59-45b1-aa02-b0b6d5f87eff
    internal-label: Approvals
  - id: d87de1f9-8e24-4c4d-aa4c-a403075091a1
    internal-label: Custom forms
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
   * Topic Groups
   * Routing Rules
   * Custom Forms
   * Company and Group information

## Best practices for creating templates

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE:this is not an extensive list, but we are updating it as we go.)</p>
-->

Consider the following when creating templates:

* Don't assign users to template tasks. Although you can leave the tasks unassigned, we recommend that you assign job roles to tasks. This will give you an idea what users might be able to be assigned to the tasks when you create the project using the template.
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

* Decide which document storage you want to use for your future projects. Some organizations have access to the following document storage types:

  * Legacy Workfront storage
  * Adobe cloud storage

  Adding documents differs depending on the type of storage you choose. The type of storage you choose for your templates will affect the type of storage future projects will inherit. 

  Adding templates to existing projects will not affect the storage type of the project. 

  For more information, also see:

  * [Create a project template](/help/quicksilver/manage-work/projects/create-and-manage-templates/create-template.md)
  * [Document management overview for projects and related objects](/help/quicksilver/manage-work/projects/manage-projects/manage-documents-on-projects.md)

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
