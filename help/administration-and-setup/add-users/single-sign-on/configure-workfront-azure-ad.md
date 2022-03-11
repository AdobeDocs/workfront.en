---
filename: configure-workfront-azure-ad
user-type: administrator
product-area: system-administration;setup
navigation-topic: single-sign-on-in-workfront
title: Configure Adobe Workfront with Azure Active Directory
description: The procedure described on this page applies only to organizations that are not yet onboarded to the Adobe Admin Console.
---

# Configure `Adobe Workfront` with Azure Active Directory

>[!IMPORTANT]
>
>The procedure described on this page applies only to organizations that are not yet onboarded to the Adobe Admin Console.
>
>If your organization has been onboarded to the Adobe Admin Console, see [Platform-based administration differences (Adobe Workfront/Adobe Business Platform)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

`Adobe Workfront` single sign-on (SSO) supports the integration with Azure Active Directory. You configure `Workfront` SSO with Azure Active Directory using the Security Assertion Markup Language (SAML) 2.0 option in `Workfront`.

>[!NOTE]
>
>This is not available if your organization’s `Workfront` instance uses a custom SSO portal>
><!-->
>or is enabled with Adobe IMS>
>-->
>. See your network or IT administrator if you need more information.

##

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

## Prerequisites

To configure `Workfront` Single Sign-On with Azure Active Directory, you need the following items:

* An Azure Active Directory subscription
* A `Workfront` subscription enabled for using Single Sign-On integrations
* An Azure Active Directory system administrator
* A `Workfront administrator`

>[!NOTE]
>
>`Workfront` is not responsible for setting up and troubleshooting your Azure Active Directory configuration. You must have an in-house system administrator that manages that part of the integration, in addition to a `Workfront administrator`.

## Add `Workfront` from the Azure Gallery

To configure the integration of `Workfront` SSO with Azure Active Directory, you need to add `Workfront` from the Azure gallery to your list of managed SaaS apps.

<ol class="lf-text-block lf-block" data-lf-anchor-id="87e4e42dcc1f6edc31cda8cbc513637a:0"> 
 <li value="1">Go to the following URL to access the <span class="bold">Azure Portal</span>: <a href="https://portal.azure.com/">https://portal.azure.com/</a> </li> 
 <li value="2"> <p>In the <span class="bold">Azure Portal</span>, on the left navigation panel, click the <span class="bold">Azure Active Directory</span> icon.</p> <p> <img src="assets/active-directory-icon.png"> </p> </li> 
 <li value="3"> <p>Navigate to <span class="bold">Enterprise applications</span>. Then go to <span class="bold">All applications</span>.</p> <p> <img src="assets/ad-all-applications-350x347.png" style="width: 350;height: 347;"> </p> </li> 
 <li value="4"> <p>To add a new application, click the <span class="bold">New application</span> button on the top of the dialog.</p> <p> <img src="assets/ad-new-application.png"> </p> </li> 
 <li value="5"> <p>In the search box, type <span class="bold"><span>Workfront</span></span>.</p> <p> <img src="assets/ad-search-350x61.png" style="width: 350;height: 61;"> </p> </li> 
 <li value="6">In the results panel, select <span class="bold"><span>Workfront</span></span>, and then click <span class="bold">Add</span> button to add the application.</li> 
</ol>

## Configure Azure Active Directory single sign-on

<ol class="lf-text-block lf-block" data-lf-anchor-id="cda51c033d1f6dff394188dfe1134350:0"> 
 <li value="1"> <p>In the Azure Portal, on the <span class="bold"><span>Workfront</span></span> application integration page, click <span class="bold">Single sign-on</span>.</p> </li> 
 <li value="2"> <p>On the <span class="bold">Single sign-on</span> dialog box, select <span class="bold">Mode</span> as <span class="bold">SAML-based Sign-on</span> to enable Single Sign-On.</p> <p> <img src="assets/ad-enable-sso-350x44.png" style="width: 350;height: 44;"> </p> </li> 
 <li value="3"> <p>In the <span class="bold"><span>Workfront</span> Domain and URLs</span> section, specify the following information:<br>-<span class="bold"> Sign-on URL</span>: your <span>Workfront</span> URL using the following pattern: https://<companyname>.my.workfront.com<br>- <span class="bold">Identifier</span>: your <span>Workfront</span> SAML 2.0 URL using the following pattern: https://<companyname>.my.workfront.com/SAML2</p> <p> <img src="assets/tutorial-workfront-url-350x47.png" style="width: 350;height: 47;"> </p> </li> 
 <li value="4"> <p>In the <span class="bold">SAML Signing Certificate</span> section, click <span class="bold">Certificate(Base64)</span> and then save the Certificate file on your computer.</p> <p> <img src="assets/ad-save-certificate-350x68.png" style="width: 350;height: 68;"> </p> </li> 
 <li value="5"> <p>Click <span class="bold">Save</span>.</p> </li> 
 <li value="6"> <p>In the <span class="bold"><span>Workfront</span> Configuration</span> section, click <span class="bold">Configure <span>Workfront</span></span> to open <span class="bold">Configure sign-on</span> window.</p> </li> 
 <li value="7"> <p>Copy the <span class="bold">Sign-Out URL</span> and<span class="bold"> SAML Single Sign-On Service URL</span> from the <span class="bold">Quick Reference</span> section.</p> <p> <img src="assets/ad-quick-reference-350x47.png" style="width: 350;height: 47;"> </p> </li> 
</ol>

## Configure `Workfront` with Azure Active Directory

<ol class="lf-text-block lf-block" data-lf-anchor-id="cda51c033d1f6dff394188dfe1134350:0"> 
 <li value="1">Log in to <span>Workfront</span> as a <span>Workfront administrator</span>.</li> 
 <li value="2">Click the <span class="bold">Main Menu</span> icon <img src="assets/main-menu-icon.png"> in the upper-right corner of <span>Adobe Workfront</span>, then click <span class="bold">Setup</span> <img src="assets/gear-icon-settings.png">.<br></li> 
 <li value="3">At the bottom of the left panel, click <span class="bold">System</span> > <span class="bold">Single Sign-On (SSO)</span>.</li> 
 <li value="4">Click the <span class="bold">Type</span> box, then click <span class="bold">SAML 2.0</span>. </li> 
 <li value="5"> <p>Select the check box next to <span class="bold">Service Provider ID</span>, then specify that ID using the following format:</p> <p>https://<companyname>.my.workfront.com/SAML2</p> </li> 
 <li value="6">Paste the <span class="bold">SAML Single Sign-On Service URL</span> into the <span class="bold">Login Portal URL</span> field.</li> 
 <li value="7">Paste the <span class="bold">Single Sign-Out URL</span> into the <span class="bold">Sign-Out URL</span> field.</li> 
 <li value="8">Specify the <span class="bold">Change Password URL</span>.</li> 
 <li value="9">Click <span class="bold">Save</span>.</li> 
</ol>

