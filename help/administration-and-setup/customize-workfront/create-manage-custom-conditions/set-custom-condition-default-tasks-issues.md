---
filename: set-custom-condition-default-tasks-issues
title: Set a custom Condition as the default for tasks and issues
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-conditions
---



# Set a custom condition as the default for tasks and issues {#set-a-custom-condition-as-the-default-for-tasks-and-issues}

When a user clicks Work on It or adds an update comment to a new task they have been assigned to (without manually setting a condition for the task), *`Adobe Workfront`* displays the default condition for tasks, which is configured in Setup. The same is true for issues.


*`Workfront`* uses the built-in condition `Going Smoothly` as the default condition for tasks and, separately, for issues. As a *`Workfront administrator`*, you can change the default condition for both of these object types to a custom condition you have created.


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



## Set a custom condition as a default condition for tasks or for issues: {#set-a-custom-condition-as-a-default-condition-for-tasks-or-for-issues}




1. Click the `Main Menu` icon ![](assets/main-menu-icon.png) in the upper-right corner of *`Adobe Workfront`*, then click `Setup` ![](assets/gear-icon-settings.png).

1. Click `Project Preferences` > `Conditions`.

1. Click the `Tasks` or `Issues` tab. 

1. Click `Set Default Conditions`. 
1. In the drop-down menu, click the custom condition you want as the default condition for tasks (or issues). 
1. Click `Save`.




>[!NOTE]
>
>
>
>
>*  A user who is assigned to a task or issue, or who has Manage permissions on it, can change its condition manually. For more information, see [Update Condition for tasks and issues](update-condition-for-tasks-and-issues.md).
>*  The three default conditions for tasks and issues that come with Workfront are Going Smoothly, Some Concerns, and Major Roadblocks. You cannot hide or delete these conditions, but you can change their names and colors. Or you can create new ones to use instead, as described in [Create or edit a custom condition](create-edit-custom-conditions.md).
>
>



For information about configuring a custom condition as a default condition for projects, see [Set a custom condition as the default for projects](set-custom-condition-default-projects.md). 


For information about custom conditions, see [Custom conditions](_custom-conditions.md).
