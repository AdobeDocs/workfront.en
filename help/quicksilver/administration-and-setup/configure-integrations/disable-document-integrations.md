---
title: Disable Document Integrations
user-type: administrator
product-area: system-administration;workfront-integrations
navigation-topic: administrator-integrations
description: As [!DNL anAdobe] [!DNL Workfront] administrator, you can disable the connection between Workfront and any of the third-party document providers.
feature: System Setup and Administration, Workfront Integrations and Apps, Digital Content and Documents
role: Admin
author: Courtney, Becky
exl-id: 78281bca-1fa1-4e78-96e5-70be12142bbd
---
# Disable document integrations

As an [!DNL Adobe] [!DNL Workfront] administrator, you can disable the connection between [!DNL Workfront] and any of the third-party document providers.

When you disable the connection between [!DNL Workfront] and a document provider, the links to the documents disappear from [!DNL Workfront]. Users can no longer see the linked documents, they cannot make any changes to the documents through the [!DNL Workfront] links, and they cannot add more documents to that provider.

## Access requirements

+++ Expand to view access requirements for the functionality in this article.

You must have the following to perform the steps in this article:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan</td> 
   <td>Any</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] license</td> 
   <td>[!UICONTROL Plan]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>You must be a [!DNL Workfront] administrator. For information on [!DNL Workfront] administrators, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Grant a user full administrative access</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your [!DNL Workfront] administrator.

+++

## Disable cloud provider integrations

To disable document integrations for [!UICONTROL Workfront DAM], [!DNL Box], [!DNL Dropbox], [!DNL Google Drive], [!DNL Microsoft OneDrive], [!DNL WebDAM]:

1. Log in to [!DNL Workfront] as a [!DNL Workfront] administrator.

{{step-1-to-setup}}

1. Click **[!UICONTROL Documents]** > **[!UICONTROL Cloud Providers]**.

1. Deselect any of the cloud providers you want to disconnect from [!DNL Workfront].
1. Click **[!UICONTROL Save]**.

   Users are not able to connect to the specific cloud provider you disabled, and they can no longer link documents from that cloud provider to Workfront.

## Disable the [!DNL SharePoint] integration

1. Log in to [!DNL Workfront] as a [!DNL Workfront] administrator.

{{step-1-to-setup}}

1. Expand **[!UICONTROL Documents]**, then click **[!UICONTROL [!DNL SharePoint] Integration]**.
1. Select the [!DNL SharePoint] integration you want to disable.
1. Click **[!UICONTROL Disable]**.\
   Users are not able to connect to the [!DNL SharePoint] site you disabled, and they can no longer link documents from [!DNL SharePoint] to [!DNL Workfront].

## Disable custom integrations

1. Log in to [!DNL Workfront] as the administrator.

{{step-1-to-setup}}

1. Click **[!UICONTROL Documents]** > **[!UICONTROL Custom Integration]**.
1. Select the custom integration you want to disable.
1. Click **[!UICONTROL Disable]**.

   Users are not able to connect to the third-party document provider you disabled, and they can no longer link documents from that cloud provider to [!DNL Workfront].
