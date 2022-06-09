---
title: Legacy Workfront Fusion service outages
user-type: administrator
content-type: reference
product-area: system-administration;workfront-integrations
navigation-topic: administrator-integrations
description: Legacy Workfront Fusion is not available as of March 31, 2021.
feature: "System Setup and Administration, Workfront Integrations and Apps"
role: Admin
---

# Legacy Workfront Fusion service outages

>[!IMPORTANT]
>
>Legacy Workfront Fusion is not available as of March 31, 2021.
>
>For information about Adobe Workfront Fusion, see [Adobe Workfront Fusion](../../workfront-fusion/workfront-fusion-2.md)

Because of the nature of Legacy Workfront Fusion, service outages have unique implications for active FLOs, depending on how each FLO is initiated.

For more details on specific incidents that could affect your FLOs, check our status page at [trust.workfront.com](https://trust.workfront.com/). Contact Workfront Support for further assistance.

The following table shows how each type of FLO is affected by a service outage:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p><strong>FLO type</strong> </p> </th> 
   <th> <p><strong>Affect during a service outage</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td><strong>Monitor FLOs</strong> </td> 
   <td>Triggered when a scheduled check finds new application data (such as when a new task is created in Workfront). Each Monitor FLO tracks when the last check was made and what the last new record was. Data is not lost when a scheduled check is missed during an outage because the new data is detected by the first check after the outage. The default for monitor FLOs is to check every 5 minutes, so an outage usually results in only a short delay to processing this type of data.</td> 
  </tr> 
  <tr> 
   <td><strong>Real-time (webhook) and API endpoint FLOs</strong> </td> 
   <td> Initiated directly by another application, including Workfront, through real-time triggers. If there is a service outage at the time of the call, the result depends on how the calling application recovers from getting no response. Like other applications, Workfront automatically retries calls again later so they succeed with the call when Legacy Workfront Fusionis back online. Workfront is designed to retry sending events when the Legacy Workfront Fusion service is unavailable and, as such, events are processed by Legacy Workfront Fusion after the service fully resumes. For more details about event subscription retries in Workfront, see <a href="../../wf-api/api/event-sub-retries.md" class="MCXref xref">Event subscription retries</a>.</td> 
  </tr> 
  <tr> 
   <td><strong>Scheduled FLOs</strong> </td> 
   <td> <p>A FLO that runs on a fixed schedule misses any scheduled runs during a full outage. Because of this, you might need to manually run the scheduled FLO after an outage is complete. </p> </td> 
  </tr> 
  <tr> 
   <td><strong>Form FLOs</strong> and <strong>FLO Pages</strong></td> 
   <td>Unavailable during outages.</td> 
  </tr> 
 </tbody> 
</table>

