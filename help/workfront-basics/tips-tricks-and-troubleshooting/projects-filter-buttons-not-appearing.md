---
filename: projects-filter-buttons-not-appearing
content-type: tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-basics
---



# Projects I'm On and Projects I Own filter buttons do not appear on the Projects page header {#projects-im-on-and-projects-i-own-filter-buttons-do-not-appear-on-the-projects-page-header}



## Problem {#problem}

The `Projects I'm On` and `Projects I Own` filter buttons do not appear in the page header of the Projects list.


## Access requirements {#access-requirements}

You must have the following access to perform the steps in this article:

<table style="width: 100%;margin-left: 0;margin-right: auto;mc-table-style: url('../../Resources/TableStyles/TableStyle-List-options-in-steps.css');" class="TableStyle-TableStyle-List-options-in-steps" cellspacing="0"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2"> 
 <tbody> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader"><span class="mc-variable WFVariables.FullProdNameWF variable varname">Adobe Workfront</span> plan</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p>Any</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader"><span class="mc-variable WFVariables.FullProdNameWF variable varname">Adobe Workfront</span> license</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray"> <p><span class="mc-variable WFVariables.WFLicense-Plan variable varname">Plan</span> </p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-LightGray" role="rowheader">Access level configurations</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-LightGray"> <p>System administrator</p> </td> 
  </tr> 
 </tbody> 
</table>



## Solution {#solution}

The project filter buttons are not included in the default layout template. The *`Workfront administrator`* must assign a layout template that includes the buttons.



1. Verify that the layout template displays the filter buttons:
    
    
    1. Access the layout template.
    1. Select `Lists` under `Customize what users see`.
    
    1. Select `Projects` under `Select a list to customize`.
    
    1. In the Filter section, verify that `Projects I'm On` and `Projects I Own` are selected.
    
    1. Click `Save`.  
       For more information, see [Customize Filters, Views, and Groupings using a layout template](customize-fvg-list-controls-layout-template.md).
    
    
    
1. Assign the layout template to the correct users, job roles, teams, or groups. For information, see [Assign users to a layout template](assign-users-to-layout-template.md).


