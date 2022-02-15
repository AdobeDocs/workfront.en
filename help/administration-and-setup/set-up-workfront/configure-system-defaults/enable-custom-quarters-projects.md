---
filename: enable-custom-quarters-projects
user-type: administrator
product-area: system-administration;projects
navigation-topic: configure-system-defaults
---



# Enable custom quarters for projects {#enable-custom-quarters-for-projects}

For reporting purposes, you might want to create custom quarters if your organization's quarters are based on specific criteria other than calendar dates (such as business days or shopping days).


You can configure up to eight custom quarters for your *`Adobe Workfront`* system.


## Access requirements {#access-requirements}

You must have the following to perform the steps in this article:

<table style="width: 100%;margin-left: 0;margin-right: auto;mc-table-style: url('../../../Resources/TableStyles/TableStyle-List-options-in-steps.css');" class="TableStyle-TableStyle-List-options-in-steps" cellspacing="0"> 
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
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-LightGray"> <p>You must be a <span class="mc-variable WFVariables.AdminWF variable varname">Workfront administrator</span>. For more information, see <a href="grant-a-user-full-administrative-access.md" class="MCXref xref">Grant a user full administrative access</a>.</p> <p>Note: If you still don't have access, ask your <span class="mc-variable WFVariables.AdminWF variable varname">Workfront administrator</span> if they set additional restrictions in your access level. For information on how a <span class="mc-variable WFVariables.AdminWF variable varname">Workfront administrator</span> can modify your access level, see <a href="create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>



## Set up custom quarters for your *`Workfront`* system {#set-up-custom-quarters-for-your-workfront-system}




1. Click `Setup` near the upper-right corner of *`Adobe Workfront`* on the Global Navigation Bar.

1. Click `Project Preferences` > `Projects.`

1. In the `Timelines` section, select `Enable Custom Quarters`.

1.  Type a name for the custom quarter.
1. Select start and end dates for the custom quarter.
1.  (Optional) Click `Add Custom Quarter` to add additional custom quarters to the system.


   ![](assets/custom-quarters-nwe-350x107.png)



1.  (Optional) Create a reporting element that refers to the fiscal quarters. 

   ` `**Example: **`` Create a filter for a project list and include the Planned Completion Date of a project referencing the custom quarters.


   ![](assets/example-of-project-filter-with-custom-quarters-350x406.png)




   The references to "This Quarter", "Next Quarter", and "Last Quarter"&nbsp;are replaced with new references to the custom quarters. 


   For information about reporting elements, see [Reporting elements: filters, views, and groupings](reporting-elements-filters-views-groupings.md). 


   For information about creating filters, see [Create or edit filters in Adobe Workfront](create-filters.md). 



&nbsp;
