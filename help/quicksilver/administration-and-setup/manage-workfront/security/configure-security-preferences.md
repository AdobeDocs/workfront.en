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
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/46D3BBajFk39FP-dMDk0SuSSGM5nYPKas11Bs159R9Y
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
    internal-label: Administration
  - id: f48b5020-b9cd-4d99-bc6e-42c35e90c1f8
    internal-label: Integrations
subfeature_v2:
  - id: e147ce9d-7675-49bd-8a32-44f27d865560
    internal-label: Get started
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
    internal-label: Admin
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
    internal-label: Reporting
  - id: b5ce8718-c3af-4fdb-a1a9-fca32f83a87c
    internal-label: Implementation
  - id: bce87dde-a4ab-44c9-8a18-ad66e4ddb377
    internal-label: Customer experience
  - id: d095671a-1355-40aa-8b5f-06c33c68080b
    internal-label: Security
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
---
# Configure system preferences

{{preview-fast-release-general}}

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

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront package</td> 
   <td><p>Any</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license</td> 
   <td><p>Standard</p><p>Plan</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>You must be a Workfront administrator.</p> </p> </td> 
  </tr> 
 </tbody> 
</table>

For information, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md). 

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
      <td role="rowheader">Let people use Workfront's mobile applications</td> 
      <td> <p>Allows users to access the mobile apps (Workfront View for iPad and mobile phone apps)</p> <p>This option is enabled by default. </p> <p>For information about Workfront View, see <a href="../../../workfront-basics/mobile-apps/using-workfront-view/use-workfront-view.md" class="MCXref xref">Use Adobe Workfront View</a>. For more information about the mobile apps, see <a href="../../../workfront-basics/mobile-apps/using-the-workfront-mobile-app/use-the-mobile-app.md" class="MCXref xref">Use the Adobe Workfront mobile app: article index</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Collaborate with people without Workfront accounts by using email addresses</p> </td> 
      <td>Allows Workfront users to share certain items with people without a Workfront account by including their email address instead of their name. Users can share the following items with external users by using their email address:
       <ul>
        <li>Document<br></li>
        <li>Document request<br></li>
        <li>Document approval</li>
        <li>Calendar</li>
       </ul><p>This option is enabled by default.</p> <p><b>IMPORTANT</b>: The External User access level is unavailable in your Workfront instance if this option is disabled. For more information, see <a href="../../../administration-and-setup/add-users/access-levels-and-object-permissions/default-access-levels-in-workfront.md" class="MCXref xref">Built-in access levels</a>.</p> </td> 
     </tr> 
     <!--
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
     -->
     <tr> 
      <td role="rowheader">Custom Help URL</td> 
      <td>Lets you define an internal custom help site for the Main Menu help icon to go to. For more information, see <a href="/help/quicksilver/administration-and-setup/customize-workfront/brand-workfront/configure-custom-help-url.md">Configure a custom help URL</a>.</p></td> 
     </tr>
    <tr> 
      <td role="rowheader">Disable auto-upgrade within Access Levels</td> 
      <td>You can disable the auto-upgrade process for Contributor access levels. When this setting is checked, Contributor-license users who have exceeded their approval decision limit must be manually upgraded to a new license by the administrator.</p></td> 
     </tr>
     <tr> 
      <td role="rowheader">Enable the Priorities worklist </td> 
      <td>Lets you choose to enable or disable the Priorities worklist experience for your users. Users will still see the Priorities icons in Workfront, but they will not have access to the functionality. For more information about Priorities, see <a href="/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/wf-preview-sandbox-environment.md">Get started with Priorities</a>.</td> 
     </tr>
     <tr>
      <td><span class="preview">Always enforce required fields in bulk edit</span></td>
      <td><span class="preview"><p>Lets you choose whether to force users to enter information in required fields when bulk editing objects.</p> <p>When this option is selected, required fields must have values before saving in bulk edit mode. If the required field is missing a value for at least one bulk selected object, saving is not permitted.</p> <p>When this option is not selected, required fields are only enforced when a user modifies the field. If a field is not modified, it is treated as optional and not validated.</p></span></td>
     </tr>
     <tr> 
      <td role="rowheader">Storage Preferences </td> 
      <td>In this section you can enable the Adobe cloud preferences. Lets you choose to enable or disable Adobe cloud storage for your entire organization or for specific groups. 
      <p>Update the following information:</p>
      <ul><li><b>Default</b>: Choose Legacy Workfront storage or Adobe cloud storage</li>
      <li><b>Allow users to select storage provider</b>: This allows users to choose between the two storage types when creating Workfront objects.</li>
      <li><b>Applies to</b>: Choose whether the default settings apply to the entire organization or to specific groups</li>
      <li><b>Select portfolios to convert to Adobe cloud storage</b>: Select portfolios that you would like to convert automatically from Workfront legacy storage to Adobe cloud storage. The portfolios are converted when you save the System Preferences.</li></ul>     
    For more information about Adobe cloud storage, see <a href="/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-esm.md">Enable Adobe cloud storage for your organization</a>.</td></tr>
    <tr> 
      <td role="rowheader">Select portfolios to convert to Adobe cloud storage </td> 
      <td>Lets you convert existing legacy Workfront storage portfolios to Adobe cloud storage. For more information, see <a href="/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/convert-portfolios-to-acs.md">Convert legacy portfolios to Adobe cloud storage</a>.</td> 
     </tr>
     <tr> 
      <td role="rowheader">Enable AI </td> 
      <td>By turning on the settings in the AI preferences area, you can enable AI, including AI Assistant. <p><b>NOTE</b>: Your organization must meet specific requirements to enable AI. For more information about AI, including the requirements, see <a href="/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md">AI Assistant overview</a>.</p></td> 
     </tr>
    <tr> 
      <td role="rowheader">AI Form Fill </td> 
      <td>Allow people to use Form Fill with AI to automatically fill a request form. For more information, see <a href="/help/quicksilver/manage-work/requests/create-requests/autofill-from-prompt-document.md">Use Form Fill powered by AI to fill in a request using prompts or documents</a>.</p></td> 
     </tr>
     <tr> 
      <td role="rowheader">Intelligent Auto-complete in Request forms </td> 
      <td>Lets you choose to enable the ability to auto-complete request forms based on previous request data. For more information about Form Auto-Complete, see <a href="/help/quicksilver/manage-work/requests/create-requests/autofill-suggestions-from-previous.md">Auto-fill a request from previous data</a>.</td> 
     </tr>
    <tr> 
      <td role="rowheader">Planning Designer</td> 
      <td>This is available only to customers who have purchased a Workfront Planning package. Turning on this setting allows your users to create and edit workspaces using the Planning Designer. For information, see <a href="/help/quicksilver/planning/general/planning-ai-designer.md">Get started with the Adobe Workfront Planning Designer</a>.</td> 
     </tr>
     <tr> 
      <td role="rowheader">Opt in to AI Betas </td> 
      <td>Lets you choose to enable AI features that are currently in Beta. If you enable this option, you can then select which AI Beta features to enable. For more information about each AI Beta feature, click the information icon next to that feature.</td> 
     </tr>
     <tr> 
      <td role="rowheader"><span class="preview">Read-only MCP tools</span></td> 
      <td><span class="preview">Lets the Workfront MCP server perform read actions on Workfront data — for example, finding or listing projects, tasks, or other items. This option is enabled by default.<p>For more information about the Workfront MCP server, see <a href="/help/quicksilver/workfront-basics/workfront-mcp-server/configure-workfront-mcp-server.md">Configure the Adobe Workfront MCP server</a>.</p></span></td> 
     </tr>
     <tr> 
      <td role="rowheader"><span class="preview">Write MCP tools</span></td> 
      <td><span class="preview">Lets the Workfront MCP server perform create, update, and delete actions on Workfront data. This option is disabled by default.<p>For more information about the Workfront MCP server, see <a href="/help/quicksilver/workfront-basics/workfront-mcp-server/configure-workfront-mcp-server.md">Configure the Adobe Workfront MCP server</a>.</p></span></td> 
     </tr>
     <tr> 
      <td role="rowheader">Test Environments</td> 
      <td>Lets you access your Workfront test environments. For more information, see <a href="/help/quicksilver/workfront-basics/priorities/get-started-with-priorities.md">The Adobe Workfront Preview Sandbox Environment</a>.</p></td> 
    </tbody> 
   </table>

1. Click **Save**.

   The changes that you saved here affect the experience of all the users in Workfront and anyone who interacts with the system as an external user.
