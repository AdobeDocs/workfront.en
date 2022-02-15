---
filename: edit-assignments-for-multiple-issues
product-area: projects
navigation-topic: manage-issues
---



# Edit user assignments for multiple issues {#edit-user-assignments-for-multiple-issues}

You can simultaneously modify user assignments to multiple issues.&nbsp;For information about editing issues or assigning them one at a time, also see the following articles:



* [Edit issues](edit-issues.md) 
* [Assign issues](assign-issues.md) 


For general information about assigning issues, see [Modify issue assignments overview](modify-issue-assignments-overview.md). 


>[!NOTE]
>
>You must have at least Contribute permissions to an issue be able to make assignments to the issue. 





## Access requirements {#access-requirements}

You must have the following access to perform the steps in this article:

<table style="width: 100%;margin-left: 0;margin-right: auto;mc-table-style: url('../../../Resources/TableStyles/TableStyle-List-options-in-steps.css');" class="TableStyle-TableStyle-List-options-in-steps" cellspacing="0"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2"> 
 <tbody> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader"><span class="mc-variable WFVariables.FullProdNameWF variable varname">Adobe Workfront</span> plan*</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p>Any </p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader"><span class="mc-variable WFVariables.FullProdNameWF variable varname">Adobe Workfront</span> licenses*</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray"> <p><span class="mc-variable WFVariables.WFLicense-Request variable varname">Request</span> or higher</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader">Access level configurations*</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p>Edit access to Issues</p> <p>Note: If you still don't have access, ask your <span class="mc-variable WFVariables.AdminWF variable varname">Workfront administrator</span> if they set additional restrictions in your access level. For information on how a <span class="mc-variable WFVariables.AdminWF variable varname">Workfront administrator</span> can modify your access level, see <a href="create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-MediumGray" role="rowheader">Object permissions</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-MediumGray"> <p>Manage permissions to the issue</p> <p>For information on requesting additional access, see <a href="request-access.md" class="MCXref xref">Request access to objects in Adobe Workfront</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your *`Workfront administrator`*.


## Modify assignments for multiple issues {#modify-assignments-for-multiple-issues}




1. Go to the issue list that contains the&nbsp;issues whose assignments you want to modify. 
1.  (Optional) Create a filter to display only issues assigned to the assignee that you want to modify.


   For example, you can create a filter to display only issues with a specific role as the assignee.&nbsp;Then, you can&nbsp;replace the role with a specific user. Do the following:

    
    
    1.  Click the `Filter` drop-down list, then click `New Filter`.
    
    
       The New Filter dialog box displays. 
    
    1. Click `Add a Filter Rule.`
    1.  To filter for a specific role, expand `Assignment Roles,` then click `ID.`
    
    
       Or
    
    
       To filter for a specific user, expand `Assignment Users,` then click `ID.`
    
    
       >[!TIP] {type="tip"}
       >
       >Do not use `Assigned to`&nbsp;because this field refers only to the Issue Owner and not to all assignees.
    
    
    
    1. In the drop-down list, select `Equal` as the filter qualifier.
    1. Begin typing the name of the user or role that you want to filter for, then click the name when it appears in the drop-down list.
    1. Click `Save Filter.`
    
    

1.  Select the issues for which you want to modify assignments, then click the `Edit` icon ![](assets/qs-edit-icon.png). 


   The `Edit Issues` displays. The items that are edited display in the upper-left corner of the page.

1.  Go to the `Assignments` section, then select `Assignee`.


   ![](assets/classic-assignmens-area-on-edit-box-350x119.png)



1. Do one of the following:
    
    
    1. `<li>To add a new assignee:  <ol>  <li value="1"><p>Start typing the name of a user, role, or team, then select it when it displays in the list. The assignment is added and does not replace the current assignments on the selected issues. </p>   <div class="tip_one-tip-with_bullets" data-mc-autonum="<b>Tip: </b>">    <span class="autonumber"><span><b>Tip: </b></span></span>    <p>You can assign multiple users, or job roles, and you can assign only one team. <span>You can assign only active users, <span>job roles</span>, and teams. </span></p>    <p><span>If a user, <span>job role</span>, or a team was assigned before they were deactivated, they remain assigned to the work item. In this case, we recommend the following:</span></p>    <ul>     <li><p><span>Reassign the work item to active resources. </span></p></li>     <li><p><span>Associate the users in a deactivated team with an active team and reassign the work item to the active team. </span></p></li>    </ul>   </div><p>Information that is common across all issues selected displays. For example, if the same user is assigned to all issues, that user displays in the <span class="bold">Assignee</span>&nbsp;column. If information is not common across the issues selected, no information displays.</p></li> </ol></li>``<li>To remove individual assignees:  <ol>  <li value="1"><p>Click the <span class="bold">X icon</span> next to the name of the assignee that you want to remove if the assignee displays in the Assignments list.</p><p>Or</p><p>(Conditional) If the assignee that you want to remove does not display in the Assignments section because the assignee is assigned to only some of the issues that you have selected, click <span class="bold">Remove Assignee</span> and start typing the name of the assignee that you want to remove, then click the name when it appears in the drop-down list.</p></li>  <li value="2">Click&nbsp;<span class="bold">Remove Assignee</span> again to add another assignee to remove.</li> </ol></li>``<li>To remove all existing assignees:  <ol>  <li value="1"><p>Click <span class="bold">Remove All Existing Assignees</span>, then click <span class="bold">Yes, Delete All Assignees</span>.</p><p>This removes not only common assignees (assignees that are displayed in the edit&nbsp;dialog box), but also all assignees on all the selected issues.</p></li> </ol></li>`
    
    
    
1.  (Optional) Modify any of the following options for the assignees you selected to associate with the issues:

    
    
    * `Issue Owner:` Select the radio button to indicate which assignee is designated as the Issues Owner. If left unselected, *`Adobe Workfront`* designates the first assignee as the Issue Owner. This is not available for team assignments. 
    
    * `Assignee's Role`: Select a role from the drop-down list. If left unselected, *`Workfront`* automatically selects the Primary Role of the user. 
    
    
    

1. Click `Save Changes`.


