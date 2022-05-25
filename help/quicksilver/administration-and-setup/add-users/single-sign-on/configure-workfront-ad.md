---
filename: configure-workfront-ad
user-type: administrator
product-area: system-administration
navigation-topic: single-sign-on-in-workfront
title: Configure Adobe Workfront with Active Directory
description: Configure Adobe Workfront with Active Directory
---

# Configure Adobe Workfront with Active Directory

<!--
<p style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">**DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. **</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">Since this is no longer supported, I am not going to update the article for NWE/phase 2</p>
-->

{{important-admin-console-onboard}}


>[!IMPORTANT]
>
>Active Directory is now supported only in a limited capacity as a Single Sign-On (SSO) option; it will be removed from the product in 2020. If you want to continue to use Active Directory as an SSO option, see [Configure Adobe Workfront with SAML 2.0 using ADFS](../../../administration-and-setup/add-users/single-sign-on/configure-workfront-saml-2-adfs.md).

To connect&nbsp;Adobe Workfront with an Active Directory Server:

1. Click the **Main Menu** icon ![](assets/main-menu-icon.png) in the upper-right corner of Adobe Workfront, then click **Setup** ![](assets/gear-icon-settings.png).  

1. Expand **System**, then click **Single Sign-On (SSO)**.

1. In the **Type** drop-down list, select **Active Directory**.  

1. Specify the following information:

   <table> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Server</td> 
      <td> <p>The&nbsp;URL of the Active Directory server where your directory service is running.</p> <p>For example, <code>ldap://hostname.com</code>. If the Active Directory server requires an SSL connection, the URL is, for example:&nbsp;<i>ldaps://hostname.com</i>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Port</td> 
      <td>The port number used for LDAP&nbsp;communication with the Active Directory server. The default port number for non-secure LDAP connections is 389. The default port number for secure LDAP connections (LDAPS) is 636.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Search Base</td> 
      <td>Specify where&nbsp;in the LDAP directory tree&nbsp;Workfront&nbsp;should find and synchronize initial user information from User objects. This is the container where Workfront&nbsp;begins&nbsp;searching for users on the Active Directory server.<br>Use the following format: ou=people,dc=example,dc=com</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Active Directory Domain</td> 
      <td>Specify the Windows domain of the Active Directory connection. Obtain this information from your Active Directory Workfront administrator.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Auto-Provision Users</td> 
      <td>When this option is enabled,&nbsp;Workfront automatically&nbsp;creates a user in the system when a new user with a user name and password in&nbsp;Active Directory&nbsp; attempts to log in to Workfront for the first time. In order for users to be created in Workfront, you need to map Workfront data attributes with the data attributes in Active Directory. See the explanation about Attribute Synchronization below.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Attribute Synchronization</td> 
      <td> <p>Click <strong>Map User Attributes</strong>, select the Workfront User Attribute that you want to map from the drop-down list, then&nbsp;specify the corresponding Directory Attribute in the Active Directory server.&nbsp;You can also specify a Default Value for the attribute&nbsp;if you want one to be set. Click <strong>Add Mapping</strong> to include additional attributes, then click <strong>Save</strong> when you are finished.<br>When a discrepancy exists between user information in Workfront and Active Directory, and Active Directory is enabled, the information in the Active Directory will update the user information in Workfront.</p> <p><b>IMPORTANT</b>: Workfront attempts to map these attributes every time a user with these attributes logs into the system. If you have existing users in the system, make sure you are not overwriting their current access level, or any other attributes, by applying this mapping.</p> <p>You can map the following Workfront attributes:</p> 
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
      <td>Specify a URL that provides the ability for users to re-set their user name or password.<br>This URL is used when Workfront users attempt to change their password through the Workfront interface.&nbsp;Because the Active Directory&nbsp;credentials are used to access Workfront, users need to be redirected to a page where they can change their&nbsp;password in Active Directory instead of completing this activity through Workfront.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Certificate</td> 
      <td>If <strong>SSL/TLS</strong> is selected, you must upload a valid SSL certificate to ensure a secure&nbsp;connection between the directory service and Workfront.&nbsp;For OnDemand accounts, a certificate is always required.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Admin Exemption</td> 
      <td> <p>Select this option to allow Workfront administrators to access Workfront via the native Workfront&nbsp;login screen with Workfront&nbsp;login credentials. If this option is not selected, Workfront administrators must use their Active Directory user name and password.</p> <p>Workfront&nbsp;first attempts to log in to Workfront via&nbsp;LDAP&nbsp;for users with the Workfront administrator access level. If the authentication to Active Directory fails, Workfront uses Workfront&nbsp;authentication for Workfront administrators.</p> <p>We recommend that you always have this option selected, to provide your Workfront administrator a way for logging into Workfront in the event that your LDAP server is temporarily unavailable.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Enable</td> 
      <td> <p>Select this option to activate SSO on the Workfront system. Ensure that you have communicated login instructions to your users.</p> <p>After you enable your SSO configuration&nbsp;in Workfront, you must update users for SSO to enable the&nbsp;<strong>Only Allow Active Directory Authentication</strong> setting for all users.</p> <p>For more information about updating users for SSO, see <a href="../../../administration-and-setup/add-users/single-sign-on/update-users-sso.md" class="MCXref xref">Update users for single sign-on</a>.</p> <p>For more information about user settings, see <a href="../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref">Edit a user's profile</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Confirm Configuration</td> 
      <td> <p>Verify that your Workfront account can connect to the Active Directory server using the connection information and credentials provided.&nbsp;Click<strong>Test Connection</strong>.</p> <p> <img src="assets/sso-active-directory-test-connection-350x166.png" alt="sso_active_directory_test_connection.png" style="width: 350;height: 166;"> <br> </p> <p>Specify the&nbsp;<strong>Username</strong> and <strong>Password</strong>&nbsp;for a user who can successfully log in to your environment using Active Directory. These are their Active Directory credentials.</p> <p>Click <strong>Test Connection</strong> to test the connection from Workfront to your Active Directory server.</p> <p>You should receive an on-screen confirmation when the connection is successful.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Click **Save** to save the Active Directory configuration.

