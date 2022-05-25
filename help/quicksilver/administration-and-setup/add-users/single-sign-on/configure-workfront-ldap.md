---
filename: configure-workfront-ldap
user-type: administrator
product-area: system-administration;setup
navigation-topic: single-sign-on-in-workfront
title: Configure Adobe Workfront with LDAP
description: Configure Adobe Workfront with LDAP
---

# Configure Adobe Workfront with LDAP

<!--
<p style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">**DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. **</p>
-->

{{important-admin-console-onboard}}

>[!IMPORTANT]
>
>Lightweight Directory Access Protocol (LDAP) is now supported only in a limited capacity as a single sign-on (SSO) option; it will be removed from the product in 2020. We recommend moving to Security Assertion Markup Language (SAML) 2.0. For more information, see [Configure Adobe Workfront with SAML 2.0](../../../administration-and-setup/add-users/single-sign-on/configure-workfront-saml-2.md).

## Access requirements

You must have the following access to perform the steps in this article: 

<table> 
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
   <td> <p>You must be a Workfront administrator.</p> <p><b>NOTE</b>: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Connect Adobe Workfront with an LDAP Directory Server

1. Click the **Main Menu** icon ![](assets/main-menu-icon.png) in the upper-right corner of Adobe Workfront, then click **Setup** ![](assets/gear-icon-settings.png).

1. In the left panel, click **System** > **Single Sign-On (SSO)**.

1. In the **Type** drop-down list, click **LDAP**.

1. Specify the following information:

   <table> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Server</td> 
      <td> <p>The URL of the LDAP server where your directory service is running.</p> <p>For example, <code>ldap://hostname.com</code>.<br>Or, if the LDAP server requires an SSL connection, <code>ldaps://hostname.com</code>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Port</td> 
      <td>The port number used for LDAP communication. The default port number for non-secure LDAP connections is 389. The default port number for secure LDAP connections (LDAPS) is 636.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Search Base</td> 
      <td>Specify where in the LDAP directory tree Workfront should find and synchronize initial user information from User objects. This is the container where Workfront begins searching for users on the LDAP server.<br>Use the following format: ou=people,dc=example,dc=com</td> 
     </tr> 
     <tr> 
      <td role="rowheader">SSL/TLS</td> 
      <td>Select this option to encrypt communication between the LDAP server and Workfront. This option is enforced for all OnDemand accounts.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Auto-Provision Users</td> 
      <td>When this option is enabled, Workfront automatically creates a user in the system when a new user with an LDAP username and password attempts to log in to Workfront for the first time. In order for users to be created in Workfront, you need to map Workfront data attributes with the LDAP data attributes.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Attribute Synchronization</td> 
      <td>Click <strong>Map User Attributes</strong>, select the Workfront User Attribute that you want to map from the drop-down list, then specify the corresponding Directory Attribute in the Active Directory server. You can also specify a Default Value for the attribute if you want one to be set. Click <strong>Add Mapping</strong> to include additional attributes, then click <strong>Save</strong> when you are finished.<p><b>IMPORTANT</b>:  Workfront attempts to map these attributes every time a user with these attributes logs into the system. If you have existing users in the system, make sure you are not overwriting their current access level, or any other attributes, by applying this mapping. </p><p>You can map the following Workfront attributes:</p> 
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
       </ul><p>If a user attempts to log in without using SSO and was created using auto-provisioning, it will appear that the their login is not working, or that their username/password combination is wrong. The user will either need to log in using their email address and Workfront password, or obtain the correct credentials for logging in using LDAP.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Change Password URL</td> 
      <td>Specify a URL that will take users to a site where they can reset their user name or password.<br>This URL is used when Workfront users attempt to change their password through the Workfront interface. Because the LDAP credentials are used to access Workfront, users need to be redirected to a page where they can change their LDAP password instead of completing this activity through Workfront.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Certificate</td> 
      <td>If SSL/TLS is selected, you must upload a valid SSL certificate to ensure a secure connection between the directory service and Workfront. For OnDemand accounts, a certificate is always required. You obtain this certificate from your LDAP system administrator. Detailed instructions on installing a valid certificate for LDAPS on LDAP can be found from Microsoft.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Admin Exemption</td> 
      <td>Select this option to allow system administrators to access Workfront via the native Workfront login screen with Workfront login credentials. If this option is not selected, Workfront administrators must use their LDAP user name and password.<p>Workfront first attempts to log in to Workfront via LDAP for users with the Workfront System Administrator access level. If the LDAP authentication fails, Workfront uses local authentication for Workfront administrators.</p><p>We recommend that you always have this option selected, to provide your Workfront administrator a way for logging into Workfront in the event that your LDAP server is temporarily unavailable.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Enable</td> 
      <td>Select this option to activate SSO on the Workfront system. Ensure that you have communicated login instructions to your users.<p>After you enable your SSO configuration in Workfront, you must update users for SSO to enable the <strong>Only Allow LDAP Authentication</strong> setting for all users.</p><p>For more information about updating users for SSO, see <a href="../../../administration-and-setup/add-users/single-sign-on/update-users-sso.md" class="MCXref xref">Update users for single sign-on</a>.</p><p>For more information about user settings, see <a href="../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref">Edit a user's profile</a>.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Confirm Configuration</td> 
      <td>Verify that your Workfront account can connect to the LDAP server using the connection information and credentials provided.<p>Click <strong>Test Connection</strong>, then specify the <strong>Username</strong> and <strong>Password</strong> for accessing the directory service, then click <strong>Test Connection</strong>.</p><p><img src="assets/sso-active-directory-and-ladap-test-connection-350x166.png" alt="sso_active_directory_and_ladap_test_connection.png" style="width: 350;height: 166;"></p><p>You should receive an on-screen notification that the connection was successful.</p></td> 
     </tr> 
    </tbody> 
   </table>

1. Click **Save** to save the LDAP configuration.

