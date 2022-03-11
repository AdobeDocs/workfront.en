---
filename: configure-workfront-saml-2-adfs
user-type: administrator
product-area: system-administration;setup
navigation-topic: single-sign-on-in-workfront
title: Configure Adobe Workfront with SAML 2.0 using ADFS
description: The procedure described on this page applies only to organizations that are not yet onboarded to the Adobe Admin Console.
---

# Configure Adobe Workfront with SAML 2.0 using ADFS

>[!IMPORTANT]
>
>The procedure described on this page applies only to organizations that are not yet onboarded to the Adobe Admin Console.
>
>If your organization has been onboarded to the Adobe Admin Console, see [Platform-based administration differences (Adobe Workfront/Adobe Business Platform)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

As an Adobe Workfront administrator, you can integrate Workfront with a Security Assertion Markup Language (SAML) 2.0 solution for single sign-on while using Active Directory Federation Services (ADFS).

This guide focuses on setting up ADFS without auto provisioning or attribute mappings. We recommend that you complete the setup and test it prior to setting up any auto provisioning.

>[!NOTE]
>
>This is not available if your organization’s Workfront instance is enabled with Adobe IMS. See your network or IT administrator if you need more information.

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

## Enable authentication to Workfront with SAML 2.0

To enable authentication to the Workfront web application and the Workfront mobile application with SAML 2.0, complete the following sections:

* [Retrieve the Workfront SSO metadata file](#retrieving-workfront-metatdata) 
* [Configure Relying Party Trusts](#configuring-relying-party-trusts) 
* [Configure Claim Rules](#configuring-claim-rules) 
* [Upload the metadata file and test the connection](#uploading-metadata-file)

### Retrieve the Workfront SSO metadata file

<ol> 
 <li value="1">Click the <span class="bold">Main Menu</span> icon <img src="assets/main-menu-icon.png"> in the upper-right corner of Adobe Workfront, then click <span class="bold">Setup</span> <img src="assets/gear-icon-settings.png">.</li> 
 <li value="2">In the left panel, click <span class="bold">System</span> > <span class="bold">Single Sign-On (SSO)</span>.</li> 
 <li value="3"> <p>In the <span class="bold">Type</span> drop-down menu, click <span class="bold">SAML 2.0</span> to display additional information and options.<br></p> </li> 
 <li value="4">Copy the URL that displays after <span class="bold">Metadata URL</span>. </li> 
 <li value="5">Continue to the following section, <a href="#configuring-relying-party-trusts" class="MCXref xref">Configure Relying Party Trusts</a>.</li> 
</ol>

### Configure Relying Party Trusts

<ol> 
 <li value="1">Open the <span class="bold">ADFS Manager</span> using the Windows server 2008 R2 (version may vary).</li> 
 <li value="2">Go to <span class="bold">Start.</span></li> 
 <li value="3">Click <span class="bold">Administration Tools.</span></li> 
 <li value="4">Click <span class="bold">ADFS 2.0 Management.</span></li> 
 <li value="5">Select <span class="bold">ADFS</span> and expand <span class="bold">Trust Relationships</span>.</li> 
 <li value="6"> <p>Right-click <span class="bold">Relying Party Trusts</span>, then select <span class="bold">Add Relying Party Trust</span> to launch the Add Relying Party Trust Wizard.</p> <p> <img src="assets/screen-shot-2014-10-22-at-2.48.12-pm-1-350x153.png" alt="" style="width: 350;height: 153;"> </p> </li> 
 <li value="7"> <p>From the <span class="bold">Welcome Page</span>, select <span class="bold">Start</span>. </p> </li> 
 <li value="8">In the <span class="bold">Select Date Source</span> section, paste the metadata URL from Workfront.</li> 
 <li value="9"> <p>Click <span class="bold">Next</span>.</p> </li> 
 <li value="10"> <p>Click <span class="bold">OK</span> to acknowledge the warning message. </p> <p>This opens the <span class="bold">Specify Display Name</span> section.</p> </li> 
 <li value="11"> <p>Add a <span class="bold">Display Name</span> and <span class="bold">Notes</span> to distinguish the Trust, then click <span class="bold">Next</span>.<br></p> <p> <img src="assets/screen-shot-2014-10-22-at-2.50.58-pm-350x282.png" alt="" style="width: 350;height: 282;"> </p> </li> 
 <li value="12"> <p>Select <span class="bold">Permit all user to access this relying party</span> (Or <span class="bold">None</span> if you want to configure this later).<br></p> <p> <img src="assets/screen-shot-2014-10-22-at-2.53.19-pm-350x232.png" alt="" style="width: 350;height: 232;"> </p> </li> 
 <li value="13"> <p>Click <span class="bold">Next</span>. </p> <p>This takes you to the <span class="bold">Ready to Add Trust</span> section.</p> </li> 
 <li value="14">Continue to the following section <a href="#configuring-claim-rules" class="MCXref xref">Configure Claim Rules</a>.</li> 
</ol>

### Configure Claim Rules

<ol> 
 <p> <li> <p>Click <span class="bold">Next</span> in the <b>Ready to Add Trust</b> section, then ensure that the <span class="bold">Open the Edit Claim Rules dialog box</span> option is selected.</p> <p>This will allow you to edit Claim Rules in a future step.<br><img src="assets/screen-shot-2014-10-22-at-2.53.28-pm-350x236.png" alt="" style="width: 350;height: 236;"></p> </li> <li>Click <span class="bold">Close</span>.</li> <li>Click <span class="bold">Add Rule.</span></li> <li> <p>Select <span class="bold">Send LDAP Attribute as Claims</span>.</p> <p> <img src="assets/screen-shot-2014-10-22-at-2.56.29-pm-350x185.png" alt="" style="width: 350;height: 185;"> </p> </li> <li>Click <span class="bold">Next</span> to display the <span class="bold">Configure Claim Rule</span> step.<br><img src="assets/screen-shot-2014-10-22-at-2.57.00-pm-350x224.png" alt="" style="width: 350;height: 224;"></li> <li> <p>Specify the following minimum requirements to configure the claim rule: (This will go in the <span class="bold">Federation ID</span> on the user setup and is used to distinguish who is logging in.)</p> 
   <table cellspacing="0"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><span class="bold">Claim rule name:</span> </td> 
      <td>Specify a name for the claim rule. For example, "Workfront."</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Attribute store</td> 
      <td>Select <span class="bold">Active Directory</span> from the drop-down menu.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">LDAP Attribute</td> 
      <td>This can be any type of attribute. We recommend using <span class="bold">SAM-Account-Name</span> for this attribute.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Outgoing Claim Type</td> 
      <td>You must select <span class="bold">Name ID</span> as the outgoing claim type</td> 
     </tr> 
    </tbody> 
   </table> </li> <li> <p> (Optional) In order to establish auto provisioning, add the following additional claims in both the LDAP Attribute and Outgoing Claim Type:</p> 
   <ul> 
    <li style="font-weight: normal;"> <span class="bold">Given Name</span></li> 
    <li style="font-weight: normal;"><span class="bold">Surname</span> </li> 
    <li style="font-weight: normal;"><span class="bold">E-Mail Address</span> </li> 
   </ul> </li> <li>Click <span class="bold">Finish</span>, then click <span class="bold">OK</span> on the next screen.</li> <li> <p>Right-click the new <span class="bold">Relying Party Trust</span>, then select <span class="bold">Properties</span>.</p> <p> <img src="assets/screen-shot-2014-10-22-at-3.03.47-pm-350x129.png" alt="" style="width: 350;height: 129;"> </p> </li> <li>Select the<span class="bold"> Advanced Tab</span>. And under <span class="bold">Secure Hash Algorithm</span> select SHA-1 or SHA-256.</li> </p> 
</ol>

>[!NOTE]
>
>What you select under Secure Hash Algorithm here must match the Secure Hash Algorithm field in Workfront under Setup > System > Single Sign-ON (SSO).

![](assets/screen-shot-2014-10-22-at-3.04.55-pm-350x232.png)

11. Continue to the following section [Upload the metadata file and test the connection](#uploading-metadata-file).

### Upload the metadata file and test the connection

<ol> 
 <li value="1"> <p>Open a browser and navigate to https://<i><yourserver></i>/FederationMetadata/2007-06/FederationMetadata.xml. <br></p> <p>This should download a Metadata file FederationMetadata.xml file.</p> </li> 
 <li value="2">Click <span class="bold">Choose File</span> under <span class="bold">Populate fields from Identity Provider Metadata</span>, and select the <span class="bold">FederationMetadata.xml</span> file.</li> 
 <li value="3">(Optional) If the certificate information did not populate with the metadata file, you can upload a file separately. Select <span class="bold">Choose File</span> in the <span class="bold">Certificate</span> section.</li> 
 <li value="4"> <p>Click <span class="bold">Test Connection</span>. If set up correctly, you should see a page similar to the one shown below:<br></p> <p> <img src="assets/screen-shot-2014-10-22-at-3.09.17-pm-adobe-branding-350x120.png" style="width: 350;height: 120;"> </p> <note type="note">
   If you want to set up attribute mapping, ensure that you copy the attributes from the Test Connection into the Directory Attribute. For more information, see Mapping User Attributes.
   <br>
  </note> </li> 
 <li value="5"> <p>Select <span class="bold">Admin Exemption</span> to allow Workfront administrators to log in using Workfront credentials with the bypass url. </p> <p>Bookmarks pointing to <i><yourdomain></i>.my.workfront.com/login bypass the redirect.</p> </li> 
 <li value="6">Select the <span class="bold">Enable</span> box to enable the configuration.</li> 
 <li value="7">Click <span class="bold">Save</span>.</li> 
</ol>

## About updating users for SSO

Following this guide, the `SSO Username` will be their `Active Directory Username`.

As a Workfront administrator, you can bulk update users for SSO. For more information about updating users for SSO, see [Update users for single sign-on](../../../administration-and-setup/add-users/single-sign-on/update-users-sso.md).

As a Workfront administrator, you can also manually assign a Federation ID editing the user's profile and completing the Federation ID field. For more information about editing a user, see [Edit a user's profile](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

>[!NOTE]
>
>When editing users' profiles to include a Federation ID, selecting `Only Allow SAML 2.0 Authentication` removes the ability to log in to Workfront using the bypass url (*<yourdomain>*.my.workfront.com/login).

