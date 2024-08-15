---
user-type: administrator
product-area: system-administration
navigation-topic: single-sign-on-in-workfront
title: Enable Outlook for Use with Workfront and SAML 2.0
description: If you enable SAML 2.0 authentication and you want your users to be able to log in to Workfront from Microsoft Outlook using their SAML 2.0 credentials, you must enable SAML 2.0 to authenticate in Office add-ins.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 8a55d364-962a-4eef-8968-b2233a71cf31
---
# Enable Outlook for use with Workfront and SAML 2.0

If you enable SAML 2.0 authentication and you want your users to be able to log in to Workfront from Microsoft Outlook using their SAML 2.0 credentials, you must enable SAML 2.0 to authenticate in Office add-ins.

>[!NOTE]
>
>This is not available if your organization's Workfront instance uses a custom SSO portal.>
><!--
>or is enabled with Adobe IMS>
>-->
>See your network or IT administrator if you need more information.

## Access requirements

+++ Expand to view access requirements for the functionality in this article.

You must have the following access to perform the steps in this article: 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan</td> 
   <td>Any</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license</td> 
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>You must be a Workfront administrator.</p> <p><b>NOTE</b>: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

## Enable Outlook for use with Workfront and SAML 2.0

{{step-1-to-setup}}

1. Click **System** > **Preferences**.

1. In the **Security** section, make sure that **Allow SAML 2.0 authentication in Office 365 add-ins**is enabled.

   This option enables embedding of Workfront in an Iframe only for Office 365 add-ins. This does not open a click-jacking breach as there is no clickable content involved.

   This option is enabled by default.

   >[!NOTE]
   >
   >If you enable the option **Allow embedding of Workfront in an iframe**, the option **Allow SAML 2.0 authentication in Office 365 add-ins** is dimmed and enabled.
   >
   >![](assets/if-you-enable.png)
   >

1. Click **Save**.

   The changes that you saved here affect the experience of all the users in Workfront.
