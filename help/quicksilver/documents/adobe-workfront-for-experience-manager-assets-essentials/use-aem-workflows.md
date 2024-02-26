---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: Use workflows in the Experience Manager Assets Essentials integration
description: Use workflows in the Experience Manager Assets Essentials integration
author: Courtney, Becky
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: 4c1e5ec1-3fd1-4527-ba8a-9db1a2350f69
---
# Use workflows in the Experience Manager Assets integration

<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview Sandbox environment.</span>

A workflow is a set of actions that connect Workfront to Adobe Experience Manager as a Cloud Service. A Workfront administrator can configure workflows in Workfront, then assign them to Project Templates. When a Project is created using a Project Template to which a workflow is assigned, the actions defined in the workflow are triggered. 

>[!NOTE]
>
>Workflows are available only in an Adobe Experience Manager as a Cloud Service integration. They are not available in integrations with Adobe Experience Manager Assets Essentials.


## Access requirements

You must have the following:

<table>
  <tr>
   <td><strong>Adobe Workfront plan*</strong>
   </td>
   <td>Any
   </td>
  </tr>
  <tr>
   <td><strong>Adobe Workfront licenses*</strong>
   </td>
   <td>Request or higher
   </td>
  </tr>
  <tr>
   <td><strong>Product</strong>
   </td>
   <td><p>You must have Experience Manager Assets as a Cloud Service or Assets Essentials, and you must be added to the product as a user in the Admin Console.</p><p>You must have write access to the repository in Adobe Experience Manager.</p>
   </td>
  </tr>
  <tr>
   <td><strong>Access level configurations*</strong>
   </td>
   <td>Edit access to Documents
<p>
<strong>Note: </strong>If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <strong>Create or modify custom access levels</strong>.
   </td>
  </tr>
  <tr>
   <td><strong>Object permissions</strong>
   </td>
   <td>Manage access or higher on the project 
<p>
For information on requesting additional access, see <strong>Request access to objects </strong>.
   </td>
  </tr>
</table>

## Prerequisites

Before you begin,

