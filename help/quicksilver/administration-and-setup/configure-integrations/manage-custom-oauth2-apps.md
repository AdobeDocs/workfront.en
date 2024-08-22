---
user-type: administrator
product-area: system-administration;workfront-integrations
navigation-topic: administrator-integrations
title: View and Manage Custom OAuth2 Applications
description: As an Adobe Workfront administrator, you can view and manage the OAuth2 applications for your instance of Workfront, which allow other applications to access Workfront.
feature: System Setup and Administration, Workfront Integrations and Apps
role: Admin
author: Becky
exl-id: 158430e5-8857-4bd8-86a6-2ba106b1638c
---
# View and manage custom OAuth2 applications

As an [!DNL Adobe Workfront] administrator, you can view and manage the OAuth2 applications for your instance of [!DNL Workfront], which allow other applications to access [!UICONTROL Workfront].

>[!NOTE]
>
>* In the context of OAuth2, "Oauth2 application" refers to this sort of access link between an app and a server such as [!DNL Workfront]. For more information, see [Create OAuth2 applications for [!DNL Workfront] integrations](../../administration-and-setup/configure-integrations/create-oauth-application.md)
>* You can have up to a total of ten OAuth2 Applications at one time.

* For information on creating custom OAuth2 applications, see [Create OAuth2 applications for [!DNL Workfront] integrations](../../administration-and-setup/configure-integrations/create-oauth-application.md)
* For instructions on configuring and using the OAuth2 application with user credentials (authorization code flow), see [Configure and use your organization's custom OAuth 2 applications using authorization code flow](../../wf-api/api/oauth-app-code-token-flow.md).
* For instructions on configuring and using the OAuth2 application using server authentication (JWT flow), see [Configure and use your organization's custom OAuth 2 applications using JWT flow](../../wf-api/api/oauth-app-jwt-flow.md).
* For instructions on configuring and using the OAuth2 application using PKCE, see [Configure and use your organization's custom OAuth 2 applications using PKCE flow](../../wf-api/api/oauth-app-pkce-flow.md).

## Access requirements

+++ Expand to view access requirements for the functionality in this article.

You must have the following access to perform the steps in this article:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan*</td> 
   <td> <p>[!DNL Pro] or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] license*</td> 
   <td> <p>[!UICONTROL Plan] or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> You must be a [!DNL Workfront] administrator. </p>
    <p>For information on [!DNL Workfront] administrators, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Grant a user full administrative access</a>.</p>
     </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your [!DNL Workfront] administrator.

+++

## Prerequisites

You must create [!UICONTROL OAuth2] applications for your organization before you can view or manage them.

For more information, see [Create OAuth2 applications for [!DNL Workfront] integrations](../../administration-and-setup/configure-integrations/create-oauth-application.md)

## Manage custom OAuth2 applications

* [View and edit custom OAuth2 applications](#view-and-edit-custom-oauth2-applications)
* [Delete custom OAuth2 applications](#delete-custom-oauth2-applications)

### View and edit custom OAuth2 applications {#view-and-edit-custom-oauth2-applications}

{{step-1-to-setup}}

1. In the left navigation panel, click **[!UICONTROL System]**, then select **[!UICONTROL OAuth Applications]**.
1. Click **[!UICONTROL Create app integration]**.
1. Hover over the application and click **[!UICONTROL Edit]** ![](assets/edit-icon.png) when it appears on the far right.
1. (Optional) Edit any details of the application.

   For fields related to OAuth2 and JWT apps, see [Create OAuth2 applications for [!DNL Workfront] integrations](../../administration-and-setup/configure-integrations/create-oauth-application.md).

### Delete custom OAuth2 applications {#delete-custom-oauth2-applications}

{{step-1-to-setup}}

1. In the left navigation panel, click **[!UICONTROL System]**, then select **[!UICONTROL OAuth Applications]**.
1. Click **  **.
1. Hover over the application and click **[!UICONTROL Delete]** ![](assets/delete.png) when it appears on the far right.

## Manage Client Secrets in OAuth2 applications

* [View Client Secret details](#view-client-secret-details)
* [Add or edit notes for Client Secret](#add-or-edit-notes-for-client-secret)
* [Delete Client Secret](#delete-client-secret)

### View Client Secret details {#view-client-secret-details}

>[!IMPORTANT]
>
>You cannot view the Client Secret itself. If you have lost your Client Secret, you must delete it and create a new one.
>
>* To delete a Client Secret, see [Delete Client Secret](#delete-client-secret) in this article.
>* To create a new Client Secret, see [Create an OAuth2 application](../../administration-and-setup/configure-integrations/create-oauth-application.md#create) in [Create OAuth2 applications for [!DNL Workfront] integrations](../../administration-and-setup/configure-integrations/create-oauth-application.md).
>

{{step-1-to-setup}}

1. In the left navigation panel, click **[!UICONTROL System]**, then select **[!UICONTROL OAuth Applications]**.
1. Hover over the application and click the **[!UICONTROL Edit]** icon when it appears on the far right.
1. View details in the Client Secret area:

   * Created date
   * Last used date
   * Notes

      To add notes to a Client Secret, see [Add or edit notes for Client Secret](#add-or-edit-notes-for-client-secret).

### Add or edit notes for Client Secret {#add-or-edit-notes-for-client-secret}

{{step-1-to-setup}}

1. In the left navigation panel, click **[!UICONTROL System]**, then select **[!UICONTROL OAuth Applications]**.
1. Click **[!UICONTROL Create app integration]**.
1. Hover over the application and click the **[!UICONTROL Edit]** icon when it appears on the far right.
1. Locate the Client Secret that you want to add or edit a note for.
1. Click the box that contains details for the Client Secret.

   You can now add note text, or edit existing note text.

   >[!NOTE]
   >
   >Note text has a maximum of 64 characters.

1. Click out of the box or press **[!UICONTROL Enter]** to save the note text.

### Delete Client Secret {#delete-client-secret}

{{step-1-to-setup}}

1. In the left navigation panel, click **[!UICONTROL System]**, then select **[!UICONTROL OAuth Applications]**.
1. Click **[!UICONTROL Create app integration]**.
1. Hover over the application and click the **[!UICONTROL Edit]** icon when it appears on the far right.
1. Locate the Client Secret that you want to delete.
1. Click the **[!UICONTROL Delete]** icon ![](assets/delete.png) next to the Client Secret.
