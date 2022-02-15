---
filename: customize-terminology
title: Customize user interface terminology using a Layout Template
user-type: administrator
product-area: system-administration;templates;setup
navigation-topic: layout-templates
---



# Customize user interface terminology using a layout template {#customize-user-interface-terminology-using-a-layout-template}

As an *`Adobe Workfront administrator`*, you can use a layout template to change the labels of some objects that appear throughout *`Workfront`* to match terms used in your organization.


After you save a layout template where you changed terminology, then log out of *`Workfront`* and back in again, the labels that you changed appear where the default labels would appear in most areas throughout *`Workfront`*: 


* Main Menu
* All areas accessed from the Main Menu
* All tabs
* All menus
* Report Builder and reporting elements (views, filters and groupings)
* Save buttons
* Exported files
* Emails
* Mobile Apps





>[!NOTE]
>
>
>
>
>* The Outlook Add-in area does not display the customized labels.
>* You might encounter grammar and other problems when you customize labels. For example, if you change "Issue" to "Request," there may be places in the UI where you see the phrase "An request." For more information, see [Implications of customizing object names](understand-objects.md#implications-of-customizing-object-names) in the article [Understand objects in Adobe Workfront](understand-objects.md)
>
>
>



For information about layout templates for groups, see [Create and modify a group’s layout templates](create-and-modify-a-groups-layout-templates.md).


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



## Customize user interface terminology {#customize-user-interface-terminology}




1. Begin working on a layout template, as described in [Create and manage layout templates](create-and-manage-layout-templates.md).
1. Click `Set Terminology` near the upper-right corner of the page.
1. Do any of the following:
    
    
    * To use an alternative term provided by *`Workfront`*, click the down arrow&nbsp; ![](assets/dropdown-arrow.png) next to the label, then click the alternative label you want in the drop-down list.
    
    
      >[!NOTE]
      >
      >Alternative labels provided in the drop-down lists are supported in versions of *`Workfront`* localized for non-English languages.
    
    
    
    * To provide your own custom alternative for the label displayed for an object, click `Set custom name` to the right of the label, then type the `Singular` and `Plural` forms of the custom term. You can click `Reset` if you change your mind.
    
    
      You can customize the following object names:
    
    
    <table style="width: 100%;margin-left: 0;margin-right: auto;mc-table-style: url('../../../Resources/TableStyles/TableStyle-List-options-in-steps.css');" class="TableStyle-TableStyle-List-options-in-steps" cellspacing="0">
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1">
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2">
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2">
 <tbody>
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray">
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader"><p><span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span> objects</p></td>
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column2-LightGray">
    <ul>
     <li>Portfolio</li>
     <li>Program</li>
     <li>Project</li>
     <li>Task</li>
     <li>Issue</li>
     <li>Goal</li>
     <li>Result</li>
     <li>Activity</li>
    </ul></td>
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"><p>For more information about these objects, see <a href="understand-objects.md" class="MCXref xref">Understand objects in&nbsp;Adobe Workfront</a>.</p></td>
  </tr>
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray">
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader"><p><span class="mc-variable WFVariables.Workfront_Align_(Goals) variable varname">Workfront Goals</span> objects</p></td>
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column2-MediumGray">
    <ul>
     <li>Goal</li>
     <li>Result</li>
     <li>Activity</li>
    </ul></td>
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray"><p>These objects require an additional license. For more information, see <a href="wf-goals-overview.md" class="MCXref xref">Adobe Workfront Goals overview</a>.</p></td>
  </tr>
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray" data-mc-conditions="">
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-LightGray" role="rowheader"><p><span class="mc-variable WFVariables.ProdNameWorkfrontScenarioPlanner variable varname">Workfront Scenario Planner</span> objects</p></td>
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column2-LightGray">
    <ul>
     <li>Initiative</li>
     <li>Scenario</li>
     <li>Plan </li>
    </ul></td>
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-LightGray"><p><span>These objects require an additional license. For information, see </span><a href="get-started-with-scenario-planning.md" class="MCXref xref">Get started with the Adobe Workfront Scenario Planner</a>.</p></td>
  </tr>
 </tbody>
</table>    
    
    
    
    
1.  When you are finished, click `Done`.


   >[!TIP] {type="tip"}
   >
   >After you click Done (and even after you save your layout template), you can always return to the Set Terminology settings and click Reset next to any custom terms to return them to their default state.



1.  Continue customizing the layout template.


   Or


   If you are finished customizing, click `Save`.

1. To see your terminology changes:
    
    
    1. Log out and back in to *`Workfront`*.
    1. Close all browser tabs that you have open for your *`Workfront`* environment.
    
    


   >[!IMPORTANT] {type="important"}
   >
   >This is also required for anyone who used the layout template before you made the terminology changes.





For more information about layout templates, see [Create and manage layout templates](create-and-manage-layout-templates.md).
