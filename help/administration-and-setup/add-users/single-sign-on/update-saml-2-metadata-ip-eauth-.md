

# Update SAML 2.0 metadata in your IDP when using enhanced authentication

>[!IMPORTANT]
>
>The procedure described on this page applies only to organizations that are not yet onboarded to the Adobe Admin Console.
>
>If your organization has been onboarded to the Adobe Admin Console, see [Platform-based administration differences (Adobe Workfront/Adobe Business Platform)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

As an Adobe Workfront administrator, you can integrate Workfront single sign-on (SSO) with any identity provider that supports the Security Assertion Markup Language (SAML) 2.0 protocol.

The following sections describe the integration process when your Workfront account has been upgraded to the enhanced authentication experience (not yet available to all organizations). For more information about the enhanced authentication experience, see [Enhanced Authentication overview](../../../administration-and-setup/manage-workfront/security/get-started-enhanced-authentication.md).

For information about configuring SAML prior to your migration to the enhanced authentication experience, see [Update SAML 2.0 metadata in your identity provider](../../../administration-and-setup/add-users/single-sign-on/update-saml-2-metadata-ip.md).

>[!NOTE]
>
>This is not available if your organization’s Workfront instance is enabled with Adobe IMS. See your network or IT administrator if you need more information.

##

## Access requirements

You must have the following to perform the steps in this article:

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>You must be a Workfront administrator. For more information, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Grant a user full administrative access</a>.</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Use Okta as your identity provider

Okta is an example of an identity provider that supports SAML 2.0. This section describes how to use Okta as your identity provider. Similar steps would be required when configuring another identity provider that supports SAML 2.0.

>[!NOTE]
>
>Users are mapped based on their email address. In order to log in to Workfront using Okta, you must have a user with the same (case-insensitive) email address created in your Workfront customer.

Complete the following sections to configure Okta as your identity provider in Workfront.

* [Create a Workfront app in Okta](#creating-a-workfront-app-in-okta) 
* [Add your Okta instance as an identity provider in Workfront](#adding-your-okta-instance-as-an-identity-provider-in-workfront)

### Create a Workfront app in Okta

<ol> 
 <li value="1">Log in to your Okta environment. </li> 
 <li value="2">Ensure that <span class="bold">Classic UI</span> is selected in the upper-left corner of the Okta interface.</li> 
 <li value="3">In the menu, click <span class="bold">Applications</span> > <span class="bold">Applications</span>.</li> 
 <li value="4">Click <span class="bold">Add Application</span>, then click <span class="bold">Create New App</span>.</li> 
 <li value="5">In the <span class="bold">Create a New Application Integration dialog</span> box, select <span class="bold">SAML 2.0</span>, then click <span class="bold">Create</span>.</li> 
 <li value="6">Specify a name for your Workfront app, then click <span class="bold">Next</span>.</li> 
 <li value="7">In the SAML Settings page that displays, locate information required for the SAML Settings page: 
  <ol>
   <li value="1">Without exiting the browser tab where the Okta interface is displayed, open a separate browser tab or window.</li>
   <li value="2"><p>Specify the following URL in the browser:<br></p><p><i>https://[your_customer_subdomain].my.workfront.com/auth/saml2/metadata</i></p></li>
   <li value="3"><p>In the resulting XML file, identify the values for <span class="bold">entityID</span> and <span class="bold">Location</span>.</p><p><img src="assets/sso-okta-350x108.png" alt="sso-okta.png" style="width: 350;height: 108;"></p></li>
   <li value="4">Copy the value from the <span class="bold">entityID</span> field to your system clipboard. Do not close this browser tab.</li>
  </ol></li> 
 <li value="8">Go back to the SAML Settings page that you opened in Step 6. </li> 
 <li value="9">Paste the value from the <span class="bold">entityID</span> field into the <span class="bold">Audience URI (SP Entity ID)</span> field.</li> 
 <li value="10">In the XML file in your other browser tab, copy the value from the <span class="bold">Location</span> field.</li> 
 <li value="11">Paste the value from the <span class="bold">Location</span> field into the <span class="bold">Single sign on</span> <span class="bold">URL</span> field.</li> 
 <li value="12">Scroll to the <span class="bold">Attribute Statements (Optional)</span> section.</li> 
 <li value="13">In the <span class="bold">Name</span> field, specify <span class="bold">email</span>.</li> 
 <li value="14">In the <span class="bold">Value</span> field, specify <span class="bold">user.email</span>.</li> 
 <li value="15">(Optional) Add any advanced values.</li> 
 <li value="16">Click <span class="bold">Next</span>.</li> 
 <li value="17">Select, <span class="bold">I'm an Okta customer adding an internal app</span>, then click <span class="bold">Finish</span>.</li> 
</ol>

### Add your Okta instance as an identity provider in Workfront

This procedure provides essential information for configuring Okta as an identity provider in Workfront. For additional information about other mappings or configuration options, see [Configure Adobe Workfront with SAML 2.0](../../../administration-and-setup/add-users/single-sign-on/configure-workfront-saml-2.md).

<ol> 
 <li value="1">Download the identity provider metadata for your Okta instance: 
  <ol>
   <li value="1">Log in to your Okta environment. </li>
   <li value="2">Ensure that <span class="bold">Classic UI</span> is selected in the upper-left corner of the Okta interface.</li>
   <li value="3">In the menu, click <span class="bold">Applications</span> > <span class="bold">Applications</span>.</li>
   <li value="4">Click the Workfront app that you created, as described in the section, <a href="#creating-a-workfront-app-in-okta" class="MCXref xref">Create a Workfront app in Okta</a></li>
   <li value="5"><p>On the <span class="bold">Sign On</span> tab, click <span class="bold">Identity Provider metadata</span>.</p><p><img src="assets/idp-okta-metadata-350x243.png" alt="idp_okta_metadata.png" style="width: 350;height: 243;"></p><p>The metadata is opened as XML in a new browser tab.</p></li>
   <li value="6">Copy the URL that is displayed in the browser URL field.</li>
  </ol></li> 
 <li value="2">Log in to Workfront as a Workfront administrator.</li> 
 <li value="3">Click the <span class="bold">Main Menu</span> icon <img src="assets/main-menu-icon.png"> in the upper-right corner of Adobe Workfront, then click <span class="bold">Setup</span> <img src="assets/gear-icon-settings.png">.</li> 
 <li value="4">In the left panel, click <span class="bold">System</span> > <span class="bold">Single Sign-On (SSO)</span>.</li> 
 <li value="5"> <p>(Conditional) If you see two tabs, click the <span class="bold">New SSO Providers</span> tab.</p> <p> <img src="assets/sso-idp-halflife-350x234.png" alt="sso_idp_halflife.png" style="width: 350;height: 234;"> </p> <note type="important">
    Do not delete your existing SSO configuration settings in the 
   <span class="bold">Current SSO Provider</span> tab until your account is updated to the enhanced authentication experience and the new SSO configuration is fully functional.
  </note> </li> 
 <li value="6">Click <span class="bold">New SSO Provider</span>.</li> 
 <li value="7">Specify a name, such as Okta IDP, then specify a description.</li> 
 <li value="8">In the <span class="bold">Populate fields from Identity Provider Metadata</span> section, paste the URL that you copied in Step 1 into the <span class="bold">Metadata URL</span> field. <br>Alternatively, you can click <span class="bold">Choose File</span> to upload an .xml file, but we recommend that you paste the URL.</li> 
 <li value="9">In the <span class="bold">Map User Attributes</span> section, in the <span class="bold">Directory Attribute</span> field, type <span class="bold">email</span>. (<span class="bold">Email Address</span> is already populated in the <span class="bold">Workfront User Attribute</span> field.)</li> 
 <li value="10">(Optional) Enable <span class="bold">Make Default SSO Provider</span> to send unathenticated users to the identity provider login screen instead of to the Workfront login screen for authentication. We recommend that you enable this option only if all users in your system access Workfront through the identity provider.</li> 
 <li value="11">Select the <span class="bold">Enable</span> checkbox. Before doing this, ensure that users in your system are aware of the new login experience to ensure they do not lose access to the Workfront system.</li> 
 <li value="12">Click <span class="bold">Test Connection</span>.<br>You should see a message telling you the connection is successful. </li> 
 <li value="13">Click <span class="bold">Save</span>. </li> 
</ol>

## Using other identity providers

When using identity providers other than Okta (such as Ping or Centrify), you must re-upload the Workfront metadata to your identity provider.
