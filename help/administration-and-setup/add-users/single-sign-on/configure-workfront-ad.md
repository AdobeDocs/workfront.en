---
filename: configure-workfront-ad
user-type: administrator
product-area: system-administration
navigation-topic: single-sign-on-in-workfront
title: Configure Adobe Workfront with Active Directory
description: Since this is no longer supported, I am not going to update the article for NWE/phase 2
---

# Configure `Adobe Workfront` with Active Directory

<!--
Since this is no longer supported, I am not going to update the article for NWE/phase 2
-->

>[!IMPORTANT]
>
>The procedure described on this page applies only to organizations that are not yet onboarded to the Adobe Admin Console.
>
>If your organization has been onboarded to the Adobe Admin Console, see [Platform-based administration differences (Adobe Workfront/Adobe Business Platform)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

>[!IMPORTANT]
>
>Active Directory is now supported only in a limited capacity as a Single Sign-On (SSO) option; it will be removed from the product in 2020. If you want to continue to use Active Directory as an SSO option, see [Configure Adobe Workfront with SAML 2.0 using ADFS](../../../administration-and-setup/add-users/single-sign-on/configure-workfront-saml-2-adfs.md).

To connect  `Adobe Workfront` with an Active Directory Server:

<ol> 
 <li value="1">Click the <span class="bold">Main Menu</span> icon <img src="assets/main-menu-icon.png"> in the upper-right corner of <span>Adobe Workfront</span>, then click <span class="bold">Setup</span> <img src="assets/gear-icon-settings.png">.<br></li> 
 <li value="2">Expand <span class="bold">System</span>, then click <span class="bold">Single Sign-On (SSO)</span>.</li> 
 <li value="3"> <p>In the <span class="bold">Type</span> drop-down list, select <span class="bold">Active Directory</span>.<br></p> </li> 
 <li value="4"> <p>Specify the following information:</p> 
  <table cellspacing="0"> 
   <col> 
   <col> 
   <tbody> 
    <tr> 
     <td role="rowheader">Server</td> 
     <td> <p>The&nbsp;URL of the Active Directory server where your directory service is running.</p> <p>For example, <i>ldap://hostname.com</i>. If the Active Directory server requires an SSL connection, the URL is, for example:&nbsp;<i>ldaps://hostname.com</i>.</p> </td> 
    </tr> 
    <tr> 
     <td role="rowheader">Port</td> 
     <td>The port number used for LDAP&nbsp;communication with the Active Directory server. The default port number for non-secure LDAP connections is 389. The default port number for secure LDAP connections (LDAPS) is 636.</td> 
    </tr> 
    <tr> 
     <td role="rowheader">Search Base</td> 
     <td>Specify where&nbsp;in the LDAP directory tree&nbsp;<span>Workfront</span>&nbsp;should find and synchronize initial user information from User objects. This is the container where <span>Workfront</span>&nbsp;begins&nbsp;searching for users on the Active Directory server.<br>Use the following format: ou=people,dc=example,dc=com</td> 
    </tr> 
    <tr> 
     <td role="rowheader">Active Directory Domain</td> 
     <td>Specify the Windows domain of the Active Directory connection. Obtain this information from your Active Directory <span>Workfront administrator</span>.</td> 
    </tr> 
    <tr> 
     <td role="rowheader">Auto-Provision Users</td> 
     <td>When this option is enabled,&nbsp;<span>Workfront</span> automatically&nbsp;creates a user in the system when a new user with a user name and password in&nbsp;Active Directory&nbsp; attempts to log in to <span>Workfront</span> for the first time. In order for users to be created in <span>Workfront</span>, you need to map <span>Workfront</span> data attributes with the data attributes in Active Directory. See the explanation about Attribute Synchronization below.</td> 
    </tr> 
    <tr> 
     <td role="rowheader">Attribute Synchronization</td> 
     <td> <p>Click <span class="bold">Map User Attributes</span>, select the <span>Workfront</span> User Attribute that you want to map from the drop-down list, then&nbsp;specify the corresponding Directory Attribute in the Active Directory server.&nbsp;You can also specify a Default Value for the attribute&nbsp;if you want one to be set. Click <span class="bold">Add Mapping</span> to include additional attributes, then click <span class="bold">Save</span> when you are finished.<br>When a discrepancy exists between user information in <span>Workfront</span> and Active Directory, and Active Directory is enabled, the information in the Active Directory will update the user information in <span>Workfront</span>.</p> <note type="important">
       <span>Workfront</span> attempts to map these attributes every time a user with these attributes logs into the system. If you have existing users in the system, make sure you are not overwriting their current access level, or any other attributes, by applying this mapping.
      </note> <p>You can map the following <span>Workfront</span> attributes:</p> 
      <ul> 
       <li>Access Level</li> 
       <li>Address</li> 
       <li>Address2</li> 
       <li>Billing Per Hour</li> 
       <li>City</li> 
       <li>Company</li> 
       <li>Cost Per Hour</li> 
       <li>Email Address</li> 
       <li>Extension</li> 
       <li>First Name</li> 
       <li>Home Group</li> 
       <li>Home Team</li> 
       <li>Job Role</li> 
       <li>Last Name</li> 
       <li>Layout Template</li> 
       <li>Manager</li> 
       <li>Mobile Phone</li> 
       <li>Phone Number</li> 
       <li>Postal Code</li> 
       <li>Schedule</li> 
       <li>State</li> 
       <li>Timesheet Profile</li> 
       <li>Title</li> 
      </ul> </td> 
    </tr> 
    <tr> 
     <td role="rowheader">Change Password URL</td> 
     <td>Specify a URL that provides the ability for users to re-set their user name or password.<br>This URL is used when <span>Workfront</span> users attempt to change their password through the <span>Workfront</span> interface.&nbsp;Because the Active Directory&nbsp;credentials are used to access <span>Workfront</span>, users need to be redirected to a page where they can change their&nbsp;password in Active Directory instead of completing this activity through <span>Workfront</span>.</td> 
    </tr> 
    <tr> 
     <td role="rowheader">Certificate</td> 
     <td>If <span class="bold">SSL/TLS</span> is selected, you must upload a valid SSL certificate to ensure a secure&nbsp;connection between the directory service and <span>Workfront</span>.&nbsp;For OnDemand accounts, a certificate is always required.</td> 
    </tr> 
    <tr> 
     <td role="rowheader">Admin Exemption</td> 
     <td> <p>Select this option to allow <span>Workfront administrator</span>s to access <span>Workfront</span> via the native <span>Workfront</span>&nbsp;login screen with <span>Workfront</span>&nbsp;login credentials. If this option is not selected, <span>Workfront administrator</span>s must use their Active Directory user name and password.</p> <p><span>Workfront</span>&nbsp;first attempts to log in to <span>Workfront</span> via&nbsp;LDAP&nbsp;for users with the <span>Workfront administrator</span> access level. If the authentication to Active Directory fails, <span>Workfront</span> uses <span>Workfront</span>&nbsp;authentication for <span>Workfront administrator</span>s.</p> <p>We recommend that you always have this option selected, to provide your <span>Workfront administrator</span> a way for logging into <span>Workfront</span> in the event that your LDAP server is temporarily unavailable.</p> </td> 
    </tr> 
    <tr> 
     <td role="rowheader">Enable</td> 
     <td> <p>Select this option to activate SSO on the <span>Workfront</span> system. Ensure that you have communicated login instructions to your users.</p> <p>After you enable your SSO configuration&nbsp;in <span>Workfront</span>, you must update users for SSO to enable the&nbsp;<span class="bold">Only Allow Active Directory Authentication</span> setting for all users.</p> <p>For more information about updating users for SSO, see <a href="../../../administration-and-setup/add-users/single-sign-on/update-users-sso.md" class="MCXref xref">Update users for single sign-on</a>.</p> <p>For more information about user settings, see <a href="../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref">Edit a user's profile</a>.</p> </td> 
    </tr> 
    <tr> 
     <td role="rowheader">Confirm Configuration</td> 
     <td> <p>Verify that your <span>Workfront</span> account can connect to the Active Directory server using the connection information and credentials provided.&nbsp;Click<span class="bold"> Test Connection</span>.</p> <p> <img src="assets/sso-active-directory-test-connection-350x166.png" alt="sso_active_directory_test_connection.png" style="width: 350;height: 166;"> <br> </p> <p>Specify the&nbsp;<span class="bold">Username</span> and <span class="bold">Password</span>&nbsp;for a user who can successfully log in to your environment using Active Directory. These are their Active Directory credentials.</p> <p>Click <span class="bold">Test Connection</span> to test the connection from <span>Workfront</span> to your Active Directory server.</p> <p>You should receive an on-screen confirmation when the connection is successful.</p> </td> 
    </tr> 
   </tbody> 
  </table> </li> 
 <li value="5">Click <span class="bold">Save</span> to save the Active Directory configuration.</li> 
</ol>

