---
filename: set-up-automatic-report-delivery
product-area: reporting;setup
navigation-topic: create-and-manage-reports
---



# Schedule an automatic report delivery {#schedule-an-automatic-report-delivery}

You can schedule reports to automatically deliver to users on a defined schedule, or you can manually send reports on a one-time basis. When you send a report from *`Adobe Workfront`*, the user receives an email with the *`Workfront`* report in a separate attachment.


For more information, including size limitations that can affect the delivery of your reports, see [Report delivery overview](set-up-report-deliveries.md).



## Access requirements {#access-requirements}

You must have the following access to perform the steps in this article:

<table style="width: 100%;margin-left: 0;margin-right: auto;mc-table-style: url('../../../Resources/TableStyles/TableStyle-List-options-in-steps.css');" class="TableStyle-TableStyle-List-options-in-steps" cellspacing="0"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2"> 
 <tbody> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader"><span class="mc-variable WFVariables.FullProdNameWF variable varname">Adobe Workfront</span> plan*</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p>Any</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader"><span class="mc-variable WFVariables.FullProdNameWF variable varname">Adobe Workfront</span> license*</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray"> <p><span class="mc-variable WFVariables.WFLicense-Plan variable varname">Plan</span> </p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader">Access level configurations*</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p>Edit access to&nbsp;Reports,&nbsp;Dashboards,&nbsp;Calendars</p> <p>Edit access to Filters,&nbsp;Views, Groupings</p> <p>Note: If you still don't have access, ask your <span class="mc-variable WFVariables.AdminWF variable varname">Workfront administrator</span> if they set additional restrictions in your access level. For information on how a <span class="mc-variable WFVariables.AdminWF variable varname">Workfront administrator</span> can modify your access level, see <a href="create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-MediumGray" role="rowheader">Object permissions</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-MediumGray"> <p>Manage permissions to a report</p> <p>For information on requesting additional access, see <a href="request-access.md" class="MCXref xref">Request access to objects in Adobe Workfront</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your *`Workfront administrator`*.


## Prerequisites {#prerequisites}

Before you begin, you must create a report. To learn more about creating reports, see [Create a custom report](create-custom-report.md).


## Schedule a report delivery {#schedule-a-report-delivery}

To schedule a report for automatic delivery or to edit or delete an existing report delivery:​



1.  Go to a report that you want to schedule for delivery.


   >[!NOTE]
   >
   >Report deliveries do not contain prompts. If you wish to limit data in a report delivery, we recommend applying filters to the report that you want to send.



1.  Click `Report Actions`, then `Send Report`.


   The `Send Report` dialog box displays.


   >[!TIP] {type="tip"}
   >
   >To send a report manually at any given time, go to the report, then click `Report Actions` > `Send Report` > `Send Now`.



1.  Select the `Repeating Deliveries` tab.
1.  (Conditional) To modify an existing repeating report delivery, select the report delivery in the `Repeating Deliveries` section.
1.  Specify the following information:

<table style="margin-left: 0;margin-right: auto;mc-table-style: url('../../../Resources/TableStyles/TableStyle-List-options-in-steps.css');" class="TableStyle-TableStyle-List-options-in-steps" cellspacing="0"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2"> 
 <tbody> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader"> <p>Send to</p> </td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p>Begin typing the name of the user, group, team, or role who you want to send the report to, then click the name when it appears in the drop-down list.</p> <p>Or</p> <p>Specify the email address of a person external to the <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span> system who you want to have access to the report.</p> <p>Repeat this process to send the report to multiple users, groups, teams, or roles.</p> <p>Note:  <p>Consider the following when adding report delivery recipients:</p> 
     <ul> 
      <li>lf your organization restricts <span class="preview mc-variable WFVariables.ProdNameWF variable varname">Workfront</span> notifications to specific email domains, you may only be able to send reports to email addresses listed in the email allowlist.<p>For information on how a <span class="preview mc-variable WFVariables.AdminWF variable varname">Workfront administrator</span> updates the email allowlist, see the section <a href="configure-your-email-allowlist.md#configur" class="MCXref xref">Configure your email allowlist</a>.</p></li> 
      <li> <p>Adding a large number of users as recipients can cause the delivery to fail. If you experience delivery failures, you can schedule multiple report deliveries with smaller groups of users.</p> </li> 
     </ul> </p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader"> <p>Email Subject</p> </td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray"> <p>Specify a subject for the email notification.</p> <p>By default, the email subject is:</p> <p><em><span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span> Report: [Name of the report] [Date]</em> </p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader"> <p>Email Message</p> </td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p>Specify a message to include in the email.</p> <p>By default, the email message is:</p> <p><em>Attached is the [report frequency] report [Name of the report] generated by <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span> on [Date].</em> </p> <p>Note: For reports delivered as an Excel file only, the following message is also added to the email: "Please be aware that with MS Excel (XLS) file types, there is a limit (65,530) on the number of hyperlinks these file types support. If you exceed those limits, your file will not open and it is recommended to resend without the hyperlinks. Please go back to the report scheduler to remove hyperlinks and resend the report." The "please go back to the report scheduler" phrase is a link back to the report.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader"> <p>Deliver this report with the Access Rights of</p> </td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray"> <p>Begin typing the name of a user who has access to the report, then click the name when it appears in the drop-down list. Users who receive the report will be granted the same level of access to the report as the user that you specify here.<br> For more information, see <a href="run-deliver-report-access-rights-another-user.md" class="MCXref xref">Run and deliver a report with the access rights of another user</a>.</p> <p>Note: This field does not support wildcards. For example, using the wildcard $$User.ID does not run the report with the access rights of the user who is receiving the report.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader"> <p>Format</p> </td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p>Select the format you want for the delivered report:</p> 
    <ul> 
     <li> <p>HTML</p> </li> 
     <li> <p>PDF</p> <p>If you select this, you can format the output using the additional <span class="bold">Paper Size</span> and <span class="bold">Orientation </span>options that display.</p> </li> 
     <li> <p>MS Excel (.xlsx)</p> </li> 
     <li> <p>TSV</p> </li> 
    </ul> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader"> <p>Include Links</p> </td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray"> <p>This option is available only when <span class="bold">MS Excel</span> is selected in the <span class="bold">Format</span> drop-down menu. When this option is enabled, any hyperlinks are included in the exported Excel document.</p> <p>Documents that contain more than 65,530 links cannot be opened. If the exported document will contain more than 65,530 links, deselect this option.</p> <p>This option is enabled by default.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader"> <p>Summary</p> </td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p>Displays a summary of when the delivery repeats.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader"> <p>Repeats</p> </td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray"> <p>Select whether the report should be delivered daily, weekly, monthly, or yearly.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader"> <p>Repeats Every</p> </td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p>Select the frequency with which you want the delivery to repeat. The value you select for this option is based on the option that is selected in the <span class="bold">Repeats</span> drop-down list.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader"> <p>Time</p> </td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray"> <p>Select the time of day for the delivery to be sent.</p> <p>Tip: Because system loads can affect report delivery times, there may be a delay between the scheduled time and the actual delivery time. If you need a report delivered by a specific time, we recommend scheduling the delivery prior to the time that it is needed. For example, we recommend scheduling the delivery a day prior to the date when it is needed.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader"> <p>Repeats On</p> </td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p>This option is available when the <span class="bold">Repeats</span> option is set to either <span class="bold">Weekly</span> or <span class="bold">Monthly</span>:</p> 
    <ul> 
     <li> <p>When the <span class="bold">Repeats</span> option is set to <span class="bold">Weekly</span>: Select the days of the week that the delivery is sent.</p> </li> 
     <li> <p>When the <span class="bold">Repeats</span> option is set to <span class="bold">Monthly</span>: Select whether the delivery is sent on the day of the month, day of the week, or last day of the month (these options leverage the date that you select in the <span class="bold">Starts On</span> field).</p> </li> 
    </ul> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader"> <p>Starts On</p> </td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray">Select the date for the scheduled delivery to begin.</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader"> <p>Ends On</p> </td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray">Select a date for the scheduled delivery to end.</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-MediumGray" role="rowheader"> <p>Never</p> </td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-MediumGray">Select <span class="bold">Never</span> if you want the scheduled delivery to last indefinitely.</td> 
  </tr> 
 </tbody> 
</table>


1.  Click `Save` to save the report delivery.


   The report displays in the `Repeating Deliveries` section (in the `Send Report` dialog box) and it will send at the scheduled time.


   For information about size limitations that can affect the delivery of your reports, see the sections [Report delivery limits](set-up-report-deliveries.md#understanding-export-limits) and [Export limits](set-up-report-deliveries.md#export) in the article [Schedule an automatic report delivery](#).

1.  (Optional) To delete a scheduled delivery:

    
    
    1.  In the `Repeating Deliveries` panel, click the scheduled delivery, then click `Delete`.
    1.  Click `Delete` to confirm.
    
    





## Video walk-through {#video-walk-through}

View the following video to learn how to schedule a report delivery. This video was recorded in *`Workfront Classic`*. However, the content also applies to *`the new Workfront experience`*.


[ ![](assets/video-walk-through--350x197.png)](https://workfront-video.wistia.com/medias/45jffmll62) 
