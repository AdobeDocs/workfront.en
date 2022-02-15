---
filename: legacy-fusion-service-outages
title: Workfront Fusion service outages
user-type: administrator
content-type: reference
product-area: system-administration;workfront-integrations
navigation-topic: administrator-integrations
---



# *`Legacy Workfront Fusion`* service outages {#legacy-workfront-fusion-service-outages}



>[!IMPORTANT] {type="important"}
>
>*`Legacy Workfront Fusion`* is not available as of March 31, 2021.
>
>
>For information about *`Adobe Workfront Fusion`*, see [Adobe Workfront Fusion](workfront-fusion-2.md)



Because of the nature of *`Legacy Workfront Fusion`*, service outages have unique implications for active FLOs, depending on how each FLO is initiated. 


For more details on specific incidents that could affect your FLOs, check our status page at [trust.workfront.com](https://trust.workfront.com/). Contact *`Workfront`* Support for further assistance. 


The following table shows how each type of FLO is affected by a service outage:

<table style="mc-table-style: url('../../Resources/TableStyles/TableStyle-HeaderRow.css');margin-left: 0;margin-right: auto;width: auto;" class="TableStyle-TableStyle-HeaderRow" cellspacing="15"> 
 <col class="TableStyle-TableStyle-HeaderRow-Column-Column1" style="width: 334px;"> 
 <col class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <thead> 
  <tr class="TableStyle-TableStyle-HeaderRow-Head-Header1"> 
   <th class="TableStyle-TableStyle-HeaderRow-HeadE-Column1-Header1"> <p><span class="bold">FLO type</span> </p> </th> 
   <th class="TableStyle-TableStyle-HeaderRow-HeadD-Column1-Header1"> <p><span class="bold">Affect during a service outage</span> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"><span class="bold">Monitor FLOs</span> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray">Triggered when a scheduled check finds new application data (such as when a new task is created in <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span>). Each Monitor FLO tracks when the last check was made and what the last new record was. Data is not lost when a scheduled check is missed during an outage because the new data is detected by the first check after the outage. The default for monitor FLOs is to check every 5 minutes, so an outage usually results in only a short delay to processing this type of data.</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"><span class="bold">Real-time (webhook) and API endpoint FLOs</span> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> Initiated directly by another application, including <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span>, through real-time triggers. If there is a service outage at the time of the call, the result depends on how the calling application recovers from getting no response. Like other applications, <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span> automatically retries calls again later so they succeed with the call when <span class="mc-variable WFVariables.ProdNameWFF-L variable varname">Legacy Workfront Fusion</span>is back online. <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span> is designed to retry sending events when the <span class="mc-variable WFVariables.ProdNameWFF-L variable varname">Legacy Workfront Fusion</span> service is unavailable and, as such, events are processed by <span class="mc-variable WFVariables.ProdNameWFF-L variable varname">Legacy Workfront Fusion</span> after the service fully resumes. For more details about event subscription retries in <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span>, see <a href="event-sub-retries.md" class="MCXref xref">Event subscription retries</a>.</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"><span class="bold">Scheduled FLOs</span> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p>A FLO that runs on a fixed schedule misses any scheduled runs during a full outage. Because of this, you might need to manually run the scheduled FLO after an outage is complete. </p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyB-Column1-MediumGray"><span class="bold">Form FLOs</span> and <span class="bold">FLO Pages</span></td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyA-Column1-MediumGray">Unavailable during outages.</td> 
  </tr> 
 </tbody> 
</table>

