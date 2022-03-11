---
filename: configure-workfront-saml-1.1
user-type: administrator
product-area: system-administration;setup
navigation-topic: single-sign-on-in-workfront
title: Configure Adobe Workfront with SAML 1.1
description: The procedure described on this page applies only to organizations that are not yet onboarded to the Adobe Admin Console.
---

# Configure `Adobe Workfront` with SAML 1.1

>[!IMPORTANT]
>
>The procedure described on this page applies only to organizations that are not yet onboarded to the Adobe Admin Console.
>
>If your organization has been onboarded to the Adobe Admin Console, see [Platform-based administration differences (Adobe Workfront/Adobe Business Platform)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

>[!IMPORTANT]
>
>Security Assertion Markup Language (SAML) 1.1 is now supported only in a limited capacity as a single sign-on (SSO) option; it will be removed from the product in 2020. We recommend moving to SAML 2.0. For more information, see [Configure Adobe Workfront with SAML 2.0](../../../administration-and-setup/add-users/single-sign-on/configure-workfront-saml-2.md).

The following sections provide information about using SAML 1.1 with `Adobe Workfront`.

## Access requirements

You must have the following to perform the steps in this article:

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><span>Adobe Workfront</span> plan</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><span>Adobe Workfront</span> license</td> 
   <td> <p><span>Plan</span> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>You must be a <span>Workfront administrator</span>. For more information, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Grant a user full administrative access</a>.</p> <p>Note: If you still don't have access, ask your <span>Workfront administrator</span> if they set additional restrictions in your access level. For information on how a <span>Workfront administrator</span> can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## SAML 1.1 single sign-on solution

As a `Workfront administrator`, you can integrate `Workfront` with SAML 1.1.

Unlike other single sign-on solutions, auto-provisioning users and attribute-mapping are not available for Federated SSO configuration, including SAML 1.1.

## Configure the SAML 1.1 server to communicate with `Workfront`

In order to have home page landing preferences honored when implementing a Federated ID (SAML) SSO environment, you need to make sure the federated server is set up to point to *https://[Assigned Company Sub-domain]. `Workfront`-ondemand.com/ `Workfront`/.*

## Configure `Workfront` with SAML 1.1

<ol> 
 <li value="1">Click the <span class="bold">Main Menu</span> icon <img src="assets/main-menu-icon.png"> in the upper-right corner of <span>Adobe Workfront</span>, then click <span class="bold">Setup</span> <img src="assets/gear-icon-settings.png">.</li> 
 <li value="2">Click <span class="bold">System</span> > <span class="bold">Single Sign-On (SSO)</span>.</li> 
 <li value="3"> <p>In the <span class="bold">Type</span> drop-down list, select <span class="bold">SAML 1.1</span>.</p> </li> 
 <li value="4"> <p>Specify the following information:</p> 
  <ul> 
   <li><span class="bold">Issuer</span>: Specify the domain provider obtained from your SAML service provider. It is possible to provide the port instead, for example: <span class="bold">example.company.com:80</span><br></li> 
   <li><span class="bold">Login Portal URL</span>: Specify the login URL used to log in to all your SSO-enabled applications, including <span>Workfront</span>.<br></li> 
   <li><span class="bold">Sign-out URL</span>: Specify the URL displayed after users log out of <span>Workfront</span>.<br></li> 
   <li><span class="bold">Change password URL</span>: Specify the URL where users will be directed if they need to change their password. <br>Since users maintain one password across multiple platforms when integrated with SAML 1.1, it is important that they are directed to a central location to change their password rather than being allowed to change their password in <span>Workfront</span>.<br></li> 
   <li><span class="bold">Certificate</span>: Upload a valid certificate for authentication of a secure connection. OnDemand clients are required to do this. The certificate is obtained from your SAML 1.1 system administrator.<br></li> 
   <li><span class="bold">Admin Exemption</span>: When this box is checked, <span>Workfront</span> will attempt to first login through SAML for users with System Administrator Access Level. If authentication fails, <span>Workfront</span> will use local authentication for administrators. We recommend that you always have this option selected, to provide your <span>Workfront administrator</span> a way for logging into <span>Workfront</span> in the event that your SAML 1.1 provider is temporarily unavailable.<br></li> 
   <li><span class="bold">Enable</span>: Select this option to enable the integration with SAML 1.1. If it is not selected, SAML 1.1 will not be activated. </li> 
  </ul> </li> 
 <li value="5">Click <span class="bold">Save</span>. </li> 
</ol>

