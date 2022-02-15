---
filename: create-dashboard
product-area: dashboards
navigation-topic: create-and-manage-dashboards
---



# Create a dashboard {#create-a-dashboard}

You can create dashboards to quickly access information in reports, calendars, and external pages.


To learn more about dashboards, see [Get started with dashboards](get-started-dashboards.md).


## Access requirements {#access-requirements}

You must have the following:

<table class="TableStyle-TableStyle-HeaderRow" style="mc-table-style: url('../../../Resources/TableStyles/TableStyle-HeaderRow.css');caption-side: bottom;" cellspacing="15"> 
 <caption style="text-align: left;">
  *To find out what plan, license type, or access you have, contact your <span class="mc-variable WFVariables.AdminWF variable varname">Workfront administrator</span>.
 </caption> 
 <col class="TableStyle-TableStyle-HeaderRow-Column-Column1" style="width: 300px;"> 
 </col> 
 <col class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 </col> 
 <tbody> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray" style="font-weight: bold;"> <p><span class="mc-variable WFVariables.FullProdNameWF variable varname">Adobe Workfront</span> plan*</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray">Any</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray" style="font-weight: bold;"> <p><span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span> license*</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> <p><span class="mc-variable WFVariables.WFLicense-Plan variable varname">Plan</span> </p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"><span class="bold">Access level configurations*</span> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p>Edit access to Reports, Dashboards, and Calendars</p> <p>Note: If you still don't have access, ask your <span class="mc-variable WFVariables.AdminWF variable varname">Workfront administrator</span> if they set additional restrictions in your access level. For information on how a <span class="mc-variable WFVariables.AdminWF variable varname">Workfront administrator</span> can change your access level, see <a href="create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyB-Column1-MediumGray" style="text-align: left;"> <p><span class="bold">Object permissions</span> </p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyA-Column1-MediumGray"> <p>You will obtain Manage permissions to the new dashboard</p> <p>For information on requesting additional access, see <a href="request-access.md" class="MCXref xref">Request access to objects in Adobe Workfront</a>.<br>For more information on permissions for dashboards, see <a href="permissions-reports-dashboards-calendars.md" class="MCXref xref">Share reports, dashboards, and calendars in Adobe Workfront</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>



## Prerequisites {#prerequisites}

You must create any of the following objects before you can add them to a dashboard: 


* `Reports`: For information on creating reports, see [Create a custom report](create-custom-report.md).

* `Calendars`: For information on creating calendars, see [Calendar reports overview](calendar-reports-overview.md).

* `External pages`: For information on creating external pages, see [Embed an external web page in a dashboard](embed-external-web-page-dashboard.md).






## Create a dashboard {#create-a-dashboard-1}




1.   `<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver"> <span style="font-weight: normal;">Click the </span> <span class="bold">Main Menu </span>icon  <img src="assets/main-menu-icon.png"> <span style="font-weight: normal;">, then click </span> <span class="bold">Dashboards.</span></MadCap:conditionalText>` 
1. Click `New Dashboard`.  
   The New Dashboard dialog box displays.

1. Specify the following: 

<table style="mc-table-style: url('../../../Resources/TableStyles/TableStyle-List-options-in-steps.css');" class="TableStyle-TableStyle-List-options-in-steps" cellspacing="0">
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1">
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2">
 <tbody>
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray">
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader">Name</td>
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"><p>This is the name of your dashboard.</p><p>If you do not specify a name, the name of the first report on the dashboard becomes the name of the dashboard, by default.</p></td>
  </tr>
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray">
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-MediumGray" role="rowheader">Description (Optional)</td>
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-MediumGray">This is a description of your dashboard.</td>
  </tr>
 </tbody>
</table>

1.  Select a layout by clicking the radio button corresponding to it.


   The single-column layout is the default.


   For information about report layout on dashboards, see [Understand how reports display on a dashboard](understand-how-reports-display-dashboard.md).

1.  Add existing reports, calendars, or external pages by searching for them in the `Search by name or type ...` field, then dragging them to the layout pane, when they appear in the list.


   >[!NOTE]
   >
   >When searching for an item, the search returns any of the 2,000 most recently created reports. Report names that include unicode characters are not returned in search results. As a best practice, avoid including unicode characters when naming objects in *`Workfront`* by typing names rather than copying and pasting names from another source. 


   ![](assets/qs-new-dashboard-ui-350x143.png)



1. (Optional) Click `Add External Page` to add an External Page to the dashboard.   
   For more information about creating external pages and embedding them into dashboards, see [Embed an external web page in a dashboard](embed-external-web-page-dashboard.md).

1. Click `Save + Close`.  
   A timestamp is displayed in the upper-right corner of the dashboard. The timestamp includes the date, time, and time zone when the dashboard was last refreshed.



