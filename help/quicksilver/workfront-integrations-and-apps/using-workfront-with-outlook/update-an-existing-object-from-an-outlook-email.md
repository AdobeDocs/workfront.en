---
product-area: workfront-integrations;projects
navigation-topic: workfront-for-outlook
title: Update an existing object from an Outlook email
description: You can update an existing project, task, or issue with information from an Outlook email.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 297eb1c4-ee9f-4bb3-a412-18f23c74b0eb
---
# Update an existing object from an [!DNL Outlook] email

>[!IMPORTANT]
>
>[Microsoft is in the process of disabling support for legacy Exchange online tokens](https://learn.microsoft.com/en-us/office/dev/add-ins/outlook/faq-nested-app-auth-outlook-legacy-tokens), which are currently used by the Workfront Outlook add-in for authentication. This change by Microsoft has already started affecting customers and will continue to roll out in phases through October 2025.
>
>* **After Microsoft fully disables these tokens, the Workfront for Microsoft Outlook integration will no longer function.** 
>
>As part of this change, Microsoft has made the decision to change the way tokens are re-enabled. After **June 30, 2025**, admins will no longer be able to re-enable tokens themselves—only Microsoft Support can grant exceptions. **On October 1, 2025, legacy tokens will be turned off for all tenants. Exceptions will not be granted.**  

You can update an existing project, task, or issue with information from an [!DNL Outlook] email.



## Access requirements

+++ Expand to view access requirements for the functionality in this article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront package</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license</td> 
   <td> <p>Standard</p>
   <p>Work or higher</p> </td> 
  </tr> 
 </tbody> 
</table>

For information, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md). 

+++

## Prerequisites

Your [!DNL Workfront] administrator must enable [!DNL Outlook for Office] with [!DNL Workfront] before you can use this integration.

## Update an existing object from an [!DNL Outlook] email

1. In [!DNL Outlook], select the email that contains the information that you want to include in an [!DNL Adobe Workfront update]. 
1. Click the **[!DNL Workfront]** icon in the upper-right corner of the email message to display the Workfront add-in.\
   You might need to click the down-pointing arrow in the upper right of your email to access the [!DNL Workfront] icon.

1. Click the **[!UICONTROL Menu]** icon ![o365_addin_menu_icon.png](assets/o365-addin-menu2-icon.png) to display the list of available [!DNL Workfront] options.\
   

1. Click **[!UICONTROL Update] in Workfront**.\
   You can update the following information from the email before it is saved as a task:

   * **[!UICONTROL Type]**: Select the type of object you are updating. You can select **[!UICONTROL Project]**, **[!UICONTROL Task]**, or **[!UICONTROL Issue]**. The object you select determines the results that display in the **[!UICONTROL Name]** field below. If you are unsure of the type of object, select **[!UICONTROL All]** to search for projects, tasks, and issues simultaneously.

   * **[!UICONTROL Name]**: Begin typing the name of the project, task, or issue that you want to update. Click the name when it appears in the drop-down list.
   * **[!UICONTROL Update]**: By default, the update is the same as the email Body. You can modify the update as desired.\

      This [!UICONTROL update] is displayed as the update status in Workfront.

   * **[!UICONTROL Attachments]**: Any email attachments are saved to the [!UICONTROL Documents] area of the task. You can delete any attachments before submitting the update.

1. (Optional) Click **[!UICONTROL Include Others]**, begin typing the name of users who you want to include in the update, then click the name when it appears in the drop-down list.\
   Repeat this process to include additional users, then click **[!UICONTROL Done]**.\
   By default, the user you are replying to receives a notification regardless of whether you include them.\

1. (Optional) Click the **[!UICONTROL Lock]** icon to restrict this update to users within your company. When the update is locked, users outside your company cannot see the update.

   * **[!UICONTROL Unlocked]:** Any user with access to the project, task, or issue where the update resides can view the update.\

      By default, the update is unlocked.\
      ![o365_addin_unlock.png](assets/o365-addin-unlock.png)

   * **[!UICONTROL Locked]:** Only users within your company can view the update.\

      ![o365_addin_lock.png](assets/o365-addin-lock.png)

1. Click **[!UICONTROL Update]**.
1. (Optional) Click **[!UICONTROL View in Workfront]** to view the updated item with the [!DNL Workfront] integration within [!UICONTROL Outlook].
