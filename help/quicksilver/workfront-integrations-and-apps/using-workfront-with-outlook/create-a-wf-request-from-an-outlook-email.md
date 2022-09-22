---
product-area: workfront-integrations;projects
navigation-topic: workfront-for-outlook
title: Create an [!DNL Adobe Workfront] request from an Outlook email
description: You can create a [!DNL Adobe Workfront] request from an email in Outlook.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 4ecfe632-5f2e-4dc2-8c88-6a8229887f53
---
# Create an [!DNL Adobe Workfront] request from an Outlook email

You can create a [!DNL Adobe Workfront] request from an email in Outlook.

When you create a [!DNL Workfront] request based on an email, the&nbsp;content of the email (including the subject and body) are included in the request by default.

>[!NOTE]
>
>You can not create a [!DNL Workfront] request from a shared Outlook mailbox.

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
   <td> <p>Work, Plan</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your [!DNL Workfront] administrator.

## Prerequisites

Your [!DNL Workfront] administrator must enable [!DNL Outlook for Office] with [!DNL Workfront] before you can use this integration.

## Create a request from an Outlook email

To create a [!DNL Workfront] Request from Outlook:

1. Select the email that contains the information you want to include in&nbsp;a [!DNL Workfront] request.&nbsp;
1. Click the&nbsp;**[!DNL Workfront]**&nbsp;icon in the upper-right corner of the email message to display the Workfront add-in.\
   You might need to click the down-pointing arrow in the upper right of your email to access the [!DNL Workfront] icon.

1. Click the **Menu** icon to display the list of available [!DNL Workfront] options.

   ![o365_addin_menu2_icon.png](assets/o365-addin-menu2-icon.png)

1. Click **Submit Request**.
1. In the **[!UICONTROL Select a Request Type]** field, select the request queue where you want to submit the request.

   ![o365_addin_submitrequest.png](assets/o365-addin-submitrequest.png)

1. Specify the following information:\
   Depending on how the request queue was set up, available fields might vary. For a complete list and description of possible fields, see [Create and submit Adobe Workfront requests](../../manage-work/requests/create-requests/create-submit-requests.md) article.

   * **[!UICONTROL Subject]:** Specify a subject for the request. By default, the email subject is used.
   * **Description:** Specify a description for the request. By default, the email body is used.
   * **Documents:** Attach any documents that you want to include in the request. You can attach documents via drag and drop, or by clicking **[!UICONTROL Select File]** and browsing to and selecting the document.\

      By default, any documents attached to the email are included in the request.

1. Click **Submit Request**.\
   The Request is submitted to [!DNL Workfront], in the specified request queue.&nbsp;

1. (Optional) Navigate back to Outlook, and select the original email.\
   At the top of the [!DNL Workfront] add-in panel, notice the confirmation with a link that the email was added to Workfront as a request. The link includes the date on which it was converted.\
   ![outlook_submitted_as_a_request.png](assets/outlook-submitted-as-a-request-350x130.png)
