---
filename: understand-how-organize-reports-dashboard
content-type: overview
product-area: reporting;dashboards
navigation-topic: report-usage
---



# Understand how&nbsp;to organize reports on a dashboard {#understand-how-to-organize-reports-on-a-dashboard}



## Access dashboard information in a report list {#access-dashboard-information-in-a-report-list}

You can see whether a report is added to a dashboard in *`Adobe Workfront`*. This might be useful when deciding which reports you can keep and which can be deleted from the system. If reports are on dashboards, users might still be relying on them. We recommend not deleting reports that are listed on dashboards that users are using.  
For more information about adding reports to dashboards, see the article [Add a report to a dashboard](add-report-dashboard.md).


You can see whether a report is added to a dashboard by doing one of the following:



* Building a view for a list of reports and including dashboard information in the columns
* Filtering a list of reports by one or several specific dashboards that you know are being actively used
* Building a report for the report object and using a view or a filter which include dashboard information


Anyone can build a view or a filter, but you must have Edit access to Reports in your access level to build a report.  
For more information about access to reports, see the article [Grant access to reports, dashboards, and calendars](grant-access-reports-dashboards-calendars.md).  
For more information about building a report, see the article [Create a custom report](create-custom-report.md).



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
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p>Edit access to&nbsp;Reports,&nbsp;Dashboards,&nbsp;Calendars</p> <p>Edit access to Filters, Views, Groupings</p> <p>Note: If you still don't have access, ask your <span class="mc-variable WFVariables.AdminWF variable varname">Workfront administrator</span> if they set additional restrictions in your access level. For information on how a <span class="mc-variable WFVariables.AdminWF variable varname">Workfront administrator</span> can modify your access level, see <a href="create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-MediumGray" role="rowheader">Object permissions</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-MediumGray"> <p>Manage permissions to a report</p> <p>For information on requesting additional access, see <a href="request-access.md" class="MCXref xref">Request access to objects in Adobe Workfront</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your *`Workfront administrator`*.


## Display dashboard information in the View of a report list {#display-dashboard-information-in-the-view-of-a-report-list}

To build a view with dashboard information for a report list:



1.  `<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver"> Click the  <span class="bold">Main Menu</span> icon  <img src="assets/main-menu-icon.png"> in the upper-right corner of  <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span>, then click  <span class="bold">Reports</span>.</MadCap:conditionalText>` 
1. On the list of reports, click the `View` drop-down menu.
1. Click `New View`.
1. Click `Add Column`.
1. Start typing "Dashboards" in the `Start typing field name` field.
1. Under the `Report` object, select `Dashboards`.

1. Click `Save View`.  
   The dashboards that a report appears on display in the Dashboards column of the report list.  
   ![](assets/qs-dashboards-in-report-view.png)  
  





## Filter a report list by dashboard information {#filter-a-report-list-by-dashboard-information}

To filter a list of reports by dashboard information:



1.  `<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver"> Click the  <span class="bold">Main Menu</span> icon  <img src="assets/main-menu-icon.png"> in the upper-right corner of  <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span>, then click  <span class="bold">Reports</span>.</MadCap:conditionalText>` 
1. On the list of reports, click the `Filter` drop-down menu.
1. Click `New Filter`, then click `Add a Filter Rule`.

1. Start typing "Dashboards" in the `Start typing field name` field.  

1. Under the `Dashboards` object, select `Name`.

1. Select `Equal` in the modifier drop-down menu, then start typing the name of the dashboard you want to filter by. You can select multiple dashboards for your filter.  
   ![](assets/qs-dashboards-in-report-filters-350x143.png)


1. Click `Save + Close`.  
   This displays a list of reports that are listed only on the specified dashboards.  
   You can also build a report for the report object and use this filter in the report.  



