---
filename: reorder-group-statuses-from-groups-area
user-type: administrator
product-area: system-administration;user-management
navigation-topic: manage-group-statuses
---



# Reorder group statuses {#reorder-group-statuses}

As a ` *`group administrator`*`, you can change the order of project, task, and issue statuses for `a group you manage`.


![](assets/statuses-350x116.png)




If there are any groups above the group you manage, their administrators can also do this for your group. The same is true for *`Workfront administrators`* (for any group).


>[!NOTE]
>
>
>
>
>*   `<MadCap:conditionalText data-mc-conditions="SnippetConditions-wf-groups.groups"> A  <span class="mc-variable WFVariables.AdminWF variable varname">Workfront administrator</span> can reorder</MadCap:conditionalText>` the statuses at the system level`<MadCap:conditionalText data-mc-conditions="SnippetConditions-wf-groups.groups"> . This</MadCap:conditionalText>` does not affect the order of statuses within groups. 
>
>
>  However, the statuses within a newly created top-level group inherit the order of the system-level statuses. (A new subgroup inherits the order of the statuses in the group one level up.)
>
>* You can reorder locked statuses. For information about locked statuses, see [Create or edit a group status](create-or-edit-a-group-status.md).
>
>





## Access requirements {#access-requirements}

You must have the following to perform the steps in this article:

<table style="width: 100%;margin-left: 0;margin-right: auto;mc-table-style: url('../../../Resources/TableStyles/TableStyle-List-options-in-steps.css');" class="TableStyle-TableStyle-List-options-in-steps" cellspacing="0"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2"> 
 <tbody> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader"><a href="https://www.workfront.com/plans" target="_blank"><span class="mc-variable WFVariables.FullProdNameWF variable varname">Adobe Workfront</span> plan</a>* </td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p>Any</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray" data-mc-conditions="SnippetConditions-wf-groups.groups"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-MediumGray" role="rowheader"><a href="https://one.workfront.com/s/document-item?bundleId=the-new-workfront-experience&amp;topicId=Content%2FAdministration_and_Setup%2FAdd_users%2FAccess_levels_and_object_permissions%2Fwf-licenses.html&amp;_LANG=en" target="_blank"><span class="mc-variable WFVariables.FullProdNameWF variable varname">Adobe Workfront</span> license</a>*</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-MediumGray"> <p><span class="mc-variable WFVariables.WFLicense-Plan variable varname">Plan</span> </p> <p>You must be a <span class="mc-variable WFVariables.AdminGroup variable varname">group administrator</span> of the group or a <span class="mc-variable WFVariables.AdminWF variable varname">Workfront administrator</span>. For more information, see <a href="group-administrators.md" class="MCXref xref">Group administrators</a> and <a href="grant-a-user-full-administrative-access.md" class="MCXref xref">Grant a user full administrative access</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;If you need to find out what plan or license type you have, contact your *`Workfront administrator`*.


## Default order of statuses {#default-order-of-statuses}

By default, statuses display in the following order:

<table style="width: 100%;mc-table-style: url('../../../Resources/TableStyles/TableStyle-HeaderRow.css');margin-left: 0;margin-right: auto;" class="TableStyle-TableStyle-HeaderRow" cellspacing="15"> 
 <col class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <col class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <col class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <thead> 
  <tr class="TableStyle-TableStyle-HeaderRow-Head-Header1"> 
   <th class="TableStyle-TableStyle-HeaderRow-HeadE-Column1-Header1" width="33.33%">Project</th> 
   <th class="TableStyle-TableStyle-HeaderRow-HeadE-Column1-Header1" width="33.33%">Task</th> 
   <th class="TableStyle-TableStyle-HeaderRow-HeadD-Column1-Header1" width="33.33%">Issue</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyB-Column1-LightGray"> 
    <ul> 
     <li>Current</li> 
     <li>Dead</li> 
     <li> On Hold </li> 
     <li> Planning </li> 
     <li> Complete </li> 
     <li> Requested </li> 
     <li> Approved </li> 
     <li> Rejected </li> 
     <li> Idea </li> 
    </ul> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyB-Column1-LightGray"> 
    <ul> 
     <li>New</li> 
     <li>In Progress</li> 
     <li>Complete</li> 
    </ul> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyA-Column1-LightGray"> 
    <ul> 
     <li>New</li> 
     <li>In Progress</li> 
     <li>Reopened</li> 
     <li>Awaiting Feedback</li> 
     <li>On Hold</li> 
     <li>Cannot Duplicate</li> 
     <li>Closed</li> 
     <li>Resolved</li> 
     <li>Verified Complete</li> 
     <li>Won't Resolve</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>




## Reorder statuses for tasks and projects `in a group` {#reorder-statuses-for-tasks-and-projects-in-a-group}




1. Click the `Main Menu` icon ![](assets/main-menu-icon.png) in the upper-right corner of *`Adobe Workfront`*, then click `Setup` ![](assets/gear-icon-settings.png).

1. In the left panel, click `Groups`, then click the name of the group.
1. In the left panel, click `Statuses`.
1. Above the Statuses list that displays, click the `Projects` or `Tasks` tab.

1.  Drag and drop the statuses in the order you want.


   The new status order is saved automatically.

1. To test the new status order, go to a task or project `associated with the group`, click the status in the upper-right corner, and make sure the statuses that display are in the order that you configured.





## Reorder statuses for issues {#reorder-statuses-for-issues}




1. Click the `Main Menu` icon ![](assets/main-menu-icon.png) in the upper-right corner of *`Adobe Workfront`*, then click `Setup` ![](assets/gear-icon-settings.png).

1. In the left panel, click `Groups`, then click the name of the group.
1. In the left panel, click `Statuses`.
1. Click the `Issues` tab.
1.   (Optional) Select an issue type ( `Bug Report`, `Change Order`, `Issue`, or `Request`).


   >[!NOTE]
   >
   >
   >    
   >    
   >    *  You cannot customize the order of statuses for the Master List.
   >    * We recommend that you order of statuses for each issue type the same way. For more information about issue types, see [Configure request types](configure-request-types.md).
   >    
   >    




1.  Drag and drop the statuses in the order you want.


   The new status order is saved automatically.

1. To test the new status order, go to an issue `associated with the group`, click the status in the upper-right corner, and make sure the statuses that display are in the order that you configured.


