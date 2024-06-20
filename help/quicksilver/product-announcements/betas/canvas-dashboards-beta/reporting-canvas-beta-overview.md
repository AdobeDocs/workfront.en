---
content-type: reference
navigation-topic: betas
title: 'Reporting Canvas beta: overview'
description: Information on the beta program for the upcoming Reporting Canvas tool for Adobe Workfront
author: Nolan
feature: Product Announcements
hidefromtoc: yes
hide: yes
exl-id: 5767ef7d-1bc3-40d8-abeb-02b15166a0a3
---
# Reporting Canvas beta: overview

## Reporting Canvas

A complete reimagination of reporting in Workfront, the new Reporting Canvas tool is currently in development. In designing Reporting Canvas, we have worked hard to provide an experience that offers maximal flexibility coupled with an intuitive, modular design—so that users like you can most effectively leverage your own data in making and sharing reports. Through a new, unified report type that allows you to drag-and-drop nearly every element onto a limitless canvas, creating a visual data masterpiece will soon be easier than ever before.

This article contains information about the current private beta, which is limited to specific customers. New Reporting Canvas features are now being deployed through Canvas Dashboards. See **Development plan** below for more information.

### Development plan

We are in the final stages of resolving a data quality issue we observed early in the Reporting Canvas beta. We will soon resume work to provide new visualizations, expand the selection of reportable Workfront objects, and improve the report creation and distribution experiences, all of which are integral to realizing our goals for Reporting Canvas.

We will deliver these new experiences incrementally, beginning with the 23.2 release, through the new Canvas Dashboards page that is now available in your Preview environment. Canvas Dashboards allow you to display existing reports alongside the new reporting capabilities we are building, and will serve as our primary environment for deploying and testing new features for Reporting Canvas. For more information on enabling and using Canvas Dashboards, see [Canvas Dashboards overview](/help/quicksilver/reports-and-dashboards/dashboards/creating-and-managing-dashboards/canvas-dashboards-overview.md).

## Participate in the beta

>[!IMPORTANT]
>
>The beta information below is for administrators that have already been included in the Reporting Canvas beta, which is no longer accepting new participants. If you would like to test new features of Reporting Canvas as they are added, see **Development plan** above for information on enabling Canvas Dashboards.

### Availability

The Reporting Canvas beta is available to all organizations that are on AWS, regardless of region.

### Join the beta

The Reporting Canvas beta is completely optional, but may only be opted into by a Workfront administrator. To opt in as a System Administrator:

1. Select the **Reporting (beta)** icon in the Main menu of your Workfront instance.
1. Click **Accept** to accept the terms and conditions.
1. Allow your organization's data to be added to Reporting Canvas (this may take up to a few hours).
1. Start using Reporting Canvas.

After your organization's data is added to Reporting Canvas, other system administrators can choose to join on an individual basis in the same way (without waiting for data to be added again).

To opt in other users that are not Workfront administrators:

1. Select the **Reporting (beta)** icon in the Main menu of your Workfront instance.
1. Click on **Reporting Canvas permissions**.
1. Search for and select the specific users you want to participate.

   >[!IMPORTANT]
   >
   >Users that you grant access to Reporting Canvas will have access to **all** data in the system in a read-only capacity, regardless of their standard permissions to view this data.

1. Click **Save**.
1. Add the **Reporting (beta)** icon into the main layout template of each user that was selected. For more information, see [Customize the Main Menu using a layout template](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-main-menu.md).
1. Each user must then individually navigate to the **Reporting (beta)** icon in their main menu and accept the terms and conditions.

### Submit feedback

To submit feedback about the beta:

1. While in Reporting Canvas in Workfront, click the **Send Feedback** button.
1. Fill out the form, then click **Submit**.

## Beta FAQ

+++Can I migrate my legacy reports to Reporting Canvas?

In short, migrating legacy reports won't be available during the beta. However, it is a planned feature (with some caveats described below) for the official launch.

While the barrier to building new reports has been significantly lowered with Reporting Canvas, we understand that bringing over some of your existing reports and dashboards will help accelerate the adoption process. As such, we want to provide the tools and resources necessary to make sure you can bring over any relevant legacy items to ensure you start off on the right foot in Reporting Canvas. Since Reporting Canvas is such a radical change to the way current reporting works, however, it would be impossible to migrate every report or dashboard exactly as it is today.

Our current strategy for migration in the official releaseis to enable you to do the following:

1. Identify the reports and dashboards that are relevant

   1. Give you the ability to export a CSV of all the reports and dashboards in the system along with any relevant tracking information (number of views, when, and by whom).
   1. Provide an export of reports that are set up with scheduled deliveries along with the recipients.

1. Select the reports and dashboards that you want to migrate, then click **Migrate**

   This is a one-way migration. It creates a copy of the selected reports and dashboards to Reporting Canvas, leaving the legacy report or dashboard intact in the current reporting tool.

   You can migrate the same report or dashboard as many times as you want.

1. In Reporting Canvas, make sure that all of the reports and dashboards you selected were migrated.
+++

+++Why can't I see all the objects I normally do?

In order to provide the beta to our customers as early as possible, we have released it with only a subset of the many object types available in Workfront today. Below are the object types currently supported in the beta:

* Assignment
* Document
* Document Approval
* Expense
* Hour
* Issue
* Note
* Portfolio
* Project
* Program
* Task
* Timesheet
* Work Item
+++

+++If something goes wrong in Reporting Canvas during the beta, will my organization's data be impacted?

No. The beta uses a copy of your organization's data that is populated into Reporting Canvas. While this means that you are safe to experiment during the beta without risk of impacting important data, it also means that in-line editing of data in Reporting Canvas will be unavailable until the official launch.
+++

+++Can I opt out of the beta once I've joined?

A Workfront administrator cannot opt out of the beta; however, non-system administrators can be removed by doing the following:

1. Log in as a System administrator.
1. Navigate to Reporting Canvas.
1. Click Reporting Canvas **permissions**.
1. Remove the users you want to opt out of the beta from the list that have been opted in.
1. Click **Save**.
+++