* Your Workfront administrator must configure workflows in an Adobe Experience Manager integration. For more information, see [Configure the Experience Manager Assets as a Cloud Service integration](../../administration-and-setup/configure-integrations/configure-aacs-integration.md#set-up-workflows-optional).

## Add a workflow to a template 

You can add a workflow to a project template. The workflow will be applied to any projects created from the template.

1. Open a template by clicking **Templates** in the Main Menu, then selecting the template from the list.
1. Click **Experience Manager Assets** in the left navigation panel.

   >[!NOTE]
   >
   >If the Experience Manager Assets section is not visible in the left navigation, your Workfront administrator has not enabled workflows for your organization. <!--Is this right?-->

1. In the **Select an integration for automated workflows field**, select the integration with the workflows you want to use for projects created from this template.
1. (Optional) Edit any workflow values that you want to apply to projects created from this template. 

   For instructions on specific workflows, see [Edit workflow values in a project](#edit-workflow-values-in-a-project) in this article.

   Only workflows that have been activated in the Experience Manager area of Setup are available in templates or projects.

1. Your changes save automatically. <!-- do they though??-->

## Add a workflow to a project

You can add a workflow when creating a project, or add a workflow to an existing project. In both cases, you will use a project template to add the workflow.

### Add a workflow when creating a project

1. Begin creating a project.

   For instructions, see [Create a project using a template](/help/quicksilver/manage-work/projects/create-projects/create-project-from-template.md).

1. When selecting a template for the project, select the template that contains the workflows you want to use for this project.
1. (Optional) Edit any workflow values for the project, as described in [Edit workflow values in a project](#edit-workflow-values-in-a-project).

   Only workflows that have been activated in the Experience Manager area of Setup are available in templates or projects.


### Add a workflow to an existing project

In the production environment:

1. Begin adding a template to the project.

   For instructions, see [Attach a template to a project](/help/quicksilver/manage-work/projects/create-and-manage-templates/attach-template-to-project.md).

1. When selecting a template for the project, select the template that contains the workflows you want to use for this project.
1. (Optional) Edit any workflow values for the project, as described in [Edit workflow values in a project](#edit-workflow-values-in-a-project).

   Only workflows that have been activated in the Experience Manager area of Setup are available in templates or projects.

In the Preview Sandbox environment:

<div class="preview">

1. Toggle the **[!UICONTROL Create Linked folder]** on or off as desired. If you toggle it on, you can then configure the following steps.
1. Enter a name for the linked folder that you are creating. If you are creating a folder tree, this is the name of the root folder.
1. (Conditional) Enable the **Default folder tree** option if you want this linked folder to be the default folder for projects created with templates that use this integration.
1. Choose a folder path to indicate where you want all linked folders associated with this integration.
1. (Conditional) To add a folder tree (nested folders) to this integration, do the following:

   1. Click the **Add folder** icon ![Add folder](assets/add-folder-aem.png).
   1. In the Name type field, select how you want to name the folder:

      * **Name**: Type in a name for the folder.
      * **Object data**: Select the source for the folder name, such as Project name.
      * **Custom form data**: Select the custom form data to use as the folder name.

      >[!NOTE]
      >
      >* Folder names must be fewer than 100 characters.
      >* The following characters will be removed from folder names:

   1. To add a nested folder to the folder tree, click the three-dot menu next to the folder you want to create a nested folder in and select **Add Folder**. Fill in the fields as described in Step the previous step.
   1. To link a folder to Workfront, select the folder and click the **Make linked folder**   icon ![Link folder](assets/link-folder.png).
   1. (Optional) To edit a folder, select the folder and click the **Edit Folder** icon ![Edit icon](assets/edit-icon.png).
   1. (Optional) To delete a folder, select the folder and click the **Delete Folder** icon ![Delete folder](assets/delete-folder.png).
1. (Conditional) To add another folder tree, click + Add folder tree and follow the steps in Step 5.

   >[!NOTE]
   >
   >This integration will create no more than 100 folders, regardless of how many folder trees are created. For example, an integration with 4 folder trees can create up to 100 folders, not 400 folders.
1. Click **[!UICONTROL Save]**, or move on to the [Publish assets that are sent to Adobe Experience Manager Assets](#publish-assets-that-are-sent-to-adobe-experience-manager-assets) section in this article.

</div>

### Edit workflow values in a project

You can edit workflow values on the project level. Project-level workflow values override values set on the project template, which override the default values set in the Adobe Experience Manager Assets integration.

All workflow values can be found in:

* The Workflows section of the Create project or Edit project window.
* The Adobe Experience Manager section of the left navigation.


   >[!NOTE]
   >
   >If these areas are not visible, your Workfront administrator has not enabled Workflows for your organization.

#### Linked folders

To edit the workflow for linked folders:

1. Toggle **[!UICONTROL Create Linked folder]** on or off as desired.
1. (Conditional) If you are enabling linked folders, choose a folder path to indicate where you want all linked folders associated with this integration. 
1. Click **[!UICONTROL Save]** if you are using the [!UICONTROL Create Project] or [!UICONTROL Edit project] window.
    
   Or

   If you are in the [!DNL Adobe Experience Manager area], your changes save automatically. <!--Do they though?-->


#### Publishing assets

To edit the workflow for publishing assets:

1. Toggle **Publish assets automatically** on or off as desired.
1. (Conditional) If you are enabling publishing, select whether you want to publish  to the publish service, the brand portal, or both.
1. Click **[!UICONTROL Save]** if you are using the [!UICONTROL Create Project] or [!UICONTROL Edit project] window.
    
   Or

   If you are in the [!DNL Adobe Experience Manager area], your changes save automatically. <!--Do they though?-->


