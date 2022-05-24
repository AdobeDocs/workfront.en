---
filename: configure-security-preferences
user-type: administrator
product-area: system-administration;user-management;setup
navigation-topic: security
title: Configure system security preferences
description: Configure system security preferences
---

# Configure system security preferences

<!--
DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.</p>
-->

{{important-admin-console-onboard}}


As an Adobe Workfront administrator, you can configure security preferences for your Workfront system:

* Access to Workfront from mobile apps and other integrated applications
* Rules for embedding Workfront in an iframe

Changes that you make in the system preferences impact all users in your system, and their experience in Workfront.

We recommend that you configure your system security preferences during the Workfront implementation and only occasionally revisit them after that.

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
   <td> <p>You must be a Workfront administrator.</p> <p><b>Note<>: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Configure your system security preferences

1. Click the **Main Menu** icon ![](assets/main-menu-icon.png) in the upper-right corner of Adobe Workfront, then click **Setup** ![](assets/gear-icon-settings.png).

1. In the left panel, click **System** > **Preferences**.  

1. In the **Security** section, select any of the following fields to establish the security settings for your organization:

   <table> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p>Allow embedding of <strong>Workfront</strong> in an iframe</p> </td> 
      <td>Lets you embed Workfront in an iframe.<p>This option is disabled by default.</p><p>Important: Displaying a web-based application in an iframe makes the application susceptible to a click-jacking security vulnerability.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Allow SAML 2.0 authentication in Office 365 add-ins</td> 
      <td> <p>Lets you embed Workfront in an iframe only for Office 365 add-ins when Workfront is integrated with a SAML 2.0 single sign-on solution. </p> <p>This option is enabled by default.</p> <p>Note:  If you enable the option above, <strong>Allow embedding of Workfront in an iframe</strong>, the option <strong>Allow SAML 2.0 authentication in Office 365 add-ins</strong> is enabled and dimmed.<br></p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Enable the use of session information when creating External Page URLs</td> 
      <td> <p>Allows users to use the Session ID information of a site when adding an External Page to a Dashboard.<br></p> <p>For more information about adding External Pages to a Dashboard, see <a href="../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/embed-external-web-page-dashboard.md" class="MCXref xref">Embed an external web page in a dashboard</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Let people use Workfront's mobile applications and the <strong>Workfront</strong> Outlook Add-In</td> 
      <td> <p>Allows users to access the mobile apps (Workfront View for iPad and mobile phone apps) and the Workfront Outlook app.</p> <p>This option is enabled by default. </p> <p>For information about Workfront View, see <a href="../../../workfront-basics/mobile-apps/using-workfront-view/use-workfront-view.md" class="MCXref xref">Use Adobe Workfront View</a>. For more information about the mobile apps, see <a href="../../../workfront-basics/mobile-apps/using-the-workfront-mobile-app/use-the-mobile-app.md" class="MCXref xref">Use the Adobe Workfront mobile app</a>.</p> <p>For more information about the Outlook plugin, see <a href="../../../workfront-integrations-and-apps/using-workfront-with-outlook/set-up-workfront-for-outlook.md" class="MCXref xref">Set up Adobe Workfront for Outlook</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Collaborate with people without Workfront accounts by using email addresses</p> </td> 
      <td>Allows Workfront users to share certain items with people without a Workfront account by including their email address instead of their name. Users can share the following items with external users by using their email address:
       <ul>
        <li>Document<br></li>
        <li>Document request<br></li>
        <li>Document approval</li>
        <li>Calendar</li>
       </ul><p>This option is enabled by default.</p> <p><b>Important</b>: The External User access level is unavailable in your Workfront instance if this option is disabled. For more information, see <a href="../../../administration-and-setup/add-users/access-levels-and-object-permissions/default-access-levels-in-workfront.md" class="MCXref xref">Built-in access levels in Workfront</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Require external users to register with a password</td> 
      <td> <p>Requires external users to register before they are able to view items in Workfront. By default, this option is disabled. When you enable this option, people without a Workfront account who are included in certain updates by their email address, will be prompted to create an account before they can view the item they are included on. This creates an External User account for them.</p> <p>This option is disabled by default.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Automatically log users out after</td> 
      <td> <p><b>Note</b>: This is not currently available. We are working on authentication enhancements that will allow you to log out inactive users automatically after a period of time that you choose.  <!--
          TEMPORARY note! Remove and update how this works after IMS takes over. There's another note like this in - Workfront basics/Manage your account and profile/Managing Your Workfront Account/log-out-of-workfront.html
        --></p> <p>This option lets you specify when a user is logged out of Workfront, after a period of inactivity. By default, users are logged out after 8 hours of inactivity. </p> <p>This option also affects Workfront customers who are using a single sign-on solution.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Automatically log mobile users out after </td> 
      <td>Lets you specify when a user is logged out of the Workfront application, after a period of inactivity. By default, users are logged out after 7 days of inactivity. <p>This option also affects Workfront customers who are using a single sign-on solution.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Enable Zoom integration in the updates stream</strong> </td> 
      <td> <p>Lets you enable or disable the Zoom integration in the Updates area for all users in the organization.<br>The Zoom integration allows users to add a Zoom meeting URL to a comment or reply in the Updates area. For more information, see <a href="https://one.workfront.com/s/article/Using-the-Zoom-integration?language=en_US">Using the Zoom integration</a>. Also see the section <a href="../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md#add" class="MCXref xref">Add an update to a work item</a> in the article<a href="../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md" class="MCXref xref">Update work</a>.</p> <p>Users can uninstall the Zoom integration in their personal instance of Workfront. For more information, see <a href="https://one.workfront.com/s/article/Uninstalling-the-Zoom-integration?language=en_US">Uninstalling the Zoom integration</a>.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Click **Save**.

   The changes that you saved here affect the experience of all the users in Workfront and anyone who interacts with them as an external user.

