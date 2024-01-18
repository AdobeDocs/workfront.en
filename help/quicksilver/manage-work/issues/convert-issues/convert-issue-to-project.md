---
product-area: projects
navigation-topic: convert-issues
title: Convert an issue to a project in Adobe Workfront
description: Convert an issue to a project in Adobe Workfront
author: Alina
feature: Work Management
exl-id: e3ba15a3-6169-466c-9912-32a8afdcc68d
---
# Convert an issue to a project in Adobe Workfront

If more work needs to be done to complete an issue after the issue is submitted, you can convert the issue to a project.

You can convert an issue to a new project or you can convert it to a project using a template. This article describes both ways for converting issues to projects.

>[!IMPORTANT]
>
>For general information about converting issues, we recommend that you also read the article [Overview of converting issues in Adobe Workfront](../../../manage-work/issues/convert-issues/convert-issues.md).

When creating a project from an issue, some of the fields on the project populate from other objects. For more information, see the "New project default settings" section in the article [Create a project](../../../manage-work/projects/create-projects/create-project.md). 

## Access requirements

You must have the following access to perform the steps in this article:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Issues, Tasks, and Projects</p> <p>Edit access to Financial Data to update financial information for a projected converted from the issue</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View permissions to the issue</p> <p>You obtain Manage permissions to the project after the issue is converted</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*To find out what plan, license type, or access you have, contact your Workfront administrator.

## Convert an issue to a project

You can convert an issue to a blank project or convert an issue to a project using a template.

1. Go to a project and click **[!UICONTROL Issues]** in the left panel. 
1. In the list of issues that displays, do one of the following:

   * To convert an issue to a blank project, click the name of the issue, click the **[!UICONTROL More]** menu ![](assets/more-icon.png) to the right of the issue name, then click **[!UICONTROL Convert to a blank project]**.

        
     Or   
      
     Select the issue in the list of issue, click the **[!UICONTROL More]** menu ![](assets/more-icon.png) at the top of the list, then click **[!UICONTROL Convert to a blank project]**. 

      >[!IMPORTANT]
      >
      >The Convert to a blank project option displays only when your system or group administrator enabled the [!UICONTROL Allow users to create projects without using a template] preference in the [!UICONTROL Setup] area. For more information, see [Configure system-wide project preferences](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).


     You must manually add tasks to the project or attach a template to the project after you convert the issue.
     
     Continue with Step 3e below. 
     
     <!--
     Is this accurate?
     -->
       
     >[!TIP]
     >   
     >* If the issue was created using a request queue, the new project inherits the request queue's Group. 
     >* If the issue was created by adding it to the Issues section of the project, the new project inherits the Group of the issue's project.

   * To convert an issue to a project using a template, do one of the following:

      * Click the name of an issue, then click the [!UICONTROL **More**] menu ![](assets/more-icon.png) to the right of the issue name

        Or
      
      * Select the issue in the list of issues, in a report, or dashboard, click the **More** menu ![](assets/more-icon.png) at the top of the list, then click **Convert to project from Template** and start typing the name of a template in the **Search Template** box, then click the name of the template when it displays in the list. Continue with Step 3.       
      
        <!--      
        (is this accurate?)      
        -->

     >[!TIP]
     >
     >If you added templates to your Favorites list, you can mouse over the [!UICONTROL **Favorite templates**] menu and click the template you want to use.

     The New Project from Template box displays. 

     ![](assets/new-project-from-template-small-box-with-template-details-panel-nwe-350x279.png)

     >[!TIP]
     >
     >If the issue is associated with an approval process or it is already associated with a resolving object, Workfront displays a warning at the top of the Convert to Project box to notify you that the approval will be removed or the resolving object will be overwritten during the conversion. For more information, see [Overview of converting issues in Adobe Workfront](../../../manage-work/issues/convert-issues/convert-issues.md).

