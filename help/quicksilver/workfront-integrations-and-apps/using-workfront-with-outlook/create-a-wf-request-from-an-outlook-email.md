---
product-area: workfront-integrations;projects
navigation-topic: workfront-for-outlook
title: Create an [!DNL Adobe Workfront] request from an Outlook email
description: You can create a [!DNL Adobe Workfront] request from an email in Outlook.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 4ecfe632-5f2e-4dc2-8c88-6a8229887f53
---
# Create an [!DNL Adobe Workfront] request from an [!UICONTROL Outlook] email

>[!IMPORTANT]
>
>[Microsoft is in the process of disabling support for legacy Exchange online tokens](https://learn.microsoft.com/en-us/office/dev/add-ins/outlook/faq-nested-app-auth-outlook-legacy-tokens), which are currently used by the Workfront Outlook add-in for authentication. This change by Microsoft has already started affecting customers and will continue to roll out in phases through October 2025.
>
>* **After Microsoft fully disables these tokens, the Workfront for Microsoft Outlook integration will no longer function.** 
>
>As part of this change, Microsoft has made the decision to change the way tokens are re-enabled. After **June 30, 2025**, admins will no longer be able to re-enable tokens themselves—only Microsoft Support can grant exceptions. **On October 1, 2025, legacy tokens will be turned off for all tenants. Exceptions will not be granted.**  

You can create a [!DNL Adobe Workfront] request from an email in Outlook.

When you create a [!DNL Workfront] request based on an email, the content of the email (including the subject and body) are included in the request by default.

>[!NOTE]
>
>You can not create a [!DNL Workfront] request from a shared [!UICONTROL Outlook] mailbox.

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

## Create a request from an [!DNL Outlook] email

To create a [!DNL Workfront] Request from [!DNL Outlook]:

1. Select the email that contains the information you want to include in a [!DNL Workfront] request. 
1. Click the **[!DNL Workfront]** icon in the upper-right corner of the email message to display the Workfront add-in.\
   You might need to click the down-pointing arrow in the upper right of your email to access the [!DNL Workfront] icon.

1. Click the **[!UICONTROL Menu]** icon ![o365_addin_menu2_icon.png](assets/o365-addin-menu2-icon.png) to display the list of available [!DNL Workfront] options.

1. Click **[!UICONTROL Submit Request]**.
1. In the **[!UICONTROL Select a Request Type]** field, select the request queue where you want to submit the request.

1. Specify the following information:\
   Depending on how the request queue was set up, available fields might vary. For a complete list and description of possible fields, see [Create and submit [!DNL Adobe Workfront] requests](../../manage-work/requests/create-requests/create-submit-requests.md) article.

   * **[!UICONTROL Subject]:** Specify a subject for the request. By default, the email subject is used.
   * **[!UICONTROL Description]:** Specify a description for the request. By default, the email body is used.
   * **[!UICONTROL Documents]:** Attach any documents that you want to include in the request. You can attach documents via drag and drop, or by clicking **[!UICONTROL Select File]** and browsing to and selecting the document.\

      By default, any documents attached to the email are included in the request.

1. Click **[!UICONTROL Submit Request]**.\
   The Request is submitted to [!DNL Workfront], in the specified request queue. 

1. (Optional) Navigate back to [!DNL Outlook], and select the original email.\
   At the top of the [!DNL Workfront] add-in panel, notice the confirmation with a link that the email was added to Workfront as a request. The link includes the date on which it was converted.\
