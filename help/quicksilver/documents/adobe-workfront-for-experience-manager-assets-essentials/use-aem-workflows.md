---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: Use workflows in the Experience Manager Assets Essentials integration
description: Use workflows in the Experience Manager Assets Essentials integration
author: Courtney, Becky
feature: Digital Content and Documents, Workfront Integrations and Apps
---
# Use workflows in the Experience Manager Assets integration

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
   <td><p>You must have Experience Manager Assets as a Cloud Service or Assets Essentials, and you must be added to the product as a user in the Admin Console.</p><p>You must have write access to the repository in Adobe Experience Manager to create linked folders.</p>>
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

* Your Workfront Administrator must configure Workflows in an Adobe Experience Manager integration. For more information, see [Configure the Experience Manager Assets as a Cloud Service integration](help\quicksilver\administration-and-setup\configure-integrations\configure-aacs-integration.md).

## Add a workflow to a template

You can add a workflow to a template. The workflow will be applied to any projects created from the template.

1. <!-- main menu snippet??--> Open a template by clicking Templates in the Main Menu, then selecting the template from the list.
1. Click **Experience Manager Assets** in the left navigation panel.

   >[!NOTE]
   >
   >If the Experience Manager Assets section is not visible in the left navigation, your Workfront administrator has not enabled Workflows for your organization.

1. In the **Select an integration for automated workflows field**, select the integration with the workflows you want to use for projects created from this template.
1. (Optional) Edit any workflow values that you want to apply to projects created from this template. 

   For example, to create a linked folder in a location other than the default value, enter the linked folder location.

1. Your changes save automatically. <!-- do they though??-->

## Add a workflow to a project

You can add a workflow when creating a project, or add a workflow to an existing project. In both cases, you will use a project template to add the workflow.

### Add a workflow when creating a project

1. Begin creating a project.

   For instructions, see [Create a project using a template](/help/quicksilver/manage-work/projects/create-projects/create-project-from-template.md).

1. When selecting a template for the project, select the template that contains the workflows you want to use for this project.
1. (Optional) Edit any workflow values for the project, as described in <!--X-->.

### Add a workflow to an existing project

1. Begin adding a template to the project.

   For instructions, see [Attach a template to a project](/help/quicksilver/manage-work/projects/create-and-manage-templates/attach-template-to-project.md).

1. When selecting a template for the project, select the template that contains the workflows you want to use for this project.
1. (Optional) Edit any workflow values for the project, as described in <!--X-->.

### Edit workflow values in a project

You can edit workflow values on the project level. Project-level workflow values override values set on the project template, which override the default values set in the Adobe Experience Manager Assets integration.

All workflow values can be found in:

* The Workflows section of the Create project or Edit project window.
* The Adobe Experience Manager section of the left navigation.

#### Linked folders

|Field|Instructions|
|---|---|
|