1. (Conditional) If you selected to convert the issue to a project using a template, continue with the following steps:

   1. Review template details on the right.

      The template details include the following:

      * Template duration
      * Template owner
      * The number of top-level tasks which includes the names of the top three tasks
      * The number of all tasks in the template
      * The names of the template custom forms

   1. (Optional) Mouse over the name of a template and click the Favorites icon ![](assets/favorites-icon-small.png) to mark it as a favorite for future use.

      >[!TIP]
      >
      >You can have up to 40 Workfront items marked as favorites. This includes templates and other items.

   1. Click [!UICONTROL **Use template**] to select a template.

      The [!UICONTROL Convert to Project] box opens.

      ![](assets/convert-to-project-from-template-large-project-box-nwe-350x291.png)

   1. If a field is already populated in the template, the field is pre-populated in the [!UICONTROL Convert to project] box. You can edit the pre-populated values to better match your project. For more information, see [Edit projects](../../../manage-work/projects/manage-projects/edit-projects.md).

      >[!TIP]
      >
      >* Your system or group administrator can add or remove fields in the [!UICONTROL Convert to Project box] by updating the Project Details information in your [!UICONTROL Layout Template]. 
      >
      >* To update fields in the [!UICONTROL Finance] section in the [!UICONTROL Convert to Project] box you must have [!UICONTROL Edit] access to [!UICONTROL Financial Data] in your access level. If you have [!UICONTROL View] access to [!UICONTROL Financial Data] in your access level all financial information from the template transfers to the new project and you cannot edit it while you convert the issue. For information, see [Grant access to financial data](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md) and [Share a template](../../../workfront-basics/grant-and-request-access-to-objects/share-a-template.md).

   1. (Optional and conditional) Click [!UICONTROL **Options**] in the left panel, then select from the options that are available:

      * [!UICONTROL **Keep the original issue and tie its resolution to this project**]

        When deselected, the original issue is deleted.

        >[!NOTE]
        >
        >Users without access or permissions to delete issues will not be able to delete the issue as they are converting it, regardless of the status of this setting. For information about access and permissions to issues, see:
        >
        >* [Grant access to issues](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-issues.md)
        > 
        >* [Share an issue](../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md) 

      * [!UICONTROL **Allow (User Name) to have access to this project**]

        If unselected, the issue's [!UICONTROL Primary Contact] has no access to the new task.

        >[!NOTE]
        >
        >The options that are available here depend on how the Workfront administrator has configured them for everyone in the system or for your group. For more information, see [Configure system-wide task and issue preferences](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).
        >
        >
        >Or, if the top-level groups in your organization configured them separately, the options available here depend on which group you selected for the new project in step 6. For more information, see [Configure task and issue preferences for a group](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md).

   1. Click [!UICONTROL **Custom Forms**] and do any of the following:

      * Review the custom forms attached to the template. They will transfer to the new project.
      * Ensure all required fields have valid information. 
      * Rearrange the custom forms by dragging them ![](assets/drag-object-icon.png) where you want them. 
      * Click the **x** icon to the right of any form that you do not want to transfer to the project. 
      * If necessary, transfer custom form information from the issue to the project.

        >[!TIP]
        >
        >* If a multi-object custom form attached to the issue is configured for use with both issues and projects, all information saved in the form is retained when you make the conversion if the fields exist both on the issue as well as the project's custom forms.
        >* If a multi-object custom form with a calculated field is attached to the issue as well as to the project, the issue and the project must be compatible with all fields referenced in the form's calculated custom fields. If there is an incompatibility, a message alerts you to make adjustments. For more information, see the "Calculated custom fields in multi-object custom forms" section in the [Add calculated data to a custom form with the legacy form builder](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md). 
        >* If you are using a template for the conversion and a custom form attached to the template contains a custom field also found in a custom form attached to the issue, the field value from the issue is used for the new project. However, if the custom field is blank on the issue, the value from the template is used.

   1. Click [!UICONTROL **Convert to project**].

      >[!TIP]
      >
      >If you decided to delete the original issue, the issue is now a project.
      >   
      >Or
      >  
      >If you decided to keep the original issue, the issue is now linked to the new project and it will complete when the project completes. 
      >
      >Some issue fields transfer to the project. Most fields defined in the template automatically transfer to the newly created project if you didn't change them in previous steps. For information, see [Overview of converting issues in Adobe Workfront](../../../manage-work/issues/convert-issues/convert-issues.md).

1. (Optional) Set any further project details ​(project owner, project dates) and tasks as necessary.
1. Click [!UICONTROL **Convert to project**].

   The issue is now converted to a project. 

1. Click [!UICONTROL **Go to project**] inside the [!UICONTROL Success] notification in the upper-right corner of the page. This opens the project page.
