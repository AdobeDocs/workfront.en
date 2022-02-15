---
filename: convert-issue-to-task
product-area: projects
navigation-topic: convert-issues
---



# Convert an issue to a task in  *`Adobe Workfront`* {#convert-an-issue-to-a-task-in-adobe-workfront}

If more work needs to be done to complete an issue after the issue is submitted, you can convert the issue to a task. 


For general information about converting issues, see [Overview of converting issues in Adobe Workfront](convert-issues.md).




## Access requirements {#access-requirements}

You must have the following access to perform the steps in this article:

<table style="width: 100%;margin-left: 0;margin-right: auto;mc-table-style: url('../../../Resources/TableStyles/TableStyle-List-options-in-steps.css');" class="TableStyle-TableStyle-List-options-in-steps" cellspacing="0"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2"> 
 <tbody> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader"><span class="mc-variable WFVariables.FullProdNameWF variable varname">Adobe Workfront</span> plan*</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p>Any</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader"><span class="mc-variable WFVariables.FullProdNameWF variable varname">Adobe Workfront</span> license*</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray"> <p><span class="mc-variable WFVariables.WFLicense-Work variable varname">Work</span> or higher</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader">Access level configurations*</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p>Edit access to Issues, Tasks, and Projects</p> <p>Note: If you still don't have access, ask your <span class="mc-variable WFVariables.AdminWF variable varname">Workfront administrator</span> if they set additional restrictions in your access level. For information on how a <span class="mc-variable WFVariables.AdminWF variable varname">Workfront administrator</span> can change your access level, see <a href="create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-MediumGray" role="rowheader">Object permissions</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-MediumGray"> <p>View permissions to the issue</p> <p>Contribute permissions to the project</p> <p>You obtain&nbsp;Manage permissions to the task after the issue is converted</p> <p>For information on requesting additional access, see <a href="request-access.md" class="MCXref xref">Request access to objects in Adobe Workfront</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your *`Workfront administrator`*.



## Convert an issue to a task {#convert-an-issue-to-a-task}




1.  `<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver"> Go to a project and click  <span class="bold">Issues</span> in the left panel. </MadCap:conditionalText>` 
1.  Click the issue you want to convert to go to the issue's landing page. 
1.   `<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver"> Click the  <span class="bold">More</span> menu on the issue, then  <span class="bold">Convert to Task</span>. </MadCap:conditionalText>` 


   ![](assets/qs-issue-more-menu-highlighted-350x430.png)



   ` `**Tip: **`` If the issue is associated with an approval process or it is already associated with a resolving object, *`Workfront`* displays a warning at the top of the Convert to Project box to notify you that the approval will be removed or the resolving object will be overwritten during the conversion. For more information, see [Overview of converting issues in Adobe Workfront](convert-issues.md).

1.  Name the task.
1.  Identify the project where the task will reside. 


   You can select a different project from the project that the issue is on.

1.  In the `Project` box, start typing the name of the project where you want to put the new task, then press `Enter` when it appears.


   By default, this box the name of the project containing the issue that you are converting.

1.  (Optional and conditional) Under `Options`, select any of the following options. 


   The *`Workfront administrator`* or *`group administrator`* must enable these preferences before they are visible during the conversion of issues: 

    
    
    *  `Keep the original issue and tie its resolution to the this task` 
    
    
      If unselected, the original issue is deleted.
    
    
      >[!NOTE]
      >
      >Users without access or permissions to delete issues will not be able to delete the issue as they are converting it, regardless of the status of this setting. For information about access and permissions to issues, see:
      >
      >    
      >    
      >    *  [Grant access to issues](grant-access-issues.md) 
      >    *  [Share an issue in Adobe Workfront](share-an-issue.md) 
      >    
      >    

    
    
    
    *  `Allow <User Name> to have access to this task` 
    
    
      If unselected, the issue's Primary Contact has no access to the new task.
    
    *  `Keep the planned completion date of the issue` 
    
    
      If unselected, the Planned Completion Date of the new task is calculated from the Planned Start Date of the task. The Planned Start Date of the new task is set according to the system preferences for new tasks.
    
    
    


   >[!NOTE]
   >
   >
   >The options that display here depend on how the *`Workfront administrator`* configured them for everyone in the system. For more information, see [Configure system-wide task and issue preferences](set-task-issue-preferences.md).
   >
   >
   >Or, if the top-level groups in your organization configured them separately, the options that display here depend on which group is associated with the project you selected in step 6. For more information, see [Configure task and issue preferences for a group](configure-task-issue-preferences-group.md).




1.   (Optional) Attach custom forms. 


   If you want to transfer custom form information from the issue you are converting to the project, add the project custom form that contains the same fields whose information you want to transfer from the issue. 


   For more information about transferring information from the custom form of the issue to that of the new task, see [Transfer custom form data to a larger work item](transfer-custom-form-data-larger-item.md).   


1.  ![](assets/qs-issue-convert-to-task-before-saving-ui-350x206.png)

1.  Click `Save Changes` when all task settings are set.


   The issue is now a task on the designated project, if you decided to delete the original issue.


   Or


   The issue is now linked to the new task on the project you chose, and it will complete once the task completes, if you decided to keep the original issue.


   Some issue fields transfer to the task. For information, see the [View original issue information on projects and tasks](#viewing-original-issue-information) section in this article.   


1.  (Optional) Continue editing the task (assignments, dates) as necessary. 




## View original issue information on projects and tasks {#view-original-issue-information-on-projects-and-tasks}

You can view the original issue information in project and task lists and reports `or in the Project Details area`. For information about building reports, see [Create a custom report](create-custom-report.md). 


The following table illustrates which&nbsp;issue fields are visible from the converted projects and tasks. 

` `**Warning: **``If the Primary&nbsp;Contact of an issue changes or if the issue becomes unlinked from the project or task after the issue has been converted, the Converted Issue Originator Name does not update and it displays the original&nbsp;Primary&nbsp;Contact of the issue at the time the issue was converted. 
