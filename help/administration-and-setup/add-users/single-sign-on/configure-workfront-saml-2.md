---
filename: configure-workfront-saml-2
user-type: administrator
product-area: system-administration;setup
navigation-topic: single-sign-on-in-workfront
---



# Configure *`Adobe Workfront`* with SAML 2.0 {#configure-adobe-workfront-with-saml}



>[!IMPORTANT] {type="important"}
>
>The procedure described on this page applies only to organizations that are not yet onboarded to the Adobe Business Platform.
>
>
>If your organization has been onboarded to the Adobe Business Platform, Single Sign-On (SSO) is handled automatically as part of that integration. You do not need to configure or enable this functionality.
>
>
>For a list of procedures that differ based on whether your organization is migrated to Adobe IMS, see [Platform-based administration differences (Adobe Workfront/Adobe Business Platform)](actions-in-admin-console.md).



As an *`Adobe Workfront administrator`*, you can configure the *`Workfront`* web and mobile applications to integrate with a Security Assertion Markup Language (SAML) 2.0 solution for single sign-on (SSO).


After you have configure SAML 2.0 in *`Workfront`*, as described in the following sections, you can maintain the configuration, as described in [Update SAML 2.0 metadata in your identity provider](update-saml-2-metadata-ip.md).


## Access requirements {#access-requirements}

You must have the following to perform the steps in this article:

<table style="width: 100%;margin-left: 0;margin-right: auto;mc-table-style: url('../../../Resources/TableStyles/TableStyle-List-options-in-steps.css');" class="TableStyle-TableStyle-List-options-in-steps" cellspacing="0"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2"> 
 <tbody> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader"><span class="mc-variable WFVariables.FullProdNameWF variable varname">Adobe Workfront</span> plan</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p>Any</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader"><span class="mc-variable WFVariables.FullProdNameWF variable varname">Adobe Workfront</span> license</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray"> <p><span class="mc-variable WFVariables.WFLicense-Plan variable varname">Plan</span> </p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-LightGray" role="rowheader">Access level configurations</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-LightGray"> <p>You must be a <span class="mc-variable WFVariables.AdminWF variable varname">Workfront administrator</span>. For more information, see <a href="grant-a-user-full-administrative-access.md" class="MCXref xref">Grant a user full administrative access</a>.</p> <p>Note: If you still don't have access, ask your <span class="mc-variable WFVariables.AdminWF variable varname">Workfront administrator</span> if they set additional restrictions in your access level. For information on how a <span class="mc-variable WFVariables.AdminWF variable varname">Workfront administrator</span> can modify your access level, see <a href="create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>



## Enable authentication to *`Workfront`* with SAML 2.0 {#enable-authentication-to-workfront-with-saml}




1. Click the `Main Menu` icon ![](assets/main-menu-icon.png) in the upper-right corner of *`Adobe Workfront`*, then click `Setup` ![](assets/gear-icon-settings.png).

1. Click `System` > `Single Sign-On (SSO).`

1. In the `Type` drop-down list, click `SAML 2.0.`

1.  Near the top of the options that appear, click `Download SAML 2.0 Metadata`, then save the file to a temporary location on your computer.  



   Your SAML 2.0 Identity Provider requires an XML file with information generated in your *`Workfront`* instance. After the file is downloaded, you need to go to your SAML 2.0 Identity Provider server and upload the *`Workfront`* SAML 2.0 Metadata XML file there.

1.  Specify the following information:

