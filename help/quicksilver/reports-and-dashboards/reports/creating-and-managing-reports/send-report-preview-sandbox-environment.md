---
product-area: reporting
navigation-topic: create-and-manage-reports
title: Send a report in the Preview Sandbox environment
description: The information on this page refers to functionality that is available only in the Preview and Custom Refresh Sandbox environments. This functionality is not available in the Production environment.
author: Nolan
feature: Reports and Dashboards
exl-id: 568360df-bec9-4767-8b5a-32a294d05d47
---
# Send a report in the Preview Sandbox environment

The information on this page refers to functionality that is available only in the Preview and Custom Refresh Sandbox environments. This functionality is not available in the Production environment.

You can set up Report Delivery options in any Adobe Workfront test environment.

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">For information about the Workfront test environments, see the "Workfront Testing Environments" section. (NOTE:&nbsp;drafted - link this section)</p>
-->

While the test environments are meant to function as close as possible to your production environment, some functionality differs from your production environment.

You can schedule reports in the test environments, but the way they are delivered differs from how they are delivered from the Production environment.

For information about scheduling reports for delivery in the Production environment, see [Report delivery overview](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md).

Depending on where you schedule the reports, the delivery functionality differs between the Preview and the Custom Refresh sandboxes.

## Access requirements

You must have the following access to perform the steps in this article:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to&nbsp;Reports,&nbsp;Dashboards,&nbsp;Calendars</p> <p>Edit access to Filters,&nbsp;Views, Groupings</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to a report</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your Workfront administrator.

## Schedule reports in the Preview environment

* [Schedule reports in the Preview environment](#schedule-reports-in-the-preview-environment)

### Schedule reports in the Preview environment

Whether a delivered report is produced or not in the Preview environment depends on whether **Receive emails from this test environment** is enabled or not.

For information about enabling emails from the Sandbox environment see [Enable delivery of emails from the Preview Sandbox environment](../../../workfront-basics/using-notifications/enable-delivery-emails-from-preview-sandbox-environment.md).

![](assets/receive-emails-from-sandbox-setting-edit-350x223.png)

Scheduling reports for delivery in the Preview environment is identical to scheduling reports in the Production environment. For information about scheduling a report for delivery, see [Report delivery overview](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md).

When you schedule a report for delivery in the Preview environment, the following scenarios exist:

* When **Receive emails from this test environment** is disabled for the user who is receiving the report, no file is produced when scheduling the report for delivery.
* When **Receive emails from this test environment** is enabled for the user who is receiving the report, the file that is produced when scheduling the report for delivery is added in the Documents tab of the user.

## Schedule reports in the Custom Refresh Sandbox environment

Whether a delivered report is produced or not in the Custom Refresh Sandbox depends on whether the Receive emails from this test environment setting is enabled or not.

For information about enabling emails from the Preview environment see the section [View and modify your email notification settings](../../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md#view) in the article [Modify your own email notifications](../../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

![](assets/receive-emails-from-sandbox-setting-edit-350x223.png)

Scheduling reports for delivery in the Custom Refresh Sandbox environment is identical to scheduling reports in the Production environment. For information about scheduling a report for delivery, see [Report delivery overview](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md).

When you schedule a report for delivery in the Custom Refresh Sandbox environment, the following scenarios exist:

* When the Receive emails from this test environment is disabled for the user who is receiving the report, no file is produced when scheduling the report for delivery.
* When the Receive emails from this test environment is enabled for the user who is receiving the report, the report is emailed as an attachment to the email address associated with the user.

## How external users are notified

External users do not receive reports sent from the Workfront test environments, nor do they receive an email notification.

External users only receive emailed reports if they are delivered from a Production environment.
