---
filename: send-report-preview-sandbox-environment
product-area: reporting
navigation-topic: create-and-manage-reports
---



# Send a report in the Preview Sandbox environment {#send-a-report-in-the-preview-sandbox-environment}


The information on this page refers to functionality that is available only in the Preview and Custom Refresh Sandbox environments. This functionality is not available in the Production environment.


You can set up Report Delivery options in any *`Adobe Workfront`* test environment.


While the test environments are meant to function as close as possible to your production environment, some functionality differs from your production environment.


You can schedule reports in the test environments, but the way they are delivered differs from how they are delivered from the Production environment.


For information about scheduling reports for delivery in the Production environment, see [Report delivery overview](set-up-report-deliveries.md).


Depending on where you schedule the reports, the delivery functionality differs between the Preview and the Custom Refresh sandboxes.



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


## Schedule reports in the Preview environment {#schedule-reports-in-the-preview-environment}




* [Schedule reports in the Preview environment](#schedule3) 




### Schedule reports in the Preview environment {#schedule-reports-in-the-preview-environment-1}

Whether a delivered report is produced or not in the Preview environment depends on whether `Receive emails from this test environment` is enabled or not.


For information about enabling emails from the Sandbox environment see [Enable delivery of emails from the Preview Sandbox environment](enable-delivery-emails-from-preview-sandbox-environment.md).


![](assets/receive-emails-from-sandbox-setting-(1)-350x223.png)




Scheduling reports for delivery in the Preview environment is identical to scheduling reports in the Production environment. For information about scheduling a report for delivery, see [Report delivery overview](set-up-report-deliveries.md).


When you schedule a report for delivery in the Preview environment, the following scenarios exist:



*  When `Receive emails from this test environment` is disabled for the user who is receiving the report, no file is produced when scheduling the report for delivery.
* When `Receive emails from this test environment` is enabled for the user who is receiving the report, the file that is produced when scheduling the report for delivery is added in the Documents tab of the user.  





## Schedule reports in the Custom&nbsp;Refresh Sandbox environment {#schedule-reports-in-the-custom-refresh-sandbox-environment}

Whether a delivered report is produced or not in the Custom Refresh Sandbox depends on whether the Receive emails from this test environment setting is enabled or not.


For information about enabling emails from the Sandbox environment see the section [Activate or deactivate your own event notifications](activate-or-deactivate-your-own-event-notifications.md#managing-emails-in-preview) in the article [Activate or deactivate your own event notifications](activate-or-deactivate-your-own-event-notifications.md).


![](assets/receive-emails-from-sandbox-setting-(1)-350x223.png)




Scheduling reports for delivery in the Custom Refresh Sandbox environment is identical to scheduling reports in the Production environment. For information about scheduling a report for delivery, see [Report delivery overview](set-up-report-deliveries.md).


When you schedule a report for delivery in the Custom Refresh Sandbox environment, the following scenarios exist:



* When the Receive emails from this test environment is disabled for the user who is receiving the report, no file is produced when scheduling the report for delivery.
* When the Receive emails from this test environment is enabled for the user who is receiving the report, the report is emailed as an attachment to the email address associated with the user.




## How external users are notified {#how-external-users-are-notified}

External users do not receive reports sent from the *`Workfront`* test environments, nor do they receive an email notification.


External users only receive emailed reports if they are delivered from a Production environment.
