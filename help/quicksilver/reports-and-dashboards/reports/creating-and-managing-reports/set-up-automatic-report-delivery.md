---
product-area: reporting;setup
navigation-topic: create-and-manage-reports
title: Schedule an automatic report delivery
description: Schedule an automatic report delivery
author: Courtney
feature: Reports and Dashboards
exl-id: 5b8e382c-bfe8-43aa-aa09-a2aa0c4d56cc
---
# Schedule an automatic report delivery

<!-- Audited: 4/2025 -->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: If this stays, fix links which now go to the reference article)</p>
-->

You can schedule reports to automatically deliver to users on a defined schedule, or you can manually send reports on a one-time basis. When you send a report from Adobe Workfront, the user receives an email with the Workfront report in a separate attachment.

For more information, including size limitations that can affect the delivery of your reports, see [Report delivery overview](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md).

## Access requirements

+++ Expand to view access requirements for the functionality in this article. 

You must have the following access to perform the steps in this article:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license</td> 
      <td> 
      <p>New: Standard</p>
      <p>Or</p>

   <p>Current: Plan</p>
       
   </td>
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>Edit access to&nbsp;Reports,&nbsp;Dashboards,&nbsp;Calendars</p> <p>Edit access to Filters,&nbsp;Views, Groupings</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to a report</p></td> 
  </tr> 
 </tbody> 
</table>

For more detail about the information in this table, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md). 

+++

## Prerequisites

