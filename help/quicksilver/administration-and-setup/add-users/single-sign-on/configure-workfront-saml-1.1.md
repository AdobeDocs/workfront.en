---
user-type: administrator
product-area: system-administration;setup
navigation-topic: single-sign-on-in-workfront
title: Configure Adobe Workfront with SAML 1.1
description: You can configure Workfront for use with SAML 1.1.
author: Becky, Caroline
feature: System Setup and Administration
role: Admin
exl-id: 0ae4f59f-6e19-4b44-ba3d-3dfd87a5815d
---
# Configure Adobe Workfront with SAML 1.1

<!--
DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.</p>
-->

{{important-admin-console-onboard}}

You can use SAML 1.1 with Adobe Workfront.

## Access requirements

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

## SAML 1.1 single sign-on solution

As a Workfront administrator, you can integrate Workfront with SAML 1.1.

Unlike other single sign-on solutions, auto-provisioning users and attribute-mapping are not available for Federated SSO configuration, including SAML 1.1.

## Configure the SAML 1.1 server to communicate with Workfront

In order to have home page landing preferences honored when implementing a Federated ID (SAML) SSO environment, you need to make sure the federated server is set up to point to `https://[Assigned Company Sub-domain].Workfront-ondemand.com/Workfront/.`

## Configure Workfront with SAML 1.1

1. Click the **Main Menu** icon ![](assets/main-menu-icon.png) in the upper-right corner of Adobe Workfront, then click **Setup** ![](assets/gear-icon-settings.png).

1. Click **System** > **Single Sign-On (SSO)**.

1. In the **Type** drop-down list, select **SAML 1.1**.
1. Specify the following information:

   * **Issuer**: Specify the domain provider obtained from your SAML service provider. It is possible to provide the port instead, for example: **example.company.com:80** 
   
   * **Login Portal URL**: Specify the login URL used to log in to all your SSO-enabled applications, including Workfront.  
   
   * **Sign-out URL**: Specify the URL displayed after users log out of Workfront.  
   
   * **Change password URL**: Specify the URL where users will be directed if they need to change their password.   
     Since users maintain one password across multiple platforms when integrated with SAML 1.1, it is important that they are directed to a central location to change their password rather than being allowed to change their password in Workfront.  
   
   * **Certificate**: Upload a valid certificate for authentication of a secure connection. OnDemand clients are required to do this. The certificate is obtained from your SAML 1.1 system administrator.  
   
   * **Admin Exemption**: When this box is checked, Workfront will attempt to first login through SAML for users with System Administrator Access Level. If authentication fails, Workfront will use local authentication for administrators. We recommend that you always have this option selected, to provide your Workfront administrator a way for logging into Workfront in the event that your SAML 1.1 provider is temporarily unavailable.  
   
   * **Enable**: Select this option to enable the integration with SAML 1.1. If it is not selected, SAML 1.1 will not be activated.

1. Click **Save**.
