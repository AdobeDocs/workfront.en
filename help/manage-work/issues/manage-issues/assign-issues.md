---
filename: assign-issues
product-area: projects
navigation-topic: manage-issues
---



# Assign issues {#assign-issues}

You can assign issues to users, roles, and teams to indicate who is responsible for completing the issues. For general information about assigning issues, see [Modify issue assignments overview](modify-issue-assignments-overview.md).

` `**Tip: **`` You can assign multiple users, or job roles, and you can assign only one team. `You can assign only active users, `job roles`, and teams.`


`If a user, `job role`, or a team was assigned before they were deactivated, they remain assigned to the work item. In this case, we recommend the following:` 



*  `Reassign the work item to active resources.` 
*  `Associate the users in a deactivated team with an active team and reassign the work item to the active team.` 


In addition to this article, we recommend that you read the following articles for more information about assigning issues:



* [Modify issue assignments overview](modify-issue-assignments-overview.md) 
* [Edit issues](edit-issues.md) 
* [Edit user assignments for multiple issues](edit-assignments-for-multiple-issues.md) 
* [Create advanced assignments](create-advanced-assignments.md) 
* [Make smart assignments](make-smart-assignments.md) 
* [Smart assignments overview](smart-assignments.md) 
* [Overview of assigning work in the Adobe Workfront Workload Balancer](assign-work-in-workload-balancer.md) 


You can assign an issue to one or multiple resources at the individual issue level, or you can assign multiple resources to multiple issues at one time. 


Assigning issues and tasks is similar in  *`Adobe Workfront`*. For general information about assigning tasks, see [Overview of modifying task assignments](modify-task-assignments-overview.md).


## Access requirements {#access-requirements}

You must have the following access to perform the steps in this article:

<table style="width: 100%;margin-left: 0;margin-right: auto;mc-table-style: url('../../../Resources/TableStyles/TableStyle-List-options-in-steps.css');" class="TableStyle-TableStyle-List-options-in-steps" cellspacing="0"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1"> 
 </col> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2"> 
 </col> 
 <tbody> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader"><span class="mc-variable WFVariables.FullProdNameWF variable varname">Adobe Workfront</span> plan*</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p>Any </p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader"><span class="mc-variable WFVariables.FullProdNameWF variable varname">Adobe Workfront</span> license*</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray"> <p><span class="mc-variable WFVariables.WFLicense-Review variable varname">Review</span> or higher</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader">Access level*</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p>Edit access to Issues</p> <p>View or higher access to Projects and Tasks</p> <p>Note: If you still don't have access, ask your <span class="mc-variable WFVariables.AdminWF variable varname">Workfront administrator</span> if they set additional restrictions in your access level. For information about access to issues in your Access Level, see <a href="grant-access-issues.md" class="MCXref xref">Grant access to issues</a>. For information on how a <span class="mc-variable WFVariables.AdminWF variable varname">Workfront administrator</span> can change your access level, see <a href="create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>. </p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-MediumGray" role="rowheader">Object permissions</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-MediumGray"> <p>Manage permissions to the issue</p> <p>Contribute permissions to the item where you are copying&nbsp;the issue with the ability to&nbsp;Add Issues.</p> <p> For information about granting permissions to issues, see <a href="share-an-issue.md" class="MCXref xref">Share an issue in Adobe Workfront</a></p> <p>For information on requesting additional permissions, see <a href="request-access.md" class="MCXref xref">Request access to objects in Adobe Workfront</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your *`Workfront administrator`*.


## Considerations for multiple assignments to job roles, teams, and users {#considerations-for-multiple-assignments-to-job-roles-teams-and-users}

