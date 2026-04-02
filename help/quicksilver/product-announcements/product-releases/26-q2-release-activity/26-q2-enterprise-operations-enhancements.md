---
title: Second Quarter 2026 Enterprise Operations enhancements
description: Second Quarter 2026 Enterprise Operations enhancements
author: Becky
feature: Product Announcements
recommendations: noDisplay, noCatalog
---
# Second Quarter 2026 Enterprise Operations enhancements

This page describes Enterprise Operations enhancements made with the Second Quarter 2026 release to the Preview environment. These enhancements will be made available in the Production environment as noted.

For a list of all changes available at this point in the Second Quarter 2026 release cycle, see [Second Quarter 2026 release overview](/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-q1-release-overview.md).

## Enterprise Operations Capabilities now available in Adobe Workfront

>[!NOTE]
>
>Preview: April 2, 2026
>Production fast release: April 15, 2026
>Production for everyone: April 16, 2026

Advanced enterprise operations capabilities from Adobe Workfront are a unified and scalable way to manage finances, projects, and enterprise access. These capabilities provide the visibility and control that enterprises need to operate profitably and efficiently.

### Advanced financial management

>[!NOTE]
>
>These features are only available for organizations on the Workflow Ultimate package.

Forecast, track, and optimize your finances with multi-level cost and billing rate hierarchies.

The enhancements to financial management include:

* **Rate attributes**, which allow you to add additional dimensions to rates beyond the job role, so that rates can vary not only by job role but also by factors such as agency, location, brand, cost center, or others. By combining these attributes, Workfront can automatically select the correct rate for assignments, ensuring financial accuracy and consistency across projects.
   
   For more information, see [Define rate attributes](/help/quicksilver/administration-and-setup/manage-enterprise-operations/define-rate-attributes.md)
* **Rate cards**, which provide a structured way to manage client-specific billing, combining role-based rates and customizable attributes to ensure accurate and controlled project costing. 

   For more information, see [Manage rate cards](/help/quicksilver/administration-and-setup/manage-enterprise-operations/manage-rate-cards.md) and [Attach a rate card to a project](/help/quicksilver/manage-work/projects/project-finances/attach-rate-card-to-project.md).
* A new cost and revenue type called **User and Role Hourly**. When this task type is assigned, an advanced rate hierarchy logic determines the billing and cost rates from different levels including the rate card, the project, the assignment, the job role, and the user profile. User and Role Hourly is the only cost and revenue type that you can use to apply rate attributes and rate cards.

   For more information, see [Overview of revenue and cost hierarchy](/help/quicksilver/manage-work/projects/project-finances/overview-revenue-cost-hierarchy.md).
* A redesigned **Advanced Assignments** experience with expanded configurability brings greater visibility and control across rates, time frames and properties. 

   For more information, see [Create advanced assignments](/help/quicksilver/manage-work/tasks/assign-tasks/create-advanced-assignments.md).

   Before the Production release on April 16, a switch will be added to allow you to choose between the old and new Advanced Assignments experiences. The old experience will remain the default
* A **Job Role for Billing**, which allows you to bill a user under a different job role than their primary job role. This is useful when a person temporarily performs work that should be billed at a different rate.

   For more information, see [Set up a Job Role for Billing](/help/quicksilver/manage-work/projects/project-finances/set-up-job-role-for-billing.md).
* Date-effective **exchange rates**. 

   For more information, see [Set up exchange rates](/help/quicksilver/administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md).
* The ability to add an **overtime multiplier on tasks**, which multiplies all Planned Hours for that task and affects the Planned Revenue calculations.

   For more information, see [Define an overtime ratio](/help/quicksilver/manage-work/projects/project-finances/define-overtime-ratio.md).
* A project-level control to **preserve all billing information** and prevent any future modifications.

   For more information, see [Edit projects](/help/quicksilver/manage-work/projects/manage-projects/edit-projects.md).
