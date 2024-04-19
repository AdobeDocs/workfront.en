---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: Use Workfront Fusion to create a Workfront Project that has Adobe Experience Manager workflows
description: If you are creating a project through Workfront Fusion and want to include Adobe Experience Manager workflows on the project, you must use a specific Fusion module configuration, described in this article.
author: Becky
feature: Digital Content and Documents, Workfront Integrations and Apps, Workfront Fusion
---
# Use Workfront Fusion to convert a Workfront issue to a project that includes Adobe Experience Manager workflows

If you are creating a project through Workfront Fusion and want to include Adobe Experience Manager workflows on the project, you must use a specific Fusion module configuration, described in this article.

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
   <td><b>Adobe Experience Manager<b>:<ul><li><p>You must have Experience Manager Assets as a Cloud Service or Assets Essentials, and you must be added to the product as a user in the Admin Console.</p></li><li><p>You must have write access to the repository in Adobe Experience Manager.</p></li></ul>
  <b>Workfront Fusion</b>:<p>New:</p> <ul><li>[!UICONTROL Select] or [!UICONTROL Prime] [!DNL Workfront] Plan: Your organization must purchase [!DNL Adobe Workfront Fusion].</li><li>[!UICONTROL Ultimate] [!DNL Workfront] Plan: [!DNL Workfront Fusion] is included.</li></ul>   <p>Or</p>
   <p>Current: Your organization must purchase [!DNL Adobe Workfront Fusion].</p>
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
r
</table>

## Prerequisites

Before you begin,

* Your Workfront administrator must configure workflows in an Adobe Experience Manager integration. For more information, see [Configure the Experience Manager Assets as a Cloud Service integration](../../administration-and-setup/configure-integrations/configure-aacs-integration.md#set-up-workflows-optional).
* You must have a project template configured with an Adobe Experience Manager integration linked folder workflow.

<!--
* You must create an OAuth2 application in Workfront that -->

## Module configuration

In Workfront Fusion, if you want to create a project that includes Adobe Experience Manager workflows, you must use the Workfront > Misc Action module.

1. Add the **Workfront** > **Misc Action** module to your scenario.
1. In the **Connection** field, select the Workfront connection that connects to the account this module will use.
1. In the **Record Type** field, select `Issue`.
1. In the **ID** field, enter or map the ID of the issue that you are converting to a project.
1. Enable **Show advanced settings**.
1. Scroll to the bottom of the module and locate the **Project (Advanced Collection)** field.


```
{
    "aemNativeFolderTreeIDs": "Folder Tree ID here",
    "aemNativeFolderWorkflowEnabled": "true",
    "name": "New Project Name Here",
    "templateID": "Template ID here"
}
```


<!--
Things to mention:

How to configure
How to find folder path 
What all to put in the options
-->



