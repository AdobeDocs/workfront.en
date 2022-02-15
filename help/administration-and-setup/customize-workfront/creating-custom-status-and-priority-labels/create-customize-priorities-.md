


# Create and customize priorities {#create-and-customize-priorities}

You can control the priorities for projects, tasks, and issues in the Setup area of *`Workfront`*. Priorities give importance to your projects, tasks, or issues in *`Adobe Workfront`*.


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



## Customizing existing priorities {#customizing-existing-priorities}

As a *`Workfront administrator`*, you can make the following modifications to the default priorities provided in *`Workfront`*:



* Rename priorities.
*  Reorder the priorities.  



  For more information on how to reorder priorities, see [Create a priority for a project task, or issue](#creating-new-priorities).&nbsp;

*  Change the default priority.   



  For more information on the functionality of changing the default priority, see [Create a priority for a project task, or issue](#creating-new-priorities).

* Edit the description for the priorities.&nbsp;
*  Set a color for each priority.  



  The color of the priority is used in chart reports, when you group your results by `Priority`.  



  For more information on chart reports, see [Add a chart to a report](add-chart-report.md).

*  Delete priorities.  



  When you delete an existing priority, you must select a replacement one.

*  Hide priorities.  



  For more information on the functionality of hiding priorities, see [Create a priority for a project task, or issue](#creating-new-priorities).





>[!NOTE]
>
>You must have at least one priority in your *`Workfront`* account for each object.


The priorities provided by default for each object type (project, task, and issue) are identical:



* None
* Low
* Normal
* High
* Urgent




## Create a priority for a project task, or issue {#create-a-priority-for-a-project-task-or-issue}

In addition to the default priorities provided in  *`Workfront`*, you can add your own priorities to reflect the needs of your organization.



1. Click the `Main Menu` icon ![](assets/main-menu-icon.png) in the upper-right corner of *`Adobe Workfront`*, then click `Setup` ![](assets/gear-icon-settings.png).  

1. In the left panel, click `Project Preferences` > `Priorities`.

1.  Click the tab for the object type you want to create a priority for ( `Project`, `Task`, or `Issue`).
1. Click `Add a New Priority`.
1.  Specify&nbsp;the following information for the new priority:

<table style="width: 100%;margin-left: 0;margin-right: auto;mc-table-style: url('../../../Resources/TableStyles/TableStyle-List-options-in-steps.css');" class="TableStyle-TableStyle-List-options-in-steps" cellspacing="0"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2"> 
 <tbody> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader">Priority Name</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray">Type a name for your priority.</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader">Importance</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray"> <p>When adding a new priority, a number is assigned to it&nbsp;by default. Edit this number, if it does not match your needs.</p> <p>The <span class="bold">Importance</span> number for each priority must be unique for the object you selected.<br>The number of the priority&nbsp;reflects the importance&nbsp;of the project, task or issue: the highest number corresponds to the highest priority.</p> <p>Note: &nbsp;You cannot edit the Importance number, after you save the priority.&nbsp;</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader">Color</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p>Choose a color for your priority.</p> <p>The color of the priority is used in chart reports and Agile Team Settings.&nbsp;For more information on chart reports, see <a href="add-chart-report.md" class="MCXref xref">Add a chart to a report</a>.</p> <p>For more information on Agile Team Settings, see in&nbsp;.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader">Default Priority</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray"> <p>Decide whether this should be a default priority&nbsp;or not, by selecting the radio button.</p> <p>If a priority is designated as the <span class="bold">Default Priority</span>, it is automatically picked&nbsp;for all the projects, tasks, or issues in <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span>. <span class="bold">Normal</span> is the default priority for all objects in <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span>.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader">Description</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray">Add a description for your priority&nbsp;to explain its function.</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-MediumGray" role="rowheader">Hide</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-MediumGray"> <p>Select this box if you want to hide&nbsp;the priority.<br>When you select&nbsp;the <span class="bold">Hide</span> option, the priority does not display anywhere in <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span> and users are not able to choose it for their projects, tasks, and issues.</p> <p>Important: &nbsp;We recommend that you hide the priorities that you no longer want to use, rather than deleting them.&nbsp;By hiding them, you still keep all your historic data, of objects that have been completed with this priority, while preventing people from choosing this priority&nbsp;in the future.&nbsp;</p>(Optional) You can change the listing order of your priorities by&nbsp;dragging and dropping them in your desired order. This changes the order in which they display&nbsp;for projects, tasks, and issues. This does not change the <span class="bold">Importance</span> number.&nbsp;</td> 
  </tr> 
 </tbody> 
</table>







1. Click `Save`.


For instructions on applying priorities to projects, tasks and issues, see the following articles:



* [Understand and update project priorities](project-priority.md) 
* [Update Task Priority](task-priority.md) 
* [Update issue Priority](update-issue-priority.md) 


