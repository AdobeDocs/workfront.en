---
filename: manage-api-keys
user-type: administrator
product-area: system-administration;user-management
navigation-topic: security
title: Manage API keys
description: In order to minimize API security vulnerabilities, Adobe Workfront administrators can manage the API Keys used to enable applications to access Workfront on behalf of a user.
---

# Manage API keys

In order to&nbsp;minimize API security vulnerabilities, *Adobe Workfront administrators* can manage the API Keys used to enable applications to access *Workfront*&nbsp;on behalf of a user.

You can reset or remove your current administrator API Key,&nbsp;configure API Keys to expire, and remove the API Keys for all users.

Examples of applications that leverage the&nbsp;*Workfront* API are:

* Document integrations such as Dropbox, Google Drive, and *Workfront DAM*
* *Workfront* mobile applications

>[!IMPORTANT]
>
>When resetting or removing an API Key, any application&nbsp;that&nbsp;leverages&nbsp;the *Workfront* API and authenticates to *Workfront* via this API Key&nbsp;must&nbsp;be re-configured in order to regain access to *Workfront*.

## Access requirements

You must have the following to perform the steps in this article:

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><em>Adobe Workfront</em> plan</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><em>Adobe Workfront</em> license</td> 
   <td> <p><em>Plan</em> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>You must be a <em>Workfront administrator</em>. For more information, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Grant a user full administrative access</a>.</p> <p>Note: If you still don't have access, ask your <em>Workfront administrator</em> if they set additional restrictions in your access level. For information on how a <em>Workfront administrator</em> can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## *Workfront* API Keys

Each user in *Workfront* has a unique&nbsp;API Key. This key&nbsp;is generated on a per-user basis at the time the user&nbsp;accesses an integration that leverages the *Workfront* API (such as the *Workfront* mobile app or a document integration).

>[!NOTE]
>
>&nbsp;API Keys you generate in the production environment are copied to your Preview environment during the weekly refresh. Any API Keys you generate in the Preview environment will be&nbsp;overwritten with your production API Keys during the weekly refresh.

*Workfront administrator*s also&nbsp;have a unique API Key.&nbsp;When an application uses an administrator API Key to access *Workfront*, the application has administrator access to *Workfront*.

## Manage an administrator API key

You can generate, reset, or remove the API Key for your administrator&nbsp;user account.&nbsp;

>[!NOTE]
>
>You can also generate an API Key through the API. For more information, see the [Event Subscription API](../../../wf-api/general/event-subs-api.md) section in [Event Subscription API](../../../wf-api/general/event-subs-api.md).

<ol> 
 <li value="1">Click the <span class="bold">Main Menu</span> icon <img src="assets/main-menu-icon.png"> in the upper-right corner of <em>Adobe Workfront</em>, then click <span class="bold">Setup</span> <img src="assets/gear-icon-settings.png">.&nbsp;</li> 
 <li value="2"> <p>Click <span class="bold">System ></span> <span class="bold">Customer Info.</span></p> </li> 
 <li value="3"> <p>(Conditional) Perform one of the following actions:</p> <p>To generate an API Key:&nbsp;In the <span class="bold">API Key Settings</span> section,&nbsp;click <span class="bold">Generate API Key</span>.</p> <p>Or<br>To reset an API Key: In the <span class="bold">API Key Settings</span> section, click&nbsp;<span class="bold">Reset</span>, then<span class="bold"> Reset.</span></p> <p>Or</p> <p>To remove the API Key: In&nbsp;the&nbsp;<span class="bold">API Key Settings</span> section,&nbsp;click <span class="bold">Remove</span>, then <span class="bold">Remove</span>.&nbsp;</p> </li> 
</ol>

## Generate an API Key for Non-Admin Users

You can generate and manage API Keys for users in roles other than *Workfront administrator*.

>[!NOTE]
>
>This is not available if your organization’s *Workfront* instance is enabled with Adobe IMS. See your network or IT administrator if you need more information.

