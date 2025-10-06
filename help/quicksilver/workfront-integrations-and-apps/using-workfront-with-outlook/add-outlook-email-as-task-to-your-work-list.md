---
product-area: workfront-integrations;projects
navigation-topic: workfront-for-outlook
title: Add an Outlook email as a task to your work list
description: You can convert [!DNL Outlook] emails to [!DNL Adobe Workfront] tasks. After an email is converted, the task is available in your Work List in the Home area.
author: Becky
feature: Workfront Integrations and Apps
exl-id: fcd02116-ffeb-43d3-8541-5e30e6cfdc5e
---
# Add an [!DNL Outlook] email as a task to your work list

>[!IMPORTANT]
>
>[Microsoft has disabled support for legacy Exchange online tokens](https://learn.microsoft.com/en-us/office/dev/add-ins/outlook/faq-nested-app-auth-outlook-legacy-tokens), which were used by the Workfront Outlook add-in for authentication. This change by Microsoft rolled out in phases and is complete as of October 1, 2025.
>
>**Because Microsoft has disabled these tokens, the Workfront for Microsoft Outlook integration no longer functions.** 

You can convert [!DNL Outlook] emails to [!DNL Adobe Workfront] tasks. After an email is converted, the task is available in your [!UICONTROL Work] List in the [!UICONTROL Home] area.

## Access requirements

You must have the following access to perform the steps in this article:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] license*</td> 
   <td> <p>[!UICONTROL Work], [!UICONTROL Plan]</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your [!DNL Workfront] administrator.

## Prerequisites

Your [!DNL Workfront] administrator must enable [!DNL Outlook for Office] with [!DNL Workfront] before you can use this integration.

## Add an [!DNL Outlook] email as a task to your work list

1. Select the email within [!DNL Outlook] that you want to convert to a task.
1. Click the **[!DNL Workfront]** icon in the upper-right corner of the email message to display the [!DNL Workfront] add-in.\
   You might need to click the down-pointing arrow in the upper right of your email to access the [!DNL Workfront] icon.

1. Click the **[!UICONTROL Menu]** ![o365_addin_menu_icon.png](assets/o365-addin-menu2-icon.png) icon to display the list of available [!DNL Workfront] options.\
   

1. Click **[!UICONTROL Add to Work]**.\

1. Deselect the **[!UICONTROL Add to Project]** field. 
1. (Optional) You can update the following information from the email before it is saved as a task:

   * **[!UICONTROL Task Name]:** By default, the task name is the same as the email Subject. You can modify the task name as desired.
   * **[!UICONTROL Description]:** By default, the description is the same as the email Body. You can modify the description as desired.
   * **[!UICONTROL Attachments]:** Any email attachments are saved to the [!UICONTROL Documents] area of the task. You can delete any attachments before saving the email as a task.

1. Click **[!UICONTROL Add]**.\
   The task is added to the [!UICONTROL Work List] in your Home area with no commit date.

1. (Optional) Click **[!UICONTROL View in Workfront]** to display the task within the [!DNL Workfront] application in a new tab.

1. (Optional) Navigate back to [!DNL Outlook], and select the original email.\
   At the top of the [!DNL Workfront] add-in panel, notice the confirmation with a link that the email was added to Workfront as a task. The link includes the date on which it was converted.\
