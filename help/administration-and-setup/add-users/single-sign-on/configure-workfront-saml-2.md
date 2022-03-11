---
filename: configure-workfront-saml-2
user-type: administrator
product-area: system-administration;setup
navigation-topic: single-sign-on-in-workfront
title: Configure Adobe Workfront with SAML 2.0
description: The procedure described on this page applies only to organizations that are not yet onboarded to the Adobe Admin Console.
---

# Configure `Adobe Workfront` with SAML 2.0

>[!IMPORTANT]
>
>The procedure described on this page applies only to organizations that are not yet onboarded to the Adobe Admin Console.
>
>If your organization has been onboarded to the Adobe Admin Console, see [Platform-based administration differences (Adobe Workfront/Adobe Business Platform)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

As an `Adobe Workfront administrator`, you can configure the `Workfront` web and mobile applications to integrate with a Security Assertion Markup Language (SAML) 2.0 solution for single sign-on (SSO).

After you have configure SAML 2.0 in `Workfront`, as described in the following sections, you can maintain the configuration, as described in [Update SAML 2.0 metadata in your identity provider](../../../administration-and-setup/add-users/single-sign-on/update-saml-2-metadata-ip.md).

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

## Enable authentication to `Workfront` with SAML 2.0

<ol> 
 <li value="1">Click the <span class="bold">Main Menu</span> icon <img src="assets/main-menu-icon.png"> in the upper-right corner of <span>Adobe Workfront</span>, then click <span class="bold">Setup</span> <img src="assets/gear-icon-settings.png">.</li> 
 <li value="2">Click <span class="bold">System</span> > <span class="bold">Single Sign-On (SSO).</span></li> 
 <li value="3">In the <span class="bold">Type</span> drop-down list, click <span class="bold">SAML 2.0.</span></li> 
 <li value="4"> <p>Near the top of the options that appear, click <span class="bold">Download SAML 2.0 Metadata</span>, then save the file to a temporary location on your computer.<br></p> <p>Your SAML 2.0 Identity Provider requires an XML file with information generated in your <span>Workfront</span> instance. After the file is downloaded, you need to go to your SAML 2.0 Identity Provider server and upload the <span>Workfront</span> SAML 2.0 Metadata XML file there.</p> </li> 
 <li value="5"> <p>Specify the following information:</p> 
  <table cellspacing="0"> 
   <col> 
   <col> 
   <tbody> 
    <tr> 
     <td role="rowheader"><span class="bold">Service Provider ID</span> </td> 
     <td> This URL, already populated for you, identifies <span>Workfront</span> to your identity provider. For example: <span class="bold"><yourcompany>.com/SAML2</span>.</td> 
    </tr> 
    <tr> 
     <td role="rowheader"><span style="font-weight: bold;">Binding Type</span> </td> 
     <td> <p>Select the method supported by your IDP server for sending authentication information:</p> 
      <ul> 
       <li>POST</li> 
       <li>REDIRECT</li> 
      </ul> </td> 
    </tr> 
    <tr> 
     <td role="rowheader"><span class="bold">Populate fields from Identity Provider Metadata</span> </td> 
     <td>In your SAML 2.0 Identity Provider solution, export a Service Provider Metadata XML file and save it to a temporary location on your computer. Select <span class="bold">Choose File</span>, then find and select the file you saved to add it to your <span>Workfront</span> configuration.</td> 
    </tr> 
    <tr> 
     <td role="rowheader"><span style="font-weight: bold;">Login Portal URL</span> </td> 
     <td>Specify your organization's common login portal. This is the URL where users log in to access <span>Workfront</span> and all other applications integrated with SAML 2.0.</td> 
    </tr> 
    <tr> 
     <td role="rowheader"><span style="font-weight: bold;">Sign-Out URL</span> </td> 
     <td> <p>Specify the sign-out URL for the IDP server. <span>Workfront</span> sends an HTTP request to this URL before signing out of <span>Workfront</span>. This closes the user's session on the remote server when the <span>Workfront</span> session is closed.</p> <note type="note">
        You are redirected to the sign-out URL only if you have the option Only Allow SAML 2.0 Authentication enabled in your user profile.
      </note> </td> 
    </tr> 
    <tr> 
     <td role="rowheader"><span class="bold">Change Password URL</span> </td> 
     <td> <p> Specify the URL where users will be redirected to change their passwords. </p> <p>Because the SAML 2.0 credentials are used to access <span>Workfront</span>, users need to be redirected to a page where they can change their SAML 2.0 password instead of completing this activity through <span>Workfront</span>.</p> </td> 
    </tr> 
    <tr> 
     <td role="rowheader"><span class="bold">Secure Hash Algorithm</span> </td> 
     <td> <p>Select the Secure Hash Algorithm (SHA) that your IDP supports:</p> 
      <ul> 
       <li>SHA-1</li> 
       <li>SHA-256</li> 
      </ul> </td> 
    </tr> 
    <tr> 
     <td role="rowheader"><span style="font-weight: bold;">Auto-Provision Users</span> </td> 
     <td> <p>Automatically creates a user in the system when a new user with a directory username and password attempts to log in to <span>Workfront</span> for the first time.</p> <p>In order to create users in <span>Workfront</span>, you need to map <span>Workfront</span> data attributes with the following user data attributes in your directory provider:</p> 
      <ul> 
       <li>First Name</li> 
       <li>Last Name</li> 
       <li>Email Address</li> 
      </ul> <p>The following options display to allow you to do this:</p> <p> <img src="assets/saml-2.0-auto-provision-users-ui-350x258.png" alt="saml_2.0_auto-provision_users_ui.png" style="width: 350;height: 258;"> </p> <p>Select the <span>Workfront</span> User Attribute that you want to map from the drop-down list, then specify the corresponding Directory Attribute in the user directory.</p> <p>The <span class="bold">Directory Attribute</span> field should contain the Directory Attribute Name from the User Attribute table you saved when successfully testing your SAML 2.0 configuration.</p> <p>You can set a Default <span>Workfront</span> Value in the <span class="bold">Default Value</span> field. You can also set rules based on the values from your SAML 2.0 Identity Provider.</p> <p class="warning" data-mc-autonum="<b>Warning: </b>"><span class="autonumber"><span><b>Warning: </b></span></span><span>Workfront</span> attempts to map the attributes listed below every time a user logs into the system. Because of this, we do not recommend mapping access levels. You can easily remove administrative access if an attribute is mapped incorrectly. Click Add Mapping to add additional rules.<em><br></em></p> <p>You can map the following <span>Workfront</span> attributes:</p> 
      <table> 
       <col> 
       <col> 
       <tbody> 
        <tr> 
         <td> 
          <ul> 
           <li> <p>Access Level</p> </li> 
          </ul> 
          <ul> 
           <li> <p>Address</p> </li> 
           <li> <p>Address2</p> </li> 
           <li> <p>Billing Per Hour</p> </li> 
           <li> <p>City</p> </li> 
           <li> <p>Company</p> </li> 
           <li> <p>Cost Per Hour</p> </li> 
           <li> <p>Email Address</p> </li> 
           <li> <p>Extension</p> </li> 
           <li> <p>First Name</p> </li> 
           <li> <p>Home Group</p> </li> 
           <li> <p>Home Team</p> </li> 
           <li> <p>Job Role</p> </li> 
           <li> <p>Last Name</p> </li> 
           <li> <p>Layout Template</p> </li> 
           <li> <p>Manager</p> </li> 
           <li> <p>Mobile Phone</p> </li> 
           <li> <p>Phone Number</p> </li> 
           <li> <p>Postal Code</p> </li> 
           <li> <p>Schedule</p> </li> 
           <li> <p>State</p> </li> 
           <li> <p>Timesheet Profile</p> </li> 
           <li> <p>Title</p> </li> 
          </ul> </td> 
         <td> <p> </p> </td> 
        </tr> 
       </tbody> 
      </table> <p>Click <span class="bold">Save</span> when you are finished mapping user attributes.</p> </td> 
    </tr> 
    <tr> 
     <td role="rowheader"><span class="bold">Certificate</span> </td> 
     <td> <p>Upload a valid SSL certificate to ensure a secure connection between the authentication service and <span>Workfront</span>. For OnDemand accounts, a certificate is always required. You can obtain this certificate from your SAML 2.0 system administrator.</p> </td> 
    </tr> 
    <tr> 
     <td role="rowheader"><span class="bold">Admin Exemption</span> </td> 
     <td> <p>Allows <span>Workfront administrators</span> to access <span>Workfront</span> using their <span>Workfront</span> login. If this option is not selected, <span>Workfront administrators</span> must use their SAML 2.0 username and password.</p> <p><span>Workfront</span> first attempts to log in to <span>Workfront</span> via SAML 2.0 for users with the <span>Workfront</span> System Administrator access level. If the SAML 2.0 authentication fails, <span>Workfront</span> uses local authentication for <span>Workfront administrators</span>.<br></p> <p>We recommend that you always have this option selected so that your <span>Workfront administrator</span> can log in to <span>Workfront</span> if your SAML 2.0 provider is ever temporarily unavailable.<br></p> </td> 
    </tr> 
    <tr> 
     <td role="rowheader"><span class="bold">Enable</span> </td> 
     <td> <p>Activates SSO on the <span>Workfront</span> system. Ensure that you have communicated login instructions to your users.</p> <p>After you enable your SSO configuration in <span>Workfront</span>, you must enable the <span class="bold">Only Allow SAML 2.0 Authentication</span> setting for all users so that they can use SSO.</p> <p>For more information about updating users for SSO, see <a href="../../../administration-and-setup/add-users/single-sign-on/update-users-sso.md" class="MCXref xref">Update users for single sign-on</a>.</p> <p>For more information about user settings, see <a href="../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref">Edit a user's profile</a>.</p> </td> 
    </tr> 
    <tr> 
     <td role="rowheader"><span class="bold">Confirm Configuration</span> </td> 
     <td> <p>Click <span class="bold">Test Connection</span> to verify that <span>Workfront</span> and the SAML 2.0 Identity Provider can communicate with each other. This connection is successful only if you exchanged the XML files.</p> <p>After you successfully test the link between your SAML 2.0 Identity Provider and <span>Workfront</span>, you see a screen similar to the one below.<br><note type="note">
         This screen is displayed in a browser pop-up, so ensure that you disable pop-up blockers in your browser.
        <br>
       </note>Save the information displayed in the table for later use.<br><img src="assets/2g-350x209.png" alt="" style="width: 350;height: 209;"></p> </td> 
    </tr> 
   </tbody> 
  </table> </li> 
 <li value="6">Click <span class="bold">Save</span> to save the SAML 2.0 configuration.</li> 
</ol>