Before you begin, you must create a report. To learn more about creating reports, see [Create a custom report](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

## Schedule a report delivery


To schedule a report for automatic delivery:​

{{step1-to-reports}}

   >[!NOTE]
   >
   >Report deliveries do not contain prompts. If you wish to limit data in a report delivery, we recommend applying filters to the report that you want to send.

1. On the **Reports** page, select a report.
1. At the top of the screen, click **Report Actions**, then **Send Report** from the drop-down that appears. The **Send Report** dialog box displays.

   >[!TIP]
   >
   >To send a report manually at any given time, go to the report, then click **Report Actions** > **Send Report** > **Send Now**.

1. Select the **Repeating Deliveries** tab.
1. (Conditional) To modify an existing repeating report delivery, select the report delivery in the **Repeating Deliveries** section on the right side of the dialog box.
1. Specify the following information:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p>Send to</p> </td> 
      <td> <p>Begin typing the name of the user, group, team, or role who you want to send the report to, then click the name when it appears in the drop-down list.</p> <p>Or</p> <p>Enter the email address of a person external to the Workfront system who you want to have access to the report.</p> <p>Repeat this process to send the report to multiple users, groups, teams, or roles.</p> <p>Note:  <p>Consider the following when adding report delivery recipients:</p> 
        <ul> 
         <li><p>If your organization restricts Workfront notifications to specific email domains, you may only be able to send reports to email addresses listed in the email allowlist.</p> <p>For example, when a user is set as a report recipient and has an email address that was previously permitted, and the allowlist is updated to no longer deliver emails to that domain, the user will no longer receive delivered reports.</p><p>For information on how a Workfront administrator updates the email allowlist, see the section <a href="../../../administration-and-setup/get-started-wf-administration/configure-your-email-allowlist.md#configur" class="MCXref xref">Configure your email allowlist</a>.</p></li> 
         <li> <p>Adding a large number of users as recipients can cause the delivery to fail. If you experience delivery failures, you can schedule multiple report deliveries with smaller groups of users.</p> </li> 
        </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Email Subject</p> </td> 
      <td> <p>Enter a subject for the email notification.</p> <p>By default, the email subject is:</p> <p><em>Workfront Report: [Name of the report] [Date]</em> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Email Message</p> </td> 
      <td> <p>Enter a message to include in the email.</p> <p>By default, the email message is:</p> <p><em>Attached is the [report frequency] report [Name of the report] generated by Workfront on [Date].</em> </p> <p>Note: For reports delivered as an Excel file only, the following message is also added to the email: "Please be aware that with MS Excel (XLS) file types, there is a limit (65,530) on the number of hyperlinks these file types support. If you exceed those limits, your file will not open and it is recommended to resend without the hyperlinks. Please go back to the report scheduler to remove hyperlinks and resend the report." The "please go back to the report scheduler" phrase is a link back to the report.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Deliver this report with the Access Rights of</p> </td> 
      <td> <p>Begin typing the name of a user who has access to the report, then click the name when it appears in the drop-down list. Users who receive the report will be granted the same level of access to the report as the user that you specify here.<br> For more information, see <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/run-deliver-report-access-rights-another-user.md" class="MCXref xref">Run and deliver a report with the access rights of another user</a>.</p> <p>Note: This field does not support wildcards. For example, using the wildcard <em>$$User.ID</em> does not run the report with the access rights of the user who is receiving the report.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Format</p> </td> 
      <td> <p>Select the format you want for the delivered report:</p> 
       <ul> 
        <li> <p>HTML</p> </li> 
        <li> <p>PDF</p> <p>If you select PDF, you can format the output using the additional <strong>Paper Size</strong> and <strong>Orientation</strong> options that display.</p> </li> 
        <li> <p>MS Excel (.xlsx)</p> </li> 
        <li> <p>TSV</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Include Links</p> </td> 
      <td> <p>This option is available only when <strong>MS Excel</strong> is selected in the <strong>Format</strong> drop-down menu. When this option is enabled, any hyperlinks are included in the exported Excel document.</p> <p>Documents that contain more than 65,530 links cannot be opened. If the exported document will contain more than 65,530 links, deselect this option.</p> <p>This option is enabled by default.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Summary</p> </td> 
      <td> <p>Displays a summary of when the delivery repeats.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Repeats</p> </td> 
      <td> <p>Select whether the report should be delivered daily, weekly, monthly, or yearly.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Repeats Every</p> </td> 
      <td> <p>Select the frequency with which you want the delivery to repeat. The value you select for this option is based on the option that is selected in the <strong>Repeats</strong> drop-down list.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Time</p> </td> 
      <td> <p>Select the time of day for the delivery to be sent.</p> <p>Tip: Because system loads can affect report delivery times, there may be a delay of up to 24 hours between the scheduled time and the actual delivery time. If you need a report delivered by a specific time, we recommend scheduling the delivery prior to the time that it is needed. In general, we recommend scheduling the delivery at least a day prior to the date when it is needed.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Repeats On</p> </td> 
      <td> <p>This option is available when the <strong>Repeats</strong> option is set to either <strong>Weekly</strong> or <strong>Monthly</strong>:</p> 
       <ul> 
        <li> <p>When the <strong>Repeats</strong> option is set to <strong>Weekly</strong>: Select the days of the week that the delivery is sent.</p> </li> 
        <li> <p>When the <strong>Repeats</strong> option is set to <strong>Monthly</strong>: Select whether the delivery is sent on the day of the month, day of the week, or last day of the month (these options leverage the date that you select in the <strong>Starts On</strong> field).</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Starts On</p> </td> 
      <td>Select the date for the scheduled delivery to begin.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Ends On</p> </td> 
      <td>Select a date for the scheduled delivery to end.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Never</p> </td> 
      <td>Select <strong>Never</strong> if you want the scheduled delivery to last indefinitely.</td> 
     </tr> 
    </tbody> 
   </table>

1. Click **Save** to save the report delivery. The report displays in the **Repeating Deliveries** section of the **Send Report** dialog box and will send at the scheduled time.

   For information about size limitations that can affect the delivery of your reports, see the sections [Report delivery limits](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md#understanding-export-limits) and [Export limits](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md#export).

>[!IMPORTANT]
>
>Scheduled reports are subject to an internal time limit when being processed for delivery. In the event a report takes longer than the limit to be sent, you will receive a notification and the report will no longer be delivered regardless of any remaining scheduled deliveries. To continue sending the report, first try reducing the size of the report through filters and views, then create a new scheduled delivery.
>
>If you are using a scheduled report delivery to analyze Workfront data through a BI tool, we recommend using Workfront Data Connect instead. For more information, see [Workfront Data Connect overview](/help/quicksilver/reports-and-dashboards/data-lake/data-lake-overview.md).

## Delete a scheduled report delivery

To delete a scheduled report delivery:​

{{step1-to-reports}}

1. On the **Reports** page, select a report.

1. At the top of the screen, click **Report Actions**, then **Send Report** from the drop-down that appears. The **Send Report** dialog box displays.

1. Select the **Repeating Deliveries** tab.
1. In the **Repeating Deliveries** section on the right side of the dialog box, click the scheduled delivery you want to delete.
1. In the **Repeating Deliveries** detail section, click **Delete**.

1. Click **Delete** to confirm.

<!--## Video walk-through

View the following video to learn how to schedule a report delivery. This video was recorded in Workfront Classic. However, the content also applies to the new Workfront experience.

[ ![Video walkthrough of report delivery](assets/video-walk-through--350x197.png)](https://workfront-video.wistia.com/medias/45jffmll62)


<h2 data-mc-conditions="QuicksilverOrClassic.Draft mode">Additional information</h2>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">See also:</p>
-->

  <!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><a href="https://one.workfront.com/s/learningpath2/workfront-reporting-20Y0z000000blhLEAQ" target="_blank">Learning Path for reports and dashboards</a> </li>
  -->

  <!--
  <p data-mc-conditions="QuicksilverOrClassic.Draft mode"><a href="https://one.workfront.com/s/basic-report-creation-program">Basic Report Creation Program for the new Workfront experience</a> </p>
  -->