<table style="width: 100%;mc-table-style: url('../../../Resources/TableStyles/TableStyle-List-options-in-steps.css');margin-left: 0;margin-right: auto;" class="TableStyle-TableStyle-List-options-in-steps" cellspacing="0"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2"> 
 <tbody> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader"><span class="bold">Service Provider ID</span> </td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> This URL, already populated for you, identifies <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span> to your identity provider. For example: <span class="bold">&lt;yourcompany&gt;.com/SAML2</span>.</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader"><span style="font-weight: bold;">Binding Type</span> </td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray"> <p>Select the method supported by your IDP server for sending authentication information:</p> 
    <ul> 
     <li>POST</li> 
     <li>REDIRECT</li> 
    </ul> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader"><span class="bold">Populate fields from Identity Provider Metadata</span> </td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray">In your SAML 2.0 Identity Provider solution, export a Service Provider Metadata XML file and save it to a temporary location on your computer. Select <span class="bold">Choose File</span>, then find and select the file you saved to add it to your <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span> configuration.</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader"><span style="font-weight: bold;">Login Portal URL</span> </td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray">Specify your organization's common login portal. This is the URL where users log in to access <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span> and all other applications integrated with SAML 2.0.</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader"><span style="font-weight: bold;">Sign-Out URL</span> </td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p>Specify the sign-out URL for the IDP server. <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span> sends an HTTP request to this URL before signing out of <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span>. This closes the user's session on the remote server when the <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span> session is closed.</p> <p>Note:  You are redirected to the sign-out URL only if you have the option Only Allow SAML 2.0 Authentication enabled in your user profile.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader"><span class="bold">Change Password URL</span> </td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray"> <p> Specify the URL where users will be redirected to change their passwords. </p> <p>Because the SAML 2.0 credentials are used to access <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span>, users need to be redirected to a page where they can change their SAML 2.0 password instead of completing this activity through <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span>.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader"><span class="bold">Secure Hash Algorithm</span> </td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p>Select the Secure Hash Algorithm (SHA) that your IDP supports:</p> 
    <ul> 
     <li>SHA-1</li> 
     <li>SHA-256</li> 
    </ul> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader"><span style="font-weight: bold;">Auto-Provision Users</span> </td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray"> <p>Automatically creates a user in the system when a new user with a directory username and password attempts to log in to <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span> for the first time.</p> <p>In order to create users in <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span>, you need to map <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span> data attributes with the following user data attributes in your directory provider:</p> 
    <ul> 
     <li>First Name</li> 
     <li>Last Name</li> 
     <li>Email Address</li> 
    </ul> <p>The following options display to allow you to do this:</p> <p> <img src="assets/saml-2.0-auto-provision-users-ui-350x258.png" alt="saml_2.0_auto-provision_users_ui.png" style="width: 350;height: 258;"> </p> <p>Select the <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span> User Attribute that you want to map from the drop-down list, then specify the corresponding Directory Attribute in the user directory.</p> <p>The <span class="bold">Directory Attribute</span> field should contain the Directory Attribute Name from the User Attribute table you saved when successfully testing your SAML 2.0 configuration.</p> <p>You can set a Default <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span> Value in the <span class="bold">Default Value</span> field. You can also set rules based on the values from your SAML 2.0 Identity Provider.</p> <p class="warning" data-mc-autonum="<b>Warning: </b>"><span class="autonumber"><span><b>Warning: </b></span></span><span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span> attempts to map the attributes listed below every time a user logs into the system. Because of this, we do not recommend mapping access levels. You can easily remove administrative access if an attribute is mapped incorrectly. Click Add Mapping to add additional rules.<em><br></em></p> <p>You can map the following <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span> attributes:</p> 
    <table style="width: 100%;"> 
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
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader"><span class="bold">Certificate</span> </td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p>Upload a valid SSL certificate to ensure a secure connection between the authentication service and <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span>. For OnDemand accounts, a certificate is always required. You can obtain this certificate from your SAML 2.0 system administrator.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader"><span class="bold">Admin Exemption</span> </td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray"> <p>Allows <span class="mc-variable WFVariables.AdminWF-plur variable varname">Workfront administrators</span> to access <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span> using their <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span> login. If this option is not selected, <span class="mc-variable WFVariables.AdminWF-plur variable varname">Workfront administrators</span> must use their SAML 2.0 username and password.</p> <p><span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span> first attempts to log in to <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span> via SAML 2.0 for users with the <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span> System Administrator access level. If the SAML 2.0 authentication fails, <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span> uses local authentication for <span class="mc-variable WFVariables.AdminWF-plur variable varname">Workfront administrators</span>.<br></p> <p>We recommend that you always have this option selected so that your <span class="mc-variable WFVariables.AdminWF variable varname">Workfront administrator</span> can log in to <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span> if your SAML 2.0 provider is ever temporarily unavailable.<br></p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader"><span class="bold">Enable</span> </td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p>Activates SSO on the <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span> system. Ensure that you have communicated login instructions to your users.</p> <p>After you enable your SSO configuration in <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span>, you must enable the <span class="bold">Only Allow SAML 2.0 Authentication</span> setting for all users so that they can use SSO.</p> <p>For more information about updating users for SSO, see <a href="update-users-SSO.md" class="MCXref xref">Update users for single sign-on</a>.</p> <p>For more information about user settings, see <a href="edit-a-users-profile.md" class="MCXref xref">Edit a user's profile</a>.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-MediumGray" role="rowheader"><span class="bold">Confirm Configuration</span> </td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-MediumGray"> <p>Click <span class="bold">Test Connection</span> to verify that <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span> and the SAML 2.0 Identity Provider can communicate with each other. This connection is successful only if you exchanged the XML files.</p> <p>After you successfully test the link between your SAML 2.0 Identity Provider and <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span>, you see a screen similar to the one below.<br><p>Note:  This screen is displayed in a browser pop-up, so ensure that you disable pop-up blockers in your browser.<br></p>Save the information displayed in the table for later use.<br><img src="assets/2g-350x209.png" alt="" style="width: 350;height: 209;"></p> </td> 
  </tr> 
 </tbody> 
</table>


1. Click `Save` to save the SAML 2.0 configuration.


