---
filename: create-customize-issue-severities
title: Create and customize issue severities
user-type: administrator
product-area: system-administration;projects
navigation-topic: create-custom-status-and-priority-labels
---



# Create and customize issue severities {#create-and-customize-issue-severities}

As an *`Adobe Workfront administrator`*, you can customize the default severities existing in *`Workfront`* or create new severities that users can associate with issues in *`Workfront`*. 


Issues are unexpected events that can prevent your projects from finishing on time or within budget. You can use severities to define how serious an issue is.


Tasks and projects do not have severities.


##  

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

{#access-requirements-you-must-have-the-following-to-perform-the-steps-in-this-article-adobe-workfront-plan-any-adobe-workfront-license-plan-access-level-configurations-you-must-be-a-workfront-administrator-for-more-information-see-grant-a-user-full-administrative-access-note-if-you-still-dont-have-access-ask-your-workfront-administrator-if-they-set-additional-restrictions-in-your-access-level-for-information-on-how-a-workfront-administrator-can-modify-your-access-level-see-create-or-modify-custom-access-levels}



## Customizing issue severities {#customizing-issue-severities}

There are 5 default issue severities in *`Workfront`*:



* Cosmetic
* Causes Confusion
* Bug with workaround
* Bug with no workaround
* Fatal error


*`Workfront administrators`* can customize the following information on the default severities provided in *`Workfront`*:



* Edit the severity name
*  Change the color associated with the severity


  >[!NOTE]
  >
  >The color of your severity is preserved in a chart report, if you group your results by `Issue Severity`. For more information on chart reports, see [Add a chart to a report](add-chart-report.md).



*  Change the default severity


  For more information about default severities, see [Create new issue severities](#creating-new-issue-severities).

* Edit the description of the severities
*  Hide a severity


  For more information about&nbsp;hiding a severity, see [Create new issue severities](#creating-new-issue-severities).

*  Delete a severity


  When you delete an existing severity, you must select a replacement one.





## Create new issue severities {#create-new-issue-severities}

As a *`Workfront administrator`*, you can create new issue severities to reflect the needs in your organization.&nbsp;



1. Click the `Main Menu` icon ![](assets/main-menu-icon.png) in the upper-right corner of *`Adobe Workfront`*, then click `Setup` ![](assets/gear-icon-settings.png).  

1. In the left panel, click `Project Preferences` > `Severities`.

1. Click `Add a New Severity`.
1.  Fill in the following information for the new severity:

<table style="width: 100%;mc-table-style: url('../../../Resources/TableStyles/TableStyle-List-options-in-steps.css');" class="TableStyle-TableStyle-List-options-in-steps" cellspacing="0"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2"> 
 <tbody> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader">Severity Name</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray">Type a name</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader">Importance</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray"> <p>When adding a new severity, a number is assigned to it by default. Edit this number, if it does not match your needs. The <span class="bold">Importance</span> number for each severity&nbsp;must be unique. The number of the severity reflects the seriousness of the issue: the highest number corresponds to the highest severity.</p> <p>Note: You cannot edit the <span class="bold">Importance</span> number, after you save the severity.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader">Color</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p>Choose a color for the severity.</p> <p>Note: The color of the severity is used in chart reports, when you group your results by <span class="bold">Issue Severity</span>. For more information on chart reports, see <a href="add-chart-report.md" class="MCXref xref">Add a chart to a report</a>.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader">Default Severity</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray">Decide whether this should be a default severity&nbsp;or not, by selecting the radio button.<br>If a severity is designated as the default severity, it is automatically selected for all newly created issues in <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span>. <span class="bold">Cosmetic</span>&nbsp;is the default severity for issues in <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span>.</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader">Description</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray">Type a description for the severity&nbsp;to explain its function.</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-MediumGray" role="rowheader">Hide</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-MediumGray"> <p>Select this box if you want to hide the severity.</p> <p>When you check the <span class="bold">Hide</span> option, the severity&nbsp;does not display anywhere in <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span> and users are not able to choose it for their issues.</p> <p>Important: We recommend that you hide the severities&nbsp;that you no longer want to use, rather than deleting them.&nbsp;By hiding them, you still keep all your historic data, of objects that have been completed with this severity, while preventing people from choosing this severity&nbsp;in the future.</p> </td> 
  </tr> 
 </tbody> 
</table>


1.  (Optional) Change the listing order of your severities by dragging and dropping them in the order you want.


   This changes the order in which they display for issues. It does not change the `Importance` number.

1. Click `Save`.


For more information on how to use severities while working with issues, see [Update issue severity](update-issue-severity.md).
