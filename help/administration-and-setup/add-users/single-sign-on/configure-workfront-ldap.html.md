



# Configure `Workfront` with LDAP {#configure-workfront-with-ldap}



>[!IMPORTANT] {type="important"}
>
>LDAP is now supported only in a limited capacity as a Single Sign-On (SSO) option; it will be removed from the product in 2020. We recommend moving to SAML 2.0. For more information, see [Configure Workfront with SAML 2.0](configure-workfront-saml-2.md).


To connect  `Workfront` with an LDAP Directory Server:&nbsp;



1. Click the **Main Menu** icon ![](assets/main-menu-icon.png) in the upper-right corner of `Workfront`, then click **Setup** ![](assets/setup-gear-icon.png).

1. In the left panel, click **System** > **Single Sign-On (SSO)**.

1. In the **Type** drop-down list, click **LDAP**.  

1.  Specify the following information:

<table style="width: 100%;margin-left: 0;margin-right: auto;mc-table-style: url('../../../Resources/TableStyles/TableStyle-List-options-in-steps.css');" class="TableStyle-TableStyle-List-options-in-steps" cellspacing="0"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2"> 
 <tbody> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray">Server</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p>The URL of the LDAP server where your directory service is running.</p> <p>For example, <a class="external" title="ldap://hostname.com" href="ldap://hostname.com">ldap://hostname.com</a>.<br>Or, if the LDAP server requires an SSL connection, <a class="external" title="ldaps://hostname.com" href="ldaps://hostname.com">ldaps://hostname.com</a>.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray">Port</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray">The port number used for LDAP&nbsp;communication. The default port number for non-secure LDAP connections is 389. The default port number for secure LDAP connections (LDAPS) is 636.</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray">Search Base</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray">Specify where&nbsp;in the LDAP directory tree&nbsp;<span class="WFVariablesProdNameWF">Workfront</span>&nbsp;should find and synchronize initial user information from User objects. This is the container where <span class="WFVariablesProdNameWF">Workfront</span>&nbsp;begins&nbsp;searching for users on the LDAP server.<br>Use the following format: ou=people,dc=example,dc=com</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray">SSL/TLS</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray">Select this option to encrypt&nbsp;communication between the LDAP server and <span class="WFVariablesProdNameWF">Workfront</span>.&nbsp;This option is enforced for all OnDemand accounts.</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray">Auto-Provision Users</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray">When this option is enabled, <span class="WFVariablesProdNameWF">Workfront</span> automatically&nbsp;creates a user in the system when a new user with an LDAP username and password attempts to log in to <span class="WFVariablesProdNameWF">Workfront</span> for the first time. In order for users to be created in <span class="WFVariablesProdNameWF">Workfront</span>, you need to map <span class="WFVariablesProdNameWF">Workfront</span> data attributes with the LDAP data attributes.</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray">Attribute Synchronization</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray">Click <b>Map User Attributes</b>, select the <span class="WFVariablesProdNameWF">Workfront</span> User Attribute that you want to map from the drop-down list, then&nbsp;specify the corresponding Directory Attribute in the Active Directory server.&nbsp;You can also specify a Default Value for the attribute&nbsp;if you want one to be set. Click <b>Add Mapping</b> to include additional attributes, then click <b>Save</b> when you are finished.<p>Important:  <span class="WFVariablesProdNameWF">Workfront</span> attempts to map these attributes every time a user with these attributes logs into the system. If you have existing users in the system, make sure you are not overwriting their current access level, or any other attributes, by applying this mapping.&nbsp;</p><p>You can map the following <span class="WFVariablesProdNameWF">Workfront</span> attributes:</p>
    <ul>
     <li value="1">Access Level</li>
     <li value="2">Address</li>
     <li value="3">Address2</li>
     <li value="4">Billing Per Hour</li>
     <li value="5">City</li>
     <li value="6">Company</li>
     <li value="7">Cost Per Hour</li>
     <li value="8">Email Address</li>
     <li value="9">Extension</li>
     <li value="10">First Name</li>
     <li value="11">Home Group</li>
     <li value="12">Home Team</li>
     <li value="13">Job Role</li>
     <li value="14">Last Name</li>
     <li value="15">Layout Template</li>
     <li value="16">Manager</li>
     <li value="17">Mobile Phone</li>
     <li value="18">Phone Number</li>
     <li value="19">Postal Code</li>
     <li value="20">Schedule</li>
     <li value="21">State</li>
     <li value="22">Timesheet Profile</li>
     <li value="23">Title</li>
    </ul><p>If a user attempts to log in without using&nbsp;SSO and&nbsp;was created using auto-provisioning, it will appear that the their login is&nbsp;not working, or that their username/password combination is wrong. The user will either need to log in using their email address and <span class="WFVariablesProdNameWF">Workfront</span> password, or&nbsp;obtain the correct credentials for logging in using LDAP.</p></td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray">Change Password URL</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray">Specify a URL that will take users to a site where they can reset their user name or password.<br>This URL is used when <span class="WFVariablesProdNameWF">Workfront</span> users attempt to change their password through the <span class="WFVariablesProdNameWF">Workfront</span> interface.&nbsp;Because the LDAP credentials are used to access <span class="WFVariablesProdNameWF">Workfront</span>, users need to be redirected to a page where they can change their LDAP password instead of completing this activity through <span class="WFVariablesProdNameWF">Workfront</span>.</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray">Certificate</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray">If SSL/TLS is selected, you must upload a valid SSL certificate to ensure a secure&nbsp;connection between the directory service and <span class="WFVariablesProdNameWF">Workfront</span>.&nbsp;For OnDemand accounts, a certificate is always required. You obtain this certificate from your LDAP system administrator.&nbsp;Detailed instructions on installing a valid certificate for LDAPS on LDAP can be found from Microsoft.</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray">Admin Exemption</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray">Select this option to allow system administrators to access <span class="WFVariablesProdNameWF">Workfront</span> via the native <span class="WFVariablesProdNameWF">Workfront</span>&nbsp;login screen with <span class="WFVariablesProdNameWF">Workfront</span>&nbsp;login credentials. If this option is not selected, <span class="WFVariablesProdNameWF">Workfront</span> administrators must use their LDAP user name and password.<p><span class="WFVariablesProdNameWF">Workfront</span>&nbsp;first attempts to log in to <span class="WFVariablesProdNameWF">Workfront</span> via&nbsp;LDAP&nbsp;for users with the <span class="WFVariablesProdNameWF">Workfront</span> System Administrator access level. If the LDAP authentication fails, <span class="WFVariablesProdNameWF">Workfront</span>&nbsp;uses local authentication for <span class="WFVariablesProdNameWF">Workfront</span> administrators.</p><p>We recommend that you always have this option selected, to provide your <span class="WFVariablesAdminWF">Workfront administrator</span> a way for logging into <span class="WFVariablesProdNameWF">Workfront</span> in the event that your LDAP server is temporarily unavailable.</p></td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray">Enable</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray">Select this option to activate SSO on the <span class="WFVariablesProdNameWF">Workfront</span> system. Ensure that you have communicated login instructions to your users.<p>After you enable your SSO configuration&nbsp;in <span class="WFVariablesProdNameWF">Workfront</span>, you must update users for SSO to enable the&nbsp;<b>Only Allow LDAP Authentication</b> setting for all users.</p><p>For more information about updating users for SSO, see <a href="update-users-SSO.md" class="MCXref xref">Update users for single sign-on</a>.</p><p>For more information about user settings, see <a href="edit-a-users-profile.md" class="MCXref xref">Edit a user's profile</a>.</p></td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-LightGray">Confirm Configuration</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-LightGray">Verify that your <span class="WFVariablesProdNameWF">Workfront</span> account can connect to the LDAP server using the connection information and credentials provided.<p>Click <b>Test Connection</b>, then specify the <b>Username</b>&nbsp;and <b>Password</b> for accessing the directory service, then click <b>Test Connection</b>.</p><p><img src="assets/sso-active-directory-and-ladap-test-connection-600x285.png" alt="sso_active_directory_and_ladap_test_connection.png" style="width: 600;height: 285;"></p><p>You should receive an on-screen notification that the connection was successful.</p></td> 
  </tr> 
 </tbody> 
</table>


1. Click **Save** to save the LDAP configuration.


