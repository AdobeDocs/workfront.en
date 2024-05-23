---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Currently available Adobe Workfront Fusion templates
description: The following public templates are currently available in Adobe Workfront Fusion.
author: Becky
feature: Workfront Fusion
exl-id: 29d95b93-ab54-416d-b0d5-ff12634951b2
---
# Currently available Adobe Workfront Fusion templates

The following public templates are currently available in Adobe Workfront Fusion.

Your team or organization may have other team-created templates available. 

To view available templates, click the **Templates** icon ![](assets/fusion-template-icon.png) in the side navigation menu in Fusion.

## Workfront templates

These templates automate Workfront processes and workflows.

### Workfront - Project Creation from CSV

This automation creates new projects in Workfront based off Name, Portfolio, Status, Planned Start Date, and Template details that you specify in a CSV.

### Workfront - Cleanup Requests with no new notes in past 30 days

Use this template to enforce a 30 day note update on your requests. Requests not updated in 30 days get their status changed and closed at 60 days.

### Workfront - Change project Status to Complete at 100% complete.

This automation updates projects to Complete status that have all tasks at 1005 complete. Projects with open issues or open tasks or project approvals will receive an update, and when resolved, the projects will move to Complete status.

### Workfront - Warn and attempt to close stale projects

Use this scenario to help automate the warning on and closure of projects that meet your organization's stale project policy.

### Workfront - Copy new notes and replies from source issue/request to already converted project or task

Use this template to copy notes and replies from an issue or request to an already converted project or task.

### Workfront - Copy Program Custom Forms and Field Data to Associated New Projects

This automation watches for new projects in programs with custom forms. It then adds those program custom forms and fields to the new projects.

### Workfront - Copy Portfolio Custom Forms and Field Data to Associated New Projects

This automation watches for new projects in portfolios with custom forms. It then adds those portfolio custom forms and fields to the new projects.

### Workfront - Convert approved issue to project

This template converts Issues to Projects. You can modify it to meet your organization's standards.

### Workfront - Copy documents from issues/requests to already converted projects or tasks

This flexible scenario copies documents from issues or requests to previously converted projects or tasks.

### Tailored Notification Based on Field Change

This template creates tailored updates (and related notifications) to individuals working on a Workfront project, based upon some unique event such as a change in a field value. The scenario watches Workfront for when a specified field changes in a Task or Issue. When encountered, the scenario will evaluate information in the related project and create a tailored update for a person assigned to a specific role on the project.

### Workfront - Bulk append to project name with convention

This bulk update template renames all projects that meet the criteria of a search (fall within a portfolio) and rename them with a standard format.

### Workfront - Rename projects with convention

This template locates all projects that meet the criteria of a filter (fall within a portfolio), and renames them with a standard format.

### Workfront - Create Baseline on Status Change

This template captures a project baseline upon any project status change noted in the "switch" modules, and creates an update in the update stream for logging.

### Workfront - Baseline creation on weekly basis

This template captures a project baseline on a weekly basis every Monday at 6am ET on projects filtered by portfolio, and creates an update in the update stream for logging.

### Find project templates not used in policy time and notify

Once a month, review your project templates using your own policy with this easy to manage template that notifies appropriate users on templates in violation of your policy.

## Workfront - Workfront Proof templates

These templates automate workflows that combine Workfront with Workfront Proof.

### Workfront Proof > Workfront - Project Update on Proof Decision

When a decision is made on a Proof that is added directly to a project, this automation gathers information on the Proof Decision, such as who made the Decision, and then reflects this progress in the corresponding Workfront Project as an update.

### Workfront Proof > Workfront - Task Update and Completion (if Approved) on Proof Decision

Where individual proofs are tied to individual tasks, this scenario closes the associated task when an approval decision on the proof is made. If approved, it completes the task and updates the project.

## HTTP - Workfront templates

These templates retrieve information from a web service, and bring that information into Workfront.

>[!NOTE]
>
> You must have a Workfront Fusion for Work Automation and Integration license to use templates in this section.

### Establishing Connection using JWT (JSON Web Token)

Establish JWT Authorization for a client API.

### APILayer > Workfront - Daily Exchange Rate Update (EUR)

This template creates a scenario that automates the updating of an exchange rate at a set point in time. This scenario pulls the rate of Euros (EUR) to US Dollars (USD) from an APIlayers.com API and updates the rate in Workfront.

## Workfront-Marketo templates

These templates support Workfront-Marketo integration. 

>[!NOTE]
>
> You must have a Workfront Fusion for Work Automation and Integration license to use templates in this section.

### Approve your Marketo Engage email draft with Workfront approval workflows

This is part of the Review and Approve integration between Workfront and Marketo Engage. This template detects if an email Proof in Workfront has been approved, and then updates the corresponding email in Marketo Engage as approved.

### Intake marketing campaign requests in Workfront and automate the creation of campaigns in Marketo Engage

This scenario provides a programmatic way to create email and webinar campaigns in Marketo Engage from a request made in Workfront. By using automation to create, organize, and configure campaigns, teams are able to improve efficiency.

### Review an email proof of your Marketo Engage email draft in Workfront

This template detects if a Workfront task has been set to a ready for review status, and then exports the email draft from Marketo Engage to save it as a Proof in Workfront.

## Workfront-SharePoint templates

These templates connect Workfront and SharePoint. 

>[!NOTE]
>
> You must have a Workfront Fusion for Work Automation and Integration license to use templates in this section.

### Watch SharePoint Folder Changes

This template allows you to see if there is a change in a SharePoint folder.


## Workfront-Anaplan templates

These templates support the Workfront-Anaplan integration, and expect a specific configuration in both Anaplan in Workfront. For information on these templates and their required configurations, see the articles for the individual templates.

For more information on the Workfront-Anaplan integration, see [Adobe Workfront with Anaplan](../../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/anaplan-integration.md).

>[!NOTE]
>
> You must have a Workfront Fusion for Work Automation and Integration license to use templates in this section.

### Spend optimization workflows

* [Send [!DNL Adobe Workfront] project updates to an [!DNL Anaplan] list item](../../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-actual-hours-updates-to-anaplan-list-item.md)
* [Send [!DNL Adobe Workfront] expenses to an [!DNL Anaplan] list item](../../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-expenses-to-anaplan-list-item.md)
* [Send [!DNL Adobe Workfront] actual hours updates to an an [!DNL Anaplan] list item](../../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-actual-hours-updates-to-anaplan-list-item.md)

### Workflows for linking budget requests

* [Create an [!DNL Anaplan] list item from an [!DNL Adobe Workfront] budget request](../../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/create-an-anaplan-list-item-from-a-workfront-budget-request.md)
* [Apply an [!DNL Anaplan] budget allocation to an [!DNL Adobe Workfront] project](../../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/apply-anaplan-budget-allocation-to-workfront-projects.md)

### Workflows for linking campaign requests

* [Create an [!DNL Anaplan] list item from an [!DNL Adobe Workfront] campaign request](../../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/create-an-anaplan-list-item-from-a-workfront-campaign-request.md)
* [Apply an [!DNL Anaplan] budget allocation to an [!DNL Adobe Workfront] campaign request or campaign project](../../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/apply-anaplan-budget-allocation-to-workfront-campaign-requests-and-projects.md)


<!--[!BADGE New!]{type=Informative} -->