<ol> 
 <li value="1">(Conditional) If your organization uses Single Sign-On (SSO) access management, temporarily disable the option requiring SSO authentication.<br>
  <ol>
   <li value="1">Click the <span class="bold">Main Menu</span> icon <img src="assets/main-menu-icon.png"> in the upper-right corner of <em>Adobe Workfront</em>, then click <span class="bold">Setup</span> <img src="assets/gear-icon-settings.png">.&nbsp;&nbsp;</li>
   <li value="2"><p>Expand <span class="bold">System</span>, then click <span class="bold">Single Sign-on (SSO)</span>.<br><img src="assets/sysadmin-security-sso-disable-31620-350x320.png" style="width: 350;height: 320;"><br></p></li>
   <li value="3"><p>Disable the checkbox requiring SSO authentication.</p><p>For example, if your organization uses SAML 2.0, disable <span class="bold">Only Allow SAML 2.0 Authentication</span>.</p></li>
  </ol></li> 
 <li value="2"> <p>In the address bar of a browser, enter the following API call:</p> <p><span class="bold"><domain></span>.my.workfront.com/attask/api/v7.0/user?action=generateApiKey&username=<span class="bold">username</span>&password=<span class="bold">password</span>&method=PUT</p> <p>Replace <domain> with your <em>Workfront</em> domain name, and username and password with the user's <em>Workfront</em> credentials.</p> </li> 
 <li value="3"> <p>(Conditional) Enable the option requiring SSO authentication if you disabled it in Step 1.</p> 
  <ol> 
   <li value="1">Click the <span class="bold">Main Menu</span> icon <img src="assets/main-menu-icon.png"> in the upper-right corner of <em>Adobe Workfront</em>, then click <span class="bold">Setup</span> <img src="assets/gear-icon-settings.png">.&nbsp;</li> 
   <li value="2">Expand <span class="bold">System</span>, then click <span class="bold">Single Sign-on (SSO)</span>.</li> 
   <li value="3">Select your SSO method in the <span class="bold">Type</span> drop down menu.</li> 
   <li value="4">Check the checkbox requiring SSO authentication.</li> 
  </ol> </li> 
</ol>

## Configure when API keys expire

You can configure API Keys to expire for all users in your system. When the API Key of a user expires, the user&nbsp;must re-authenticate to any applications that use the *Workfront* API to access *Workfront*. You can change the frequency with which the API Keys expire. You can also configure&nbsp;whether API Keys expire when the password of a user expires.

<ol> 
 <li value="1">Click the <span class="bold">Main Menu</span> icon <img src="assets/main-menu-icon.png"> in the upper-right corner of <em>Adobe Workfront</em>, then click <span class="bold">Setup</span> <img src="assets/gear-icon-settings.png">.&nbsp;&nbsp;<br></li> 
 <li value="2"> <p>Click <span class="bold">System</span> > <span class="bold">Customer Info</span>.</p> </li> 
 <li value="3"> <p>In the <span class="bold">API Key Settings</span> area, in the <span class="bold">After creation</span><em>, </em><span class="bold">API keys expire in</span> drop-down list, select the timeframe when you want the API keys to expire.</p> <p>When you change this option, the new timeframe begins from the time that you made the change. For example, if you change this option from <em>1 month</em> to <em>6 months</em>, the API Keys expire 6 months from the time&nbsp;you make the change.</p> <p>By default, API Keys expire each month.</p> </li> 
 <li value="4"> <p>To configure API Keys to expire at the time the users' passwords expire, select <span class="bold">Remove API key when a user's password expire</span>.</p> <p>By default, this option is not selected.</p> <p>For information about how to configure user passwords to expire, see <a href="../../../administration-and-setup/manage-workfront/security/configure-security-preferences.md" class="MCXref xref">Configure system security preferences</a>.&nbsp;</p> </li> 
 <li value="5">Click <span class="bold">Save</span>.</li> 
</ol>

## Remove the API keys for all users

If you are concerned about a particular security breach regarding your *Workfront* system, you can&nbsp;remove API Keys simultaneously for all users.

>[!IMPORTANT]
>
>Removing API Keys for all users invalidates ALL of the API Keys for all the users in the system. This action will cause all of your integrations in *Workfront* to fail until you generate a new API Key in *Workfront* and update all your&nbsp;integrations.

