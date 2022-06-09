---
user-type: administrator
content-type: reference
product-area: system-administration;workfront-integrations
navigation-topic: best-practices-catalog
title: Actions to take after installing a blueprint
description: This article outlines what you should do after you install a blueprint in Adobe Workfront to fully deploy the blueprint to your system users.
feature: System Setup and Administration
role: Admin
---

# Actions to take after installing a blueprint

This article outlines what you should do after you install a blueprint in Adobe Workfront to fully deploy the blueprint to your system users.

* [Project template recommendations](#project-template-recommendations) 
* [Organizational structure recommendations](#organizational-structure-recommendations)

## Project template recommendations {#project-template-recommendations}

This section contains recommendations for the project templates installed with your blueprints.

* [Assign users to newly created roles and teams](#assign-users-to-newly-created-roles-and-teams) 
* [Apply a custom form to the template and the template tasks](#apply-a-custom-form-to-the-template-and-the-template-tasks) 
* [Update template task duration and effort estimates](#update-template-task-duration-and-effort-estimates) 
* [Associate a milestone path and milestones](#associate-a-milestone-path-and-milestones) 
* [Roll out the template to your team](#roll-out-the-template-to-your-team) 
* [Create or update reports and dashboards](#create-or-update-reports-and-dashboards)

### Assign users to newly created roles and teams {#assign-users-to-newly-created-roles-and-teams}

The roles and/or teams created during the blueprint installation process do not have users associated with them automatically. Without assigning users to the newly added roles or teams, you will create work for a function that no one will pick up. In some cases, you might need to create new users to fill these roles and teams. For information on creating new users, see [Add users](../../administration-and-setup/add-users/create-and-manage-users/add-users.md).

### Apply a custom form to the template and the template tasks {#apply-a-custom-form-to-the-template-and-the-template-tasks}

The installation process does not associate the project template with any custom forms. If your projects or your tasks require specific forms or fields to be populated to create reporting consistency, or if your digital request form contains fields that need to be retained at the project level, we recommend that you associate the template or the template tasks with those forms. For information, see [Add a custom form to an object](../../workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md).

### Update template task duration and effort estimates {#update-template-task-duration-and-effort-estimates}

Every task in the template contains a planned duration and planned effort estimate. These estimates serve as a starting point for durations and time spent for these activities. However, your organization's capabilities, skills, and pace are unique. You should review each task's estimated duration and effort to adjust it to reflect your organization's needs. For information, see [Manage task information in the Task Details Overview area](../../manage-work/tasks/manage-tasks/task-information-in-overview.md).

### Associate a milestone path and milestones {#associate-a-milestone-path-and-milestones}

The installation process does not associate the project template with a milestone path. Apply a milestone path to the template and apply milestones to key tasks in the template to support your milestone reporting needs. For information, see [Associate milestones with tasks](../../manage-work/tasks/manage-tasks/associate-milestones-with-tasks.md).

### Roll out the template to your team {#roll-out-the-template-to-your-team}

Prepare training materials for both the work managers who will use this template and the individual contributors who will execute the work within the project template.

### Create or update reports and dashboards {#create-or-update-reports-and-dashboards}

If the solution represents a new type of work that your organization has not performed previously in Workfront, you may need to create new reports and dashboards to support the work. For information, see [Create a custom report](../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md) and [Create a dashboard](../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/create-dashboard.md).

If the solution is similar to work that you have already been executing in Workfront, then you should verify that the work feeds into existing reports and dashboards as expected. If it does not feed into your existing reporting, take action to update filters or create new reports.

## Organizational structure recommendations {#organizational-structure-recommendations}

This section contains recommendations for the organizational structure elements installed with your blueprints.

### Companies

Note that companies are currently only available on certain blueprints in the Preview environment.

After installing a blueprint that includes a company:

* Add a custom form to augment the company record with useful details (the form and its details are unique to you). For information, see [Add a custom form to an object](../../workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md).
* If the company represents a client, review the override rates associated with the company. For information, see [Override job role billing rates at the company level](../../administration-and-setup/set-up-workfront/organizational-setup/override-job-role-billing-rates-company-level.md).
* If the company represents a client, and if there are other unique-to-that-organization project templates, firstpre-associate the project templates with the newly added company. For information, see [Edit project templates](../../manage-work/projects/create-and-manage-templates/edit-templates.md).
* If the company represents a client or a vendor, associate existing users from the external organization that may be in your environment already. For information, see [Create and edit companies](../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md).
* If the company represents a client or a vendor, create additional collaborator users for the external organization that you may need in your environment to streamline communication, work execution, and approvals. For information on creating new users, see [Add users](../../administration-and-setup/add-users/create-and-manage-users/add-users.md).
* Update organizational chart relationships for any users now associated with the newly added company. For information, see [Create direct reports](../../administration-and-setup/add-users/create-and-manage-users/create-direct-reports.md) and [View the organizational chart](../../people-teams-and-groups/work-directly-with-others/view-the-org-chart.md).

For additional information on companies, see [Create and edit companies](../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md).

