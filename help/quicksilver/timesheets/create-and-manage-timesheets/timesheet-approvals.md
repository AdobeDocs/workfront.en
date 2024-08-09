---
product-area: timesheets
navigation-topic: create-and-manage-timesheets
title: Approve a timesheet
description: The process of approving timesheets provides managers with visibility into the work hours of their direct reports. Approvers can verify that all time recorded has been allocated in the correct areas and that a sufficient number of hours have been recorded for the period.
author: Alina
feature: Timesheets
exl-id: b27b3307-f61b-456d-8076-590d1c391b4b
---
# Approve a timesheet

<!--Audited: 8/2024-->

The process of approving timesheets provides managers with visibility into the work hours of their direct reports. Approvers can verify that all time recorded has been allocated in the correct areas and that a sufficient number of hours have been recorded for the period.

Adobe Workfront provides the ability to configure timesheet approvals to support in this area.

For information on submitting a timesheet, see [Submit a timesheet for approval](../../timesheets/create-and-manage-timesheets/submit-timesheet-for-approval.md).

## Access requirements

+++ Expand to view access requirements for the functionality in this article. 

You must have the following access to perform the steps in this article:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront plan</p></td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront license*</p></td> 
   <td> <p>New: Standard</p>
   <p>Current: Plan </p> 
   <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>Administrative access to Timesheets & hours </p> </td> 
  </tr> 
   
   </td> 
  </tr> 
 </tbody> 
</table>

*For information, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).   

+++

## Designate timesheet approvers

Typically, timesheets are approved by functional managers or human resources personnel. Timesheets are not usually approved by project managers. Project managers may approve time logged on projects, but team or human resource managers should approve timesheets. 

A timesheet approver is defined when creating the Timesheet Profile. You must have a Plan license to be designated as an approver.

For more information about designating timesheet approvers, see the section [Create or edit a timesheet profile](../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md#create) in the article [Create, edit, and assign timesheet profiles](../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md).

## Approve a timesheet

You can approve any timesheets that have been submitted where you have been designated as an approver. When a timesheet is submitted for approval, the timesheet is listed in the **Approvals** area on your **Home**  page. For more information, see [Approving work](../../review-and-approve-work/manage-approvals/approving-work.md).

If the Workfront administrator has enabled the Timesheet Approval to User and the Timesheet Rejection to User event handlers, you are notified after the timesheet is approved or rejected. For information about enabling event notifications, see [Event notification types](../../administration-and-setup/manage-workfront/emails/event-notifications-available-in-wf.md).

To approve a timesheet:

{{step1-to-timesheets}}
   
   The **Timesheets** area opens. 

1. Select the **My Timesheet Approvals** in the upper-right corner of the page to view only timesheets that you approve

   Or

   Select the **My Timesheet Approvals** filter at the top of the timesheet list.

   ![](assets/my-timesheet-approvals-my-timesheets-pills-on-timesheets-list-nwe-350x58.png)

   >[!NOTE]
   >
   >The My Timesheet Approvals option does not display at the top of the timesheet list or in the list of filters if your Workfront administrator or a group administrator removed the My Timesheet Approvals filter from either the List Controls in the Setup area or from your Layout Template. For more information see the following articles:
   >
   >   
   >   
   >   * [Customize Filters, Views, and Groupings using a layout template](../../administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md) 
   >   
   >

1. (Optional) Click the **search** icon ![](assets/search-icon.png) at the top of the timesheet list and type a keyword to locate a specific timesheet. You can search for a time frame, or an owner or approver's name. 
1. Click the time frame for the timesheet you want to approve. The timesheet opens. 

   >[!TIP]
   >
   >Timesheets awaiting approval have a status of [!UICONTROL Submitted].


1. Click **Approve**

   Or

   If you want to reject the timesheet, click **Reject** in the lower-left corner of the timesheet.

   If approved, the timesheet status changes to **Closed**.

   If rejected, the timesheet status changes to **Rejected**.