* **A job role alias**, which is defined on a rate card. When the rate card is attached to a project, the alias appears on information such as placeholder assignments, expenses, and reports, instead of the internal job role name.

   For more information, see [Manage rate cards](/help/quicksilver/administration-and-setup/manage-enterprise-operations/manage-rate-cards.md).

### Historical data tracing

Use **project snapshots** to manage projects more effectively and make informed decisions.

For more information, see [Create and view project snapshots](/help/quicksilver/manage-work/projects/create-projects/create-snapshots.md).

>[!NOTE]
>
>* Project snapshots are only available for organizations on the Workflow Ultimate package.
>* Product snapshots will not have a Preview release, and will be released directly to Production on April 16.

### Enterprise permissions

**Business profiles** provide secure, scalable system access and help to strengthen enterprise governance. 

For more information, see [Business profiles overview](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/business-profiles.md).

>[!NOTE]
>
>Business profiles are only available for organizations on the Workflow Ultimate package.

Also, permissions to view both cost and billing data have been separated from the general finance permissions, both in the user access levels and in object permissions. For more information, see [Grant access to financial data](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md) and [Share financial permissions on an object](/help/quicksilver/workfront-basics/grant-and-request-access-to-objects/share-financial-permissions-object.md).

>[!NOTE]
>
>Separate cost and billing permissions are available for organizations on all Workfront and Workflow packages.

### Custom form and field enhancements

Advanced logic in custom forms provides clearer insights and more accurate project and financial management.

The enhancements to custom forms include:

* New **advanced logic types**: advanced display, default value, conditional formatting, and editability

   For more information, see [Add logic rules to custom forms and fields](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/display-skip-logic-form-designer.md).

   >[!NOTE]
   >
   >The new logic types are only available for organizations on the Workflow Prime or Ultimate packages.

* Enhancements to the form designer interface:
   * The form name now appears on the top left of the designer, allowing you to see the name on a long form when you scroll.
   * Object types that the form can attach to are in a dropdown list.
   * You can choose to display or hide logic indicators on the fields, for all logic types. Display and skip logic types show indicators for both affected fields. All other logic types affect one field.

   For more information, see [Create a custom form](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

   >[!NOTE]
   >
   >These features are available for organizations on all Workfront and Workflow packages.

* The ability to add custom forms to teams, rate cards, and job roles
   For more information, see [Create a custom form](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

   >[!NOTE]
   >
   >* Adding custom forms to rate cards and job roles requires the Workflow Ultimate package.
   >* Adding custom forms to teams is available for organizations on all Workfront and Workflow packages.

* A **Finance permission type** setting on currency-formatted fields, to allow access only to users who have certain permissions set in their access levels
   For more information, see [Restrict access to financial data in custom fields](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/restrict-access-to-financial-data.md).

   >[!NOTE]
   >
   >This feature is available for organizations on all Workfront and Workflow packages.

### Layout template enhancements

>[!NOTE]
>
>These features are available for organizations on all Workfront and Workflow packages.


In layout templates, you can customize the headers and left navigation menus of additional objects, and display and hide items more easily in the Main Menu. You can also use a layout template to determine the options that appear when a user clicks the **More** menu (the three-dot menu) on projects, tasks, issues, portfolios, and programs.

For more information, see [Create and manage layout templates](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).

### Custom localization

>[!NOTE]
>
>This feature is only available for organizations on the Workflow Prime or Ultimate packages.

Custom localization allows you to define custom terms and phrases in different languages. Workfront then displays these terms in the language set in the browser settings.
For example, you can set the label "Target Audience" to translate to the German word "Zielgruppe." Any user with German set as the language for their Adobe IMS account sees the word "Zielgruppe" as a label for any fields labeled "Target Audience" in English.

For more information, see [Configure custom localization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/configure-custom-localization.md).

### Automate actions with Business Rules

>[!NOTE]
>
>These features are only available for organizations on the Workflow Ultimate package.

Workfront administrators can now configure business rules to automate actions for the created, edited, or modified object when certain conditions are met. Available actions include sharing the object, or attaching a custom form to the object.

For more information, see [Create and edit business rules](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/business-rules.md).


