---
filename: grouping-collapsed-or-expanded-results
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
---



# Grouping: indicate whether the results of a grouping should be collapsed or expanded using text mode {#grouping-indicate-whether-the-results-of-a-grouping-should-be-collapsed-or-expanded-using-text-mode}

You can indicate whether the results in a grouping should display collapsed or expanded in a list or report by using the standard report builder. The results in a grouping display expanded, by default. For information about creating a grouping, see [Create groupings](create-groupings.md).

` `**Tips: **`` 


* When you manually adjust groupings when viewing a list, *`Adobe Workfront`* remembers your manual preference until you log out. When you log back in, the list displays according to this setting.
* The results of a grouping always display expanded after accessing them from a chart element.


You can also indicate whether a grouping should display expanded or collapsed using text mode.



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


## Indicate whether the results of a grouping should be collapsed or expanded using text mode {#indicate-whether-the-results-of-a-grouping-should-be-collapsed-or-expanded-using-text-mode}




1. Go to a list of objects.
1. From the `Grouping`drop-down menu, select `New Grouping`.

1.  Add a grouping and click `Switch to Text Mode`.


   Or


   If the grouping is already in text mode, add the following code to the grouping level that you want to display collapsed:




   ```
   group.0.iscollapsed=true
   ```



1.  (Optional) If you want the grouping to display expanded, add the following code to the appropriate grouping level:




   ```
   group.0.iscollapsed=false
   ```



1. Click `Done`, then `Save Grouping`.



