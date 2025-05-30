---
product-area: workfront-integrations
navigation-topic: workfront-for-outlook
title: Permissions levels for [!DNL Workfront] for Outlook
description: The [!DNL Workfront for Outlook] add-in requires Read/write mailbox access. The [!DNL Workfront for Outlook] integration requires the highest level permissions because it has the functionality to download email attachments from the Outlook exchange server and upload them to [!DNL Workfront], when the user submits a Request from an email that has attachments.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 704da044-21ed-4ca1-be6f-0e0aa832e069
---
# Permissions levels for [!DNL Workfront for Outlook]

>[!NOTE]
>
>Microsoft is in the process of disabling support for legacy Exchange Online tokens, which are used by this integration. A new Microsoft Office 365 integration will be available in September 2025, which will not use legacy Exchange Online tokens. 
>
>In the meantime, we highly recommend renewing your legacy Exchange Online token:
>
>* Before June 30, 2025: Your Microsoft administrator can renew your legacy Exchange Online token.
>* After June 30, 2025, you must contact Microsoft Support to renew your legacy Exchange Online token. 


[!DNL Workfront for Outlook] requires the highest of the four levels of permissions allowed in [!DNL Outlook] add-ins.

For details regarding permissions in [!DNL Outlook] add-ins, see [Privacy, permissions and security for [!DNL Outlook] add-ins](https://docs.microsoft.com/en-us/office/dev/add-ins/outlook/privacy-and-security) in the [!DNL Microsoft] documentation.

The [!DNL Workfront for Outlook] add-in requires Read/write mailbox access (`ReadWriteMailbox`), which is the highest permission scope.
The [!DNL Workfront for Outlook] integration requires the highest level permissions because it has the functionality to download email attachments from the [!DNL Outlook] exchange server and upload them to [!DNL Workfront], when the user submits a Request from an email that has attachments. For this functionality to work, [!DNL Workfront for Outlook] uses the function `mailbox.getCallbackTokenAsync()` from [!DNL Office] Add-in JavaScript API to get the Token and use that to download email attachments from the exchange server. The only permission that allows use of that function is `ReadWriteMailbox`. For more information, see [Privacy, permissions and security for Outlook add-ins](https://docs.microsoft.com/en-us/office/dev/add-ins/outlook/privacy-and-security) in the Microsoft documentation.

The [!DNL Workfront for Outlook] add-in also requires `ReadWriteItem` permission (included in `ReadWriteMailbox`), which is used to read the email body and read/update email metadata:

* Read email body:

   [!DNL Workfront for Outlook] reads the email body when a user submits the request or sends the email body as an update to [!DNL Adobe Workfront] Object.
* Read/Update email metadata:

   [!DNL Workfront for Outlook] updates email headers when a user submits a request from an email. This is done to store information about the submitted [!DNL Adobe Workfront] object, so the next time the user opens the add-in for the same email the information about previous actions with that email are shown.

[!DNL Workfront for Outlook] accesses a user's Mailbox only when the user performs an action within the add-on. It does not have any background functionality. Workfront for Outlook accesses the user's mailbox in the following scenario only:

* The user attempts to submit a request, create a task, or send an email as an update from [!DNL Workfront for Outlook] (Opening the add-in and selecting an action)
    * [!DNL Workfront for Outlook] reads the email body to populate in the form inside the add-in.
    * [!DNL Workfront for Outlook] reads email metadata to display information on the add-in about the previous actions done in the add-in with the same email.
* When a user submits a request, creates a task, or sends an email as an update from [!DNL Workfront for Outlook] (clicking the [!UICONTROL submit] button on the add-in):
    * [!DNL Workfront for Outlook] reads the email body to send it to  Workfront as a request description or a comment.
    * [!DNL Workfront for Outlook] updates the email metadata to store information about the submitted requests or updated object.
    * [!DNL Workfront for Outlook] downloads email attachments from the exchange server to upload to submitted requests, created tasks, or updated objects.