Users can have more than one job role associated with their profile. For information about associating users with job roles, see [Edit a user's profile](edit-a-users-profile.md). 


Tasks or issues are usually first assigned to one or multiple job roles or to a team. When projects are ready to start, they might need to also be assigned to users.   
If a task or an issue is assigned to one or multiple roles and then you also assign a user, *`Adobe Workfront`* decides which job role to associate with the additional user (if any)&nbsp;according to the following rules:



*  If there is only one job role assigned and it matches the user's Primary Role, then the task or issue is assigned only to the user fulfilling their&nbsp;Primary Role. 
*  If there are multiple roles assigned and at least one of the roles matches the user's secondary roles, then the task or issue is assigned to the user fulfilling one of their Other Roles — which *`Workfront`* selects at random if there are multiple matches — as well as any additional roles that are assigned.
*  If there is one or more job roles assigned and there are no matches to the user's roles, then the task or issue is assigned to both&nbsp;the role or roles as well as to the user. 


If a task or an issue is assigned to a team and you also assign a user, the task or issue remains assigned to both the team and the user. 


## Assign a single issue {#assign-a-single-issue}




1. Go to an issue that you want to assign.
1.  Click `Assign to` in the upper-right corner of the issue header, in the `Assignments` area


   Or


   Click the name of the current assignments, if the issue is already assigned. 


   ![](assets/nwe-assign-to-button-in-header-350x77.png)



1.  Do one of the following:

    
    
    *  Start typing the name of a user, role, or team that you want to assign, then click it when it appears on the list.
    
    
      ![](assets/nwe-assignments-expanded-in-task-header-350x259.png)    
    

    
    * (Conditional) Click one of the names in the `Suggested Assignments` list 
    * Click  `Assign to me` to assign it to yourself
    *  Click `Advanced Assignments`
    
    
      Creating advanced assignments is similar for tasks and issues. For information about how to make advanced assignments, see [Create advanced assignments](create-advanced-assignments.md).
    
    
    

1.  Click `Save` to complete assigning the issue. 
1.  (Optional) Click the `X icon` next to the name of the assignments in the Assignments area on the header of the issue to remove an assignment.




## Assign an issue in a list {#assign-an-issue-in-a-list}

You can assign issues in a list or a report when any of the assignments fields are visible in the list's view. This is faster way to assign issues. 


Depending on which field is visible in the view you can assign the following entities to the issue: 

To assign issues in a list: 



1.  Go to a list of issues that has the Assigned To, Assigned, or Assignments fields in the view.
1.  To assign issues do one of the following:

    
    
    *  Click inside the `Assigned To` or `Assigned` fields and start typing the name of an active user that you want to assign to the issue, then click it when it displays in the list.
    
    
      ![](assets/assigned-to-field-task-list-nwe.png)    
    

    
    *  Click inside the `Assignments` field and start typing the name of an `active` user, `job role`, or `active` team that you want to assign to the issue, then click it when it displays in the list.
    
    
      ![](assets/assignments-field-task-list-nwe.png)    
    

    
    
    

1.  (Conditional) When visible in the Assignments field, click the `People icon` ` ![](assets/teams.png)

   ` in the upper-right corner of the assignments box to open the Advanced Assignments box and create advanced assignments. For more information, see [Create advanced assignments](create-advanced-assignments.md). 


   >[!TIP] {type="tip"}
   >
   >You cannot make advanced assignments from the Assigned To or Assigned fields.



1.  After adding your assignees to the issue, press Enter or click anywhere on the page to save your changes. 




## Assign issues in bulk {#assign-issues-in-bulk}




1. Go to a list of issues that you want to assign in bulk. 
1.  Select several issues in the list. 
1.  Click the `Edit icon` ![](assets/qs-edit-icon.png). 


   The `Edit Issues` dialog box opens.

1.  In the `Assignments` area, select the `Assignee` box, then start typing the name of a user, job role, or team that you want to assign to all the issues. 


   >[!IMPORTANT] {type="important"}
   >
   >If any of the issues is already assigned, the resources you indicate here are added to the issues instead of replacing the existing resources on the issues. 



1. (Optional) Select the radio button in the `Issue Owner` column to indicate which resource is the primary assignee or the Owner of the issue, when you assign more than one resource to the issue. This is not available for teams. 
1. (Optional) Select a role that the user should fulfill on the issue from the `Pick a role` drop-down menu in the `Assignee's Role` column when you assign users to issues. If you do not select a role, *`Workfront`* automatically selects the user's Primary&nbsp;Role. 

1. (Optional) If you want to remove existing assignees from all issues do one of the following:
    
    
    1. Start typing the name of a user, role, or team you want to remove from the issue, then select it when it appears on the list and click `Remove Assignee` to add additional assignees to remove. 
    1. Click  `Remove All Existing Assignees` to remove all assignees from all selected issues.
    
    
1. Click  `Save Changes`.
1. (Optional and conditional) When the Assigned to or the Assignments fields display in your list of issues, click inside one of these columns for an issue, then click the `X icon` next to the name of an assignee to remove it from the issue. 


