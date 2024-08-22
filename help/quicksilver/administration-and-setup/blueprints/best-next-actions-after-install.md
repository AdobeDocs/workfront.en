---
user-type: administrator
content-type: reference
product-area: system-administration;workfront-integrations
navigation-topic: best-practices-catalog
title: Actions to Take after Installing a Blueprint
description: This article outlines what you should do after you install a blueprint in [!DNL Adobe Workfront] to fully deploy the blueprint to your system users.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 6e5da58f-105a-4edf-8fc1-65e8762d43c6
---
# Actions to take after installing a blueprint

This article outlines what you should do after you install a blueprint in [!DNL Adobe Workfront] to fully deploy the blueprint to your system users.

* [Project template recommendations](#project-template-recommendations)
* [Organizational structure recommendations](#organizational-structure-recommendations)
* [Dashboard recommendations](#dashboard-recommendations)

## Project template recommendations {#project-template-recommendations}

This section contains recommendations for the project templates installed with your blueprints.

### Assign users to newly created roles and teams {#assign-users-to-newly-created-roles-and-teams}

The roles and/or teams created during the blueprint installation process do not have users associated with them automatically. Without assigning users to the newly added roles or teams, you will create work for a function that no one will pick up. In some cases, you might need to create new users to fill these roles and teams. For information on creating new users, see [Add users](../../administration-and-setup/add-users/create-and-manage-users/add-users.md).

### Apply a custom form to the template and the template tasks {#apply-a-custom-form-to-the-template-and-the-template-tasks}

The installation process does not associate the project template with any custom forms. If your projects or your tasks require specific forms or fields to be populated to create reporting consistency, or if your digital request form contains fields that need to be retained at the project level, we recommend that you associate the template or the template tasks with those forms. For information, see [Add a custom form to an object](../../workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md).

### Update template task duration and effort estimates {#update-template-task-duration-and-effort-estimates}

Every task in the template contains a planned duration and planned effort estimate. These estimates serve as a starting point for durations and time spent for these activities. However, your organization's capabilities, skills, and pace are unique. You should review each task's estimated duration and effort to adjust it to reflect your organization's needs. For information, see [Manage task information in the [!UICONTROL Task Details Overview] area](../../manage-work/tasks/manage-tasks/task-information-in-overview.md).

### Associate a milestone path and milestones {#associate-a-milestone-path-and-milestones}

The installation process does not associate the project template with a milestone path. Apply a milestone path to the template and apply milestones to key tasks in the template to support your milestone reporting needs. For information, see [Associate milestones with tasks](../../manage-work/tasks/manage-tasks/associate-milestones-with-tasks.md).

### Roll out the template to your team {#roll-out-the-template-to-your-team}

Prepare training materials for both the work managers who will use this template and the individual contributors who will execute the work within the project template.

### Create or update reports and dashboards {#create-or-update-reports-and-dashboards}

If the solution represents a new type of work that your organization has not performed previously in [!DNL Workfront], you may need to create new reports and dashboards to support the work. For information, see [Create a custom report](../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md) and [Create a dashboard](../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/create-dashboard.md).

If the solution is similar to work that you have already been executing in [!DNL Workfront], then you should verify that the work feeds into existing reports and dashboards as expected. If it does not feed into your existing reporting, take action to update filters or create new reports.

## Organizational structure recommendations {#organizational-structure-recommendations}

This section contains recommendations for the organizational structure elements installed with your blueprints.

### Companies

After installing a blueprint that includes a company:

* Add a custom form to augment the company record with useful details (the form and its details are unique to you). For information, see [Add a custom form to an object](../../workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md).
* If the company represents a client, review the override rates associated with the company. For information, see [Override job role billing rates at the company level](../../administration-and-setup/set-up-workfront/organizational-setup/override-job-role-billing-rates-company-level.md).
* If the company represents a client, and if there are other unique-to-that-organization project templates, first pre-associate the project templates with the newly added company. For information, see [Edit project templates](../../manage-work/projects/create-and-manage-templates/edit-templates.md).
* If the company represents a client or a vendor, associate existing users from the external organization that may be in your environment already. For information, see [Create and edit companies](../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md).
* If the company represents a client or a vendor, create additional collaborator users for the external organization that you may need in your environment to streamline communication, work execution, and approvals. For information on creating new users, see [Add users](../../administration-and-setup/add-users/create-and-manage-users/add-users.md).
* Update organizational chart relationships for any users now associated with the newly added company. For information, see [Create direct reports](../../administration-and-setup/add-users/create-and-manage-users/create-direct-reports.md) and [View the organizational chart](../../people-teams-and-groups/work-directly-with-others/view-the-org-chart.md).

For additional information on companies, see [Create and edit companies](../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md).

## Dashboard recommendations {#dashboard-recommendations}

This section contains recommendations for the dashboards and reports installed with a blueprint.

### Update the newly created dashboards to add/remove reports

The dashboards added from a blueprint have one or more reports, external pages, or calendars. It is likely that you will either not need all the reports and other dashboard elements, or you will need to augment the dashboard with existing reports, external pages, and calendars before it is ready to share with other people. For information, see [Add a report to a dashboard](/help/quicksilver/reports-and-dashboards/dashboards/creating-and-managing-dashboards/add-report-dashboard.md).

### Update the newly created reports to add/remove columns or filter criteria

The reports distributed through a dashboard blueprint do not have all the columns or filter criteria to support your configuration of [!DNL Workfront]. It is expected that you will make some adjustments to the reports to fit within your standards. To build consistency with other reports in your environment, you may want to add a column you include on all reports for the object being listed, or to add some filter criteria that limit results to a particular project type or user group. For information, see [Create or edit views](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/create-edit-views.md) and [Create or edit filters](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/create-filters.md).

### Share the dashboards or reports with users

If you are not planning to place the dashboard on a layout template, you should share the dashboard with the people who will find it useful. For information, see [Share a dashboard](/help/quicksilver/reports-and-dashboards/dashboards/creating-and-managing-dashboards/share-dashboard.md) and [Share a report](/help/quicksilver/reports-and-dashboards/reports/creating-and-managing-reports/share-report.md).

### Add the dashboards to layout templates

The best way to make information available to other people is to add dashboards to layout templates. Identify the layout templates of the people who would most benefit from reviewing the dashboard on a regular basis and add the newly created dashboard to those layout templates. For information, see [Create and manage layout templates](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).

### Update other dashboards and reports

The introduction of a new dashboard and its reports may make it possible to retire and adjust other existing dashboards and reports. Take the time to review your existing reports to identify any redundant and contradictory reports.

### Distribute custom data to relevant forms

Some reports included in a dashboard blueprint have custom data fields in either the view, filter, or grouping of the report. In some cases, the blueprint will also have a form that these fields are associated with. However, more often than not, the custom fields are not applied to a custom form. For the columns, filters, or groupings to work correctly, these fields must be associated with forms that are connected to a user, project, task, or other object record. For information, see [Design a form with the form designer](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).
