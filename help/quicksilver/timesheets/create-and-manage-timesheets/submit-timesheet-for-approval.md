---
product-area: timesheets
navigation-topic: create-and-manage-timesheets
title: Submit a Timesheet for Approval
description: Submitting your timesheet for approval provides your manager with visibility into your work hours. Approvers can verify that all time recorded has been allocated in the correct areas and that a sufficient number of hours have been recorded for the time period.
author: Lisa
feature: Timesheets
exl-id: 253e20c8-58f8-4b23-a769-b0e36557066a
TQID: https://experienceleague.adobe.com/uxfkWowkcyC9zeX1vNaZaY-i3AFCHMngvflZ8-REnac
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
    internal-label: Administration
subfeature_v2:
  - id: b04e3dc0-3a59-45b1-aa02-b0b6d5f87eff
    internal-label: Approvals
  - id: ce22a157-dd2c-405f-b740-c2f204bb4c1a
    internal-label: Timesheets
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
    internal-label: Reporting
  - id: bce87dde-a4ab-44c9-8a18-ad66e4ddb377
    internal-label: Customer experience
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
---
# Submit a timesheet for approval

<!--Audited: 8/2024-->

Submitting your timesheet for approval provides your manager with visibility into your work hours. Approvers can verify that all time recorded has been allocated in the correct areas and that a sufficient number of hours have been recorded for the time period.

## Access requirements

+++ Expand to view access requirements for the functionality in this article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront package</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront license</td> 
   <td> <p>Light or higher </p>
   <p>Review or higher </p>
  </tr> 
  <tr> 
   <td>Access level configurations</td> 
   <td> <p>View or higher access to tasks and issues </p> </td> 
  </tr> 
  <tr> 
   <td>Object permissions</td> 
   <td> <p>View or higher permissions to the timesheet</p> </td> 
  </tr> 
 </tbody> 
</table>

For information, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Submit a timesheet for approval

* [Submit a timesheet for approval](#submit-a-timesheet-for-approval) 
* [View the status of a submitted timesheet](#view-the-status-of-a-submitted-timesheet)

### Submit a timesheet for approval

After a timesheet approver is set (as described in the section [Designate timesheet approvers](../../timesheets/create-and-manage-timesheets/timesheet-approvals.md#designating-a-timesheet-approver) in the article [Approve a timesheet](../../timesheets/create-and-manage-timesheets/timesheet-approvals.md)), the **Close** button at the bottom of the timesheet changes to a **Submit for approval** button.

To submit a timesheet for approval:

1. Go to a timesheet that has been configured to have an approver.
1. Log time, as described in [Log time](../../timesheets/create-and-manage-timesheets/log-time.md).
1. Click **Submit for approval** to launch the timesheet approval process.

   ![Submit for approval button](assets/submit-for-approval-button-on-timesheet.png)

   The **Submit for approval** button is replaced by the **Approve**, **Reject**, and **Recall** buttons. The status of the timesheet changes to **Submitted**.

   When your timesheet is submitted for approval, the approver sees the timesheet listed in the **My Approvals** widget in the **Home** area. The following things might occur:

   * If they approve it, the **Recall** button changes to **Re-open** and the timesheet status updates to **Open**.
   * If they reject it, the **Submit for approval** button replaces the **Recall** button and the timesheet status updates to **Rejected**.

1. (Optional) Click **Recall** if you need to reopen the timesheet and update your time. For information, see the [Recall a timesheet](#recall-a-timesheet) section in this article.

### View the status of a submitted timesheet {#view-the-status-of-a-submitted-timesheet}

You can view the status of a timesheet after you submit it.

If the Workfront administrator has enabled the Timesheet Approval to User and the Timesheet Rejection to User event handlers, you are notified after the timesheet is approved or rejected. For information about enabling event notifications, see [Event notification types](../../administration-and-setup/manage-workfront/emails/event-notifications-available-in-wf.md).

Without these notifications, you can learn about the status of your submitted timesheets in the Timesheet area of Workfront.

To view the status of a timesheet:

{{step1-to-timesheets}}

   All timesheets that you have access to view are displayed by default.

   ![Timesheets list](assets/list-of-all-timesheets.png)

1. (Optional) Do one of the following to update the filter in the list of timesheets:

   * Select **My Timesheet Approvals** in the upper-right corner of the page to view only timesheets that you approve,

     Or

     Select **My Timesheets** to view only your timesheets.

     This applies the **My Timesheet Approvals** or the **My Timesheet** filters to the list of timesheets.

   * Click the **Filter** icon ![Filter icon](assets/filter-nwepng.png) to apply a filter or create a new filter. For information about creating or updating filters, see [Create or edit filters in Adobe Workfront](../../reports-and-dashboards/reports/reporting-elements/create-filters.md).

   >[!NOTE]
   >
   >The My Timesheet Approvals and My Timesheets options do not display at the top of the timesheet list or in the list of filters if your Workfront administrator or a group administrator removed those filters from either the List Controls in the Setup area or from your Layout Template. For more information, see [Customize Filters, Views, and Groupings using a layout template](../../administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md).

1. (Conditional) If you selected **My Timesheets**, ensure that the **Standard** view is applied and notice the **Status** column.

   Timesheets can have the following statuses:

   | Status | Description |
   | --------- | ---------- |
   | Open | <p>Your timesheet is currently open and you may log time.</p><p>A recalled timesheet displays with a status of Open. For information, see the [Recall a timesheet](#recall-a-timesheet) section in this article.</p> |
   | Submitted | You submitted your timesheet for approval but it has not been approved yet. You may recall a submitted timesheet to continue editing it. For information, see the [Recall a timesheet](#recall-a-timesheet) section in this article. |
   | Closed | <p>The following scenarios exist:</p><ul><li>If the timesheet has no approver, you saved your time and closed it.</li><li>If the timesheet has an approver, you have submitted it for approval and it has been approved.</li></ul> |
   | Rejected | You submitted the timesheet for approval and the approver rejected it. |

## Recall a timesheet {#recall-a-timesheet}

You can recall a timesheet that has already been submitted for approval. Only timesheets that haven't been approved can be recalled.

To recall a timesheet:

{{step1-to-timesheets}}

1. Click **My Timesheets** in the upper-right corner of the screen, or select **My Timesheets** from the **Filter** ![Filter icon](assets/filter-nwepng.png) drop-down menu.
1. Click the time frame for a timesheet with a status of **Submitted**.
1. Click **Recall**.

   The timesheet becomes editable again and its status changes to **Open**.
