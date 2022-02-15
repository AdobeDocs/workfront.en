---
filename: reorder-system-statuses
user-type: administrator
product-area: system-administration;projects
navigation-topic: create-custom-status-and-priority-labels
---



# Reorder system-level and group statuses {#reorder-system-level-and-group-statuses}

As a *`Workfront administrator`*, you can change the order of project, task, and issue statuses for `<MadCap:conditionalText data-mc-conditions="SnippetConditions-wf-groups.system-level"> everyone in the system or for a single group</MadCap:conditionalText>`.


![](assets/statuses-350x116.png)




>[!NOTE]
>
>
>
>
>*   `<MadCap:conditionalText data-mc-conditions="SnippetConditions-wf-groups.system-level"> Reordering</MadCap:conditionalText>` the statuses at the system level does not affect the order of statuses within groups. 
>
>
>  However, the statuses within a newly created top-level group inherit the order of the system-level statuses. (A new subgroup inherits the order of the statuses in the group one level up.)
>
>* You can reorder locked statuses. For information about locked statuses, see [Create or edit a status](create-or-edit-a-status.md).
>* *`Group administrators`* can also reorder statuses used in their groups. For more information, see [Reorder group statuses](reorder-group-statuses-from-groups-area.md).
>
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
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray" data-mc-conditions="SnippetConditions-wf-groups.system-level"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-MediumGray" role="rowheader"><a href="https://one.workfront.com/s/document-item?bundleId=the-new-workfront-experience&amp;topicId=Content%2FAdministration_and_Setup%2FAdd_users%2FAccess_levels_and_object_permissions%2Fwf-licenses.html&amp;_LANG=en" target="_blank"><span class="mc-variable WFVariables.FullProdNameWF variable varname">Adobe Workfront</span> license</a>*</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-MediumGray"> <p><span class="mc-variable WFVariables.WFLicense-Plan variable varname">Plan</span> </p> <p>You must be a <span class="mc-variable WFVariables.AdminWF variable varname">Workfront administrator</span>. For information on <span class="mc-variable WFVariables.AdminWF-plur variable varname">Workfront administrators</span>, see <a href="grant-a-user-full-administrative-access.md" class="MCXref xref">Grant a user full administrative access</a>.</p> </td> 
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




## Reorder statuses for tasks and projects`<MadCap:conditionalText data-mc-conditions="SnippetConditions-wf-groups.system-level">  system wide or for a group</MadCap:conditionalText>` {#reorder-statuses-for-tasks-and-projects-system-wide-or-for-a-group}




1. Click the `Main Menu` icon ![](assets/main-menu-icon.png) in the upper-right corner of *`Adobe Workfront`*, then click `Setup` ![](assets/gear-icon-settings.png).

1. In the left panel, click `Project Preferences > Statuses`.
1.  (Conditional) If you are reordering statuses for a group, start typing the name of the group in the box in the upper-right corner, then click the name when it appears.


   ![](assets/system-statuses-in-upper-rt-corner-group-350x139.jpg)



1. Above the Statuses list that displays, click the `Projects` or `Tasks` tab.

1.  Drag and drop the statuses in the order you want.


   The new status order is saved automatically.

1. To test the new status order, go to a task or project, click the status in the upper-right corner, and make sure the statuses that display are in the order that you configured.





## Reorder statuses for issues {#reorder-statuses-for-issues}




1. Click the `Main Menu` icon ![](assets/main-menu-icon.png) in the upper-right corner of *`Adobe Workfront`*, then click `Setup` ![](assets/gear-icon-settings.png).

1. Click `Project Preferences > Statuses.`
1.  (Conditional) If you are reordering statuses for a group, start typing the name of the group in the box in the upper-right corner, then click the name when it appears.


   ![](assets/issue-statuses-group-name-350x162.png)



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

1. To test the new status order, go to an issue, click the status in the upper-right corner, and make sure the statuses that display are in the order that you configured.