<ol> 
 <li value="1">Click the <span class="bold">Main Menu</span> icon <img src="assets/main-menu-icon.png"> in the upper-right corner of <em>Adobe Workfront</em>, then click <span class="bold">Setup</span> <img src="assets/gear-icon-settings.png">.&nbsp;&nbsp;<br></li> 
 <li value="2">Expand <span class="bold">System</span>, then click <span class="bold">Customer Info.</span></li> 
 <li value="3">In the <span class="bold">API Key Settings</span> area, click <span class="bold">Remove all API keys</span>, then click <span class="bold">Remove</span> <span class="bold">All</span>.</li> 
</ol>

## Restricting API logins with an X.509 certificate

>[!IMPORTANT]
>
>The procedure described in this section applies only to organizations that have not yet been onboarded to the Adobe Business Platform. Logging in to *Workfront* through the *Workfront* API is not available if your organization has been onboarded to the Adobe Business Platform.
>
>For a list of procedures that differ based on whether your organization has been onboarded to the Adobe Business Platform, see [Platform-based administration differences (Adobe Workfront/Adobe Business Platform)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

Third-party applications can communicate with *Workfront* through the API. To increase the security of your *Workfront* site, you can configure *Workfront* to restrict API login requests by uploading an X.509 certificate to Workfront *Workfront*.&nbsp;Once enabled, all login requests through the API must include a client certificate in addition to username and password.

>[!NOTE]
>
>This is not available if your organization’s *Workfront* instance is enabled with Adobe IMS. See your network or IT administrator if you need more information.

* [Obtain the X.509 certificate](#obtaining-the-x509-certificate) 
* [Upload the certificate to Workfront](#uploading-the-certificate-to-workfront) 
* [Verify API login calls are restricted](#verify)

### Obtain the X.509 certificate

Obtain a valid X.509 certificate from a trusted Certificate Authority (such as Verisign), and place it in a temporary location on your workstation.&nbsp;

### Upload the certificate to *Workfront*

After you have obtained the X.509 certificate from your Certificate Authority, you need to upload it to *Workfront*.

<ol> 
 <li value="1">Click the <span class="bold">Main Menu</span> icon <img src="assets/main-menu-icon.png"> in the upper-right corner of <em>Adobe Workfront</em>, then click <span class="bold">Setup</span> <img src="assets/gear-icon-settings.png">.<br></li> 
 <li value="2">Expand <span class="bold">System</span>, then click <span class="bold">Customer Info</span>.</li> 
 <li value="3"> <p>In the<span class="bold"> API Key Settings</span> area, select <span class="bold">Enable X.509 Certificate</span>.</p> </li> 
 <li value="4">On your workstation, browse to and select the X.509 certificate that you previously downloaded.</li> 
 <li value="5">(Optional) Click <span class="bold">View Details</span>&nbsp;next to the certificate name to view the following details about the certificate:</li> 
 <ul> 
  <li>Subject Common Name</li> 
  <li>Subject Organization</li> 
  <li>Subject Organization Unit</li> 
  <li>Issuer Common Name</li> 
  <li>Issuer Organization</li> 
  <li>Issuer Organization Unit</li> 
  <li>Serial Number</li> 
  <li>Issue Date</li> 
  <li>Expiration Date</li> 
 </ul> 
 <li value="6">Click <span class="bold">Save</span>.&nbsp;</li> 
</ol>

### Verify API login calls are restricted

Prior to configuring your instance of *Workfront* to require an X.509 certificate, perform an API request to the `/login` endpoint using valid username and password parameters. You will receive a 200 response that contains a sessionID.

After making the X.509 certificate a requirement via the customer info page in your instance of *Workfront*, make another login attempt. This time you will receive a 500 error response with the following message: “Untrusted request. Please contact your system administrator and attach certificate."

After confirming that the X.509 certificate is required, perform the same login request with an additional parameter for apiCertificate set to the value of your certificate. If this operation was performed correctly you will receive a 200 response that contains a valid sessionID.
