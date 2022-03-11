---
filename: log-in-to-workfront
product-area: user-management
navigation-topic: manage-your-workfront-account
title: Log in to Adobe Workfront
description: You need the following information to log in to Adobe Workfront:
---

# Log in to Adobe Workfront

You need the following information to log in to Adobe Workfront:

* `A login URL:` This is your company's unique URL, which should have this format: `yourCompanyDomain.my.workfront.com`.  
  If you are set up for single sign-on (SSO), your URL might have been changed by your Workfront administrator. For more information about logging in to Workfront with SSO, see [Log in to Workfront with SSO](#logging-in-to-workfront-with-sso) in this article.

  The domain name for your company is established by Workfront. To change your domain name, contact our Customer Support team. For information about how to contact our Customer Support team, see [Contact Customer Support](../../../workfront-basics/tips-tricks-and-troubleshooting/contact-customer-support.md).

* `A username:` Your Workfront administrator sets up your user name.
* `A password:` If your system is not set up for SSO, you set up your Workfront password after receiving an email invitation from the Workfront administrator.

  For more information about logging in to Workfront with SSO, see [Log in to Workfront with SSO](#logging-in-to-workfront-with-sso) in this article.

  For more information about receiving email invitations and creating a Workfront password, see [Receive email invitations and create a password for Adobe Workfront](../../../workfront-basics/manage-your-account-and-profile/managing-your-workfront-account/receive-email-invitations.md).

## Access requirements

You must have the following access to perform the steps in this article:

<table cellspacing="0"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Request or higher</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan or license type you have, contact your Workfront administrator.

## Log in to Workfront without SSO

If your Workfront administrator did not set up Workfront to integrate with your SSO solution, you will need a new username and password for Workfront. For information about configuring Workfront to integrate with an SSO solution, see [Overview of single sign-on in Adobe Workfront](../../../administration-and-setup/add-users/single-sign-on/sso-in-workfront.md).

To log into Workfront using your Workfront username and password:

1. Open a browser window, then type in the unique URL of your company, which should have the following format: `yourCompanyDomain.my.workfront.com`.

   For more information about what browsers are supported for Workfront, see [Adobe Workfront browser requirements](../../../workfront-basics/workfront-browser-requirements.md).

1. In the login screen, enter your username and password.

   Your username is typically the email address associated with your Workfront account. If you forgot your password, see [Reset your password](../../../workfront-basics/manage-your-account-and-profile/managing-your-workfront-account/reset-your-password.md).

1. (Conditional) If your organization's Workfront login URL&nbsp;doesn't contain a domain, you must specify your domain in the Domain field.
1. Click `Login`.

## Log in to Workfront with SSO

If your Workfront administrator integrated Workfront with a single sign-on solution, you should contact them for the information needed for your logging in to Workfront. For more information about integrating Workfront with an SSO solution, see [Overview of single sign-on in Adobe Workfront](../../../administration-and-setup/add-users/single-sign-on/sso-in-workfront.md).

To log in to Workfront using your SSO&nbsp;username and password:

1. Open a browser window.

   For more information about what browsers are supported for Workfront, see [Adobe Workfront browser requirements](../../../workfront-basics/workfront-browser-requirements.md).

1. Type the unique URL of your company.

   If your Workfront administrator did not change the default Workfront URL, it should have the following format:

   `yourCompanyDomain.my.workfront.com` 

1. Your Workfront administrator can ensure that you have the correct URL.
1. On the login screen, enter your username and password.

   Your username and password are typically&nbsp;your network user name and password, which you use for all your applications. If you forgot your password or your user name, use the tools provided in your environment for resetting them, or contact your Workfront administrator.

   The look and feel of your login screen changes depending on what SSO solution you use and the way it was configured by your Workfront administrator.&nbsp;

1. Complete your login.

## Log in to the Workfront mobile app

<ol> 
 <li style="font-style: normal;" value="1"> <p>Launch the Workfront mobile app, then type your organization's domain.</p> <p>This is the SAML domain if your organization is using SSO.</p> <note type="tip">
   This is typically your company name. If you are unsure, contact your Workfront administrator.
  </note> </li> 
 <li style="font-style: normal;" value="2"> <p>Specify the Workfront URL for your company or the link to your SAML authentication portal.</p> <p>The Workfront URL should display in the following format<i>:</i><![CDATA[
               
                ]]><br style="font-style: normal;"><span class="bold">yourDomain.my.workfront.com</span></p> <p>For example:</p> <p><span class="bold">swains.my.workfront.com</span> </p> </li> 
 <li style="font-style: normal;" value="3"> <p>If you are logging in with you SAML credentials, follow the login steps from your SAML authentication portal.</p> <p> Your Workfront administrator must enable SAML 2.0 authentication with the Workfront web application in order to log in with your SAML credentials. For information about how to enable SAML 2.0, see the section <a href="../../../administration-and-setup/add-users/single-sign-on/configure-workfront-saml-2.md#saml-with-workfront-web-app" class="MCXref xref">Configure Adobe Workfront with SAML 2.0</a> in the article <a href="../../../administration-and-setup/add-users/single-sign-on/configure-workfront-saml-2.md" class="MCXref xref">Configure Adobe Workfront with SAML 2.0</a>. If you cannot log in as described in this section, contact your Workfront administrator.</p> </li> 
 <li value="4">Tap <span class="bold">Continue in browser</span>.</li> 
 <li value="5">Specify the <span class="bold">Username </span>of your Workfront account or SAML user.</li> 
 <li value="6">Specify the <span class="bold">Password</span> for your Workfront account or SAML user.</li> 
 <li value="7">(Optional) Tap the eye icon to display or hide your password.</li> 
 <li value="8"> <p>Tap <span class="bold">SIGN IN</span>.</p> <p>You are signed in.</p> </li> 
 <li value="9"> <p>Tap <span class="bold">Okay, got it</span> or <span class="bold">GETTING STARTED</span> to navigate through the tutorials displayed.</p> <p>These tutorials display only the first time you access the app. They display again only when you uninstall and reinstall the Workfront mobile app, or if you log in as another user. After closing out the tutorials, the area that displays is the one that you selected to show </p> </li> 
</ol>

