---
user-type: administrator
product-area: system-administration;user-management;setup
navigation-topic: security
title: Configure System Preferences
description: As an Adobe Workfront administrator, you can configure preferences for your Workfront system, including security preferences.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: f92ceed7-b191-425b-9fff-1b0947f32db8
---
# Configure system preferences

<!--
DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.</p>
-->

<!--Audited: 05/2024-->

{{important-admin-console-onboard}}

As an Adobe Workfront administrator, you can configure preferences for your Workfront system, including:

* Access to Workfront from mobile apps and other integrated applications
* Rules for embedding Workfront in an iframe

Changes that you make in the system preferences impact all users in your system, and their experience in Workfront.

We recommend that you configure your system preferences during the Workfront implementation and only occasionally revisit them after that.

## Access requirements

+++ Expand to view access requirements for the functionality in this article.

You must have the following access to perform the steps in this article: 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan</td> 
   <td>Any</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license</td> 
   <td><p>New: Standard</p>
   <p>or</p>
   <p>Current: Plan</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>You must be a Workfront administrator.</p></td> 
  </tr> 
 </tbody> 
</table>

For more detail about the information in this table, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Configure your system preferences

{{step-1-to-setup}}

1. In the left panel, click **System** > **Preferences**.

1. Select any of the following fields to establish the settings for your organization:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p>Enable fast release process</p> </td> 
      <td>Lets you enable monthly Workfront releases for your organization instead of quarterly releases.</p><p>For more information about the fast release process, see <a href="/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md" class="MCXref xref">Enable or disable fast releases for your organization</a>.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Allow embedding of Workfront in an iframe</p> </td> 
      <td>Lets you embed Workfront in an iframe.<p>This option is disabled by default.</p><p><b>IMPORTANT</b>: Displaying a web-based application in an iframe makes the application susceptible to a click-jacking security vulnerability.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Allow SAML 2.0 authentication in Office 365 add-ins</td> 
      <td> <p>Lets you embed Workfront in an iframe only for Office 365 add-ins when Workfront is integrated with a SAML 2.0 single sign-on solution. </p> <p>This option is enabled by default.</p> <p><b>NOTE</b>:  If you enable the option above, <strong>Allow embedding of Workfront in an iframe</strong>, the option <strong>Allow SAML 2.0 authentication in Office 365 add-ins</strong> is enabled and dimmed.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Enable the use of session information when creating External Page URLs</td> 
      <td> <p>Allows users to use the Session ID information of a site when adding an External Page to a Dashboard.</p> <p>This option is insecure and off by default. It is recommended to use OAuth for integrations instead.</p> <p>For more information about adding External Pages to a Dashboard, see <a href="../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/embed-external-web-page-dashboard.md" class="MCXref xref">Embed an external web page in a dashboard</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Let people use Workfront's mobile applications and the Workfront Outlook Add-In</td> 
      <td> <p>Allows users to access the mobile apps (Workfront View for iPad and mobile phone apps) and the Workfront Outlook app.</p> <p>This option is enabled by default. </p> <p>For information about Workfront View, see <a href="../../../workfront-basics/mobile-apps/using-workfront-view/use-workfront-view.md" class="MCXref xref">Use Adobe Workfront View</a>. For more information about the mobile apps, see <a href="../../../workfront-basics/mobile-apps/using-the-workfront-mobile-app/use-the-mobile-app.md" class="MCXref xref">Use the Adobe Workfront mobile app: article index</a>.</p> <p>For more information about the Outlook plugin, see <a href="../../../workfront-integrations-and-apps/using-workfront-with-outlook/set-up-workfront-for-outlook.md" class="MCXref xref">Set up Adobe Workfront for Outlook</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Collaborate with people without Workfront accounts by using email addresses</p> </td> 
      <td>Allows Workfront users to share certain items with people without a Workfront account by including their email address instead of their name. Users can share the following items with external users by using their email address:
       <ul>
        <li>Document<br></li>
        <li>Document request<br></li>
        <li>Document approval</li>
        <li>Calendar</li>
       </ul><p>This option is enabled by default.</p> <p><b>Important</b>: The External User access level is unavailable in your Workfront instance if this option is disabled. For more information, see <a href="../../../administration-and-setup/add-users/access-levels-and-object-permissions/default-access-levels-in-workfront.md" class="MCXref xref">Built-in access levels</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Require external users to register with a password</td> 
      <td> <p>Requires external users to register before they are able to view items in Workfront. By default, this option is disabled. When you enable this option, people without a Workfront account who are included in certain updates by their email address, will be prompted to create an account before they can view the item they are included on. This creates an External User account for them.</p> <p>This option is disabled by default.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Automatically log users out after</td> 
      <td> Lets you specify when a user is logged out of Workfront, after a period of inactivity. By default, users are logged out after 8 hours of inactivity. <p>This option also affects Workfront customers who are using a single sign-on solution.</p> <p>This setting is not available to organizations that have been migrated to Adobe IMS.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Automatically log mobile users out after </td> 
      <td>Lets you specify when a user is logged out of the Workfront application, after a period of inactivity. By default, users are logged out after 7 days of inactivity. <p>This option also affects Workfront customers who are using a single sign-on solution.</p> <p>This setting is not available to organizations that have been migrated to Adobe IMS.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Custom Help URL</td> 
      <td>Lets you define an internal custom help site for the Main Menu help icon to go to. For more information, see <a href="/help/quicksilver/administration-and-setup/customize-workfront/brand-workfront/configure-custom-help-url.md">Configure a custom help URL</a>.</p></td> 
     </tr>
     <tr> 
      <td role="rowheader">Users in the system will default to seeing the New Home experience </td> 
      <td>Lets you specify whether users will see the New Home experience by default. When enabled, users will see the New Home experience by default, but can still opt to enable or disable New Home on an individual basis. When disabled, users will not see the banner that allows them to switch to New Home—however, they can still navigate to their New Home page by manually entering <code>/home/workspaces</code> at the end of their instance URL. This setting is enabled by default.</td> 
     </tr>
     <tr> 
      <td role="rowheader">Enable the Priorities worklist </td> 
      <td>Lets you choose to enable or disable the Priorities worklist experience for your users. Users will still see the Priorities icons in Workfront, but they will not have access to the functionality. For more information about Priorities, see <a href="/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/wf-preview-sandbox-environment.md">Get started with Priorities</a>.</td> 
     </tr>
     <tr> 
      <td role="rowheader">Test Environments</td> 
      <td>Lets you access your Workfront test environments. For more information, see <a href="/help/quicksilver/workfront-basics/priorities/get-started-with-priorities.md">The Adobe Workfront Preview Sandbox Environment</a>.</p></td> 
    </tbody> 
   </table>

1. Click **Save**.

   The changes that you saved here affect the experience of all the users in Workfront and anyone who interacts with the system as an external user.
