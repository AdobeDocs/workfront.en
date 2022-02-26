---
filename: configure-workfront-aem
title: Configure Workfront with Adobe Experience Manager
user-type: administrator
product-area: system-administration;workfront-integrations;setup
navigation-topic: administrator-integrations
title: Configure Workfront with Adobe Experience Manager
description: As an Adobe Workfront administrator, you can integrate Workfront with Adobe Experience Manager (AEM) Assets and provide your organization with a comprehensive content management solution for the creation, sharing, and maintenance of assets within your workflow.
---

# Configure *Workfront* with Adobe Experience Manager

As an *Adobe Workfront administrator*, you can integrate *Workfront* with Adobe Experience Manager (AEM)&nbsp;Assets and provide your organization with a comprehensive content management solution for the creation,&nbsp;sharing, and maintenance of assets within your workflow.&nbsp;&nbsp;

## Access requirements

You must have the following access to perform the steps in this article:

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><em>Adobe Workfront</em> plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><em>Adobe Workfront</em> license*</td> 
   <td> <p>Plan</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>You must be a <em>Workfront administrator</em>. For information on <em>Workfront administrators</em>, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Grant a user full administrative access</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your *Workfront administrator*.

## *Workfront* for AEM Assets

The *Workfront* for AEM Assets connector allows your organization to do the following:

* Collaborate and manage creative content by linking AEM assets and folders to projects, tasks, issues, and requests in *Workfront*.

  For more information about configuring documentation integrations with third-party applications, see&nbsp; [Configure document integrations](../../administration-and-setup/configure-integrations/configure-document-integrations.md).

* Integrate with the AEM Digital Asset Management (DAM) repository, allowing you to use *Workfront* to manage and share digital assets stored in the DAM.

  For more information about linking documents and asset folders, see &nbsp; [Link documents from external applications](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md).

* Combine and apply metadata from both applications to an asset.
* View an all-inclusive communication stream for an asset.&nbsp;Updates and comments made to an asset either in *Workfront* or AEM Assets are synchronized to the&nbsp;other application, establishing a comprehensive history of communications made to the&nbsp;asset.

  For more information about making comments in *Workfront*, see [Add an update to a document](../../documents/managing-documents/add-update-documents.md).

## Prerequisites for installing the AEM Assets connector

Before you can install the *Workfront* connector for AEM Assets, ensure that the following prerequisites are met:

* AEM Assets installed and configured, version 6.0 or later

  For information about installing AEM Assets, see the [Adobe Experience Manager documentation](https://docs.adobe.com/docs/en/aem/6-2/deploy.html).

* AEM Touch-Optimized&nbsp;User Interface activated

## Install the *Workfront* for AEM Assets connector package

To install the *Workfront* for AEM Assets connector, you must import the connector into AEM&nbsp;as a package using the CRX Package Manager.

<ol> 
 <li value="1"> <p>On a workstation where you have already installed AEM, download the <em>Workfront</em> for AEM Assets Connector installation file.</p> <p>You can get&nbsp;the <em>Workfront</em> for AEM Assets connector from your <em>Workfront</em> representative.</p> </li> 
 <li value="2">Log in to AEM using an administrator account.</li> 
 <li value="3"> <p>Click <span class="bold">Tools</span> > <span class="bold">Deployment</span> > <span class="bold">Packages</span>.</p> <p>The CRX Package Manager opens.</p> </li> 
 <li value="4"> <p>Click <span class="bold">Upload Package.</span></p> <p><span class="bold"><img src="assets/aem-package-manager-upload-350x93.png" alt="aem_package_manager_upload.png" style="width: 350;height: 93;"></span> </p> </li> 
 <li value="5">In the Upload Package dialog box, browse for and select the <em>Workfront</em> Connector package, then click <span class="bold">OK</span>.<br>The package displays in the CRX Package Manager.</li> 
 <li value="6"> <p>Click <span class="bold">Install.</span></p> <p><span class="bold"><img src="assets/installconnector-350x119.png" alt="InstallConnector.png" style="width: 350;height: 119;"><br></span> </p> </li> 
 <li value="7">On the Package dialog box, ignore the advanced settings and click <span class="bold">Install</span>.</li> 
 <li value="8">(Optional) To confirm the connector successfully installed, ensure the following statement displays in the Activity Log:<br><pre>Package installed in <time></pre></li> 
 <li value="9"> <p>Close the CRX Package Manager.</p> <p>The connector is installed and you can now configure AEM Assets to integrate with <em>Workfront</em>.</p> </li> 
 <li value="10">Continue with <a href="#configur" class="MCXref xref">Configure AEM Assets to integrate with Workfront</a>.</li> 
</ol>

## Configure AEM Assets to integrate with *Workfront*

After you install the connector, import the connector package to AEM and configure AEM to link with documents in *Workfront*.

For information on installing the connector, see&nbsp; [Install the Workfront for AEM Assets connector package](#installi).

* [Install the connector package on AEM assets version 6.4 (Touch UI)](#installi2) 
* [Install the connector package on AEM Assets versions 6.3 or older (classic UI)](#installi3) 
* [Configure the AEM Externalizer](#configur3)

### Install the connector package on AEM assets version 6.4 (Touch UI)

<ol> 
 <li value="1">Log in to AEM Assets as a <em>Workfront administrator</em>.</li> 
 <li value="2">Click <span class="bold">Tools</span> ><span class="bold"> Cloud Services&nbsp;</span>><span class="bold"> <em>Workfront</em> Integration Configuration</span> ><span class="bold"> Global-<em>Workfront</em>.</span><span class="bold"><br></span></li> 
 <li value="3">(Conditional) If you have not yet done so, create a <em>Workfront</em> cloud configuration file. 
  <ol> 
   <li value="1"><p>Click&nbsp;&nbsp;<span class="bold">Create</span> in the upper-right corner of the Global-<em>Workfront</em> page.</p><p><span class="bold"><img src="assets/wfintegrationconfig2-350x173.png" alt="WFintegrationConfig2.png" style="width: 350;height: 173;"></span></p></li> 
   <li value="2"><p>In the <span class="bold"><em>Workfront</em> URL</span> box, specify the URL for your <em>Workfront</em> instance. </p><p>For example, https://<em><account></em>.my.workfront.com,&nbsp;where <em><account></em> is the account you use for integrations with AEM.&nbsp;</p></li> 
   <li value="3">Click the<span class="bold">&nbsp;Base Folder</span> box, then in the drop-down menu select the path where documents that are linked to <em>Workfront</em> objects are stored.</li> 
   <li value="4"><p>Click <span class="bold">Select</span> in the upper-right corner.</p><p>You can link to any folder beneath the root /content/dam/.</p><note type="note">
      The /content/dam/ root folder is automatically created and configured when you install the 
     <em>Workfront</em> for AEM Assets connector.
    </note></li> 
   <li value="5"><p>In the <span class="bold"><em>Workfront</em> API Key</span> box, specify your <em>Workfront</em> API Key.</p><p>For information on API keys, see .</p><p>To retrieve your <em>Workfront</em> API key: </p> 
    <ol> 
     <li value="1">Open a browser tab, and log into your <em>Workfront</em> account as a <em>Workfront administrator</em>.</li> <draft-comment>
      <li value="2" data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click the <span class="bold">Main Menu</span> icon <img src="assets/main-menu-icon.png"> in the upper-right corner of <em>Adobe Workfront</em>, then click <span class="bold">Setup</span> <img src="assets/gear-icon-settings.png">.</li>
     </draft-comment>
     <li value="2" data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click the <span class="bold">Main Menu</span> icon <img src="assets/main-menu-icon.png"> in the upper-right corner of <em>Adobe Workfront</em>, then click <span class="bold">Setup</span> <img src="assets/gear-icon-settings.png">.</li> 
     <li value="3"><p>Click <span class="bold">System</span> ><span class="bold"> Customer Info</span>.</p><p>If you have already generated an API key, your <em>Workfront</em> API Key displays under the Your User's API Key label.</p></li> 
     <li value="4">(Conditional) If you have not yet generated an API key, you need to generate one: 
      <ol> 
       <li value="1"><p>In the <span class="bold">API Key Settings</span> section, ensure that the <span class="bold">After Creation, API keys expire in</span> option is set to None.</p><p>If you select an expiration period, the connector will stop working after the API Key expires. You will then to need to re-generate an API Key and update your <em>Workfront</em> configuration.</p></li> 
       <li value="2"><p>Under the <span class="bold">Your User's API Key</span> label, click <span class="bold">Generate API Key</span>.</p><p>An API Key for <em>Workfront</em> generates and displays.</p></li> 
      </ol></li> 
     <li value="5">Copy the API Key to your clipboard.</li> 
     <li value="6">Open the browser tab for AEM Connector and in the <span class="bold"><em>Workfront</em> API Key</span> box, paste the API Key you copied.</li> 
    </ol></li> 
   <li value="6"><p>(Conditional) Click the <span class="bold">Advanced</span> tab in the upper-left corner of the <em>Workfront</em> Integration Configuration page, and select the following options if applicable:</p><p><span class="bold">Allow Collection Browsing:&nbsp;</span>Select this option if your organization allows <em>Workfront</em> users to link AEM Assets collections to <em>Workfront</em> objects.</p><p><span class="bold">User Federated ID:</span> Select this option if your organization is using Federated IDs or Single Sign-On (SSO) when logging into <em>Workfront</em>.</p><p><span class="bold">Ignore Email Domain:</span> Select this option if your AEM users do not use the domain name in their user ID.&nbsp;</p><p><span class="bold">Restrict Access:</span> Select this option to specify the appropriate <em>Workfront</em> IP addresses that need to be added to the allowlist. For more information about the allowlist, see <a href="../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md" class="MCXref xref">Configure your firewall's allowlist</a>.</p></li> 
   <li value="7">Click the <span class="bold">Basic</span> tab in the upper-left corner of the <em>Workfront</em> Integration Configuration page, and then click <span class="bold">Connect</span>.</li> 
  </ol></li> 
 <li value="4"> (Conditional) If you already created a <em>Workfront</em> cloud configuration file, select&nbsp;<span class="bold">Global-<em>Workfront</em></span>, and then in the upper-left corner, click <span class="bold">Properties</span>.</li> 
 <li value="5"> <p>Generate the AEM API Key by clicking <span class="bold">Generate Key,</span> then copy the AEM API key to your clipboard.</p> <p>You will need the AEM API Key later when you configure <em>Workfront</em> to integrate with AEM Assets. For more information, see <a href="#configur2" class="MCXref xref">Configure Workfront to integrate with AEM assets</a>.</p> </li> 
 <li value="6"> <p>In the upper-right corner, click <span class="bold">Save</span>.</p> <p>The&nbsp;Global-<em>Workfront</em> window displays.</p> <p> <img src="assets/properties-350x117.png" alt="Properties.png" style="width: 350;height: 117;"> </p> </li> 
 <li value="7"> <p>(Optional) Synchronize&nbsp;bi-directional communication between AEM and <em>Workfront</em>. </p> 
  <ol> 
   <li value="1">Click <span class="bold">Global-<em>Workfront</em>.</span></li> 
   <li value="2"> <p>In the upper-left corner of the window, click <span class="bold">Properties</span>.</p> <p>The <em>Workfront</em> Integration Configuration page displays.</p> <p> <img src="assets/properties2-350x444.png" alt="Properties2.png" style="width: 350;height: 444;"> </p> </li> 
   <li value="3">(Optional) To enable the synchronization of comments between AEM Assets and <em>Workfront</em>, click <span class="bold">Enable Comment Sync</span>.</li> 
   <li value="4"> <p>(Optional) To turn off comment synchronization, click <span class="bold">Disable Comment Sync.</span></p> <p>Or</p> <p>Delete the&nbsp;NOTE CREATE event subscription registered to your AEM instance.</p> <p>For information on event subscriptions, see <a href="../../wf-api/general/event-subs-api.md" class="MCXref xref">Event Subscription API</a>.</p> </li> 
  </ol> </li> 
 <li value="8">Continue with <a href="#configur3" class="MCXref xref">Configure the AEM Externalizer</a>.<br></li> 
</ol>

### Install the connector package on AEM Assets versions 6.3 or older (classic UI)&nbsp;

<ol> 
 <li value="1">Log in to AEM Assets as a <em>Workfront administrator</em>.</li> 
 <li value="2">Click<span class="bold"> Tools</span> ><span class="bold"> Deployment</span> ><span class="bold">&nbsp;Cloud Services.</span></li> 
 <li value="3">Locate the <span class="bold"><em>Workfront</em> Document Sync</span> service, then click <span class="bold">Show Configurations</span>.</li> 
 <li value="4"> <p>In the<span class="bold"> Available Configurations</span> section, click <span class="bold">default (workfront-dam integration configuration)</span>.</p> <p> <img src="assets/wfconfig-350x150.png" alt="WFconfig.png" style="width: 350;height: 150;"> </p> <p>The AEM Default page displays. You need to first configure the <em>Workfront</em> Configuration settings.</p> </li> 
 <li value="5"> <p>Click <span class="bold">Edit</span>.</p> <p> <img src="assets/aemdetailspage-350x241.png" alt="AEMdetailsPage.png" style="width: 350;height: 241;"> </p> <p>The <em>Workfront</em> Configuration page displays.<br><img src="assets/wf-config-350x408.png" alt="WF_Config.png" style="width: 350;height: 408;"><br></p> </li> 
 <li value="6"> <p>In the <span class="bold"><em>Workfront</em> URL</span> box, specify the URL for your <em>Workfront</em> instance. </p> <p>For example, https://<em><account></em>.my.workfront.com,&nbsp;where <em><account></em> is the account you use for integrations with AEM Assets. This is a required field.</p> </li> 
 <li value="7"> <p>In the<span class="bold">&nbsp;Base Folder</span> box,&nbsp;specify the path where documents that are linked to <em>Workfront</em> objects are stored.&nbsp;You can link to any folder beneath the root /content/dam/.</p> <note type="note">
    The /content/dam/ root folder is automatically created and configured when you install the 
   <em>Workfront</em> for AEM Assets connector.
  </note> <p>This is a required field.</p> </li> 
 <li value="8"> <p>In the <span class="bold"><em>Workfront</em> API Key</span> box, specify your <em>Workfront</em> API Key.</p> <p>For information on API keys, see .</p> <p> To retrieve your <em>Workfront</em> API key: </p> 
  <ol> 
   <li value="1">Open a browser tab, and log into your <em>Workfront</em> account as a <em>Workfront administrator</em>.</li> <draft-comment>
    <li value="2" data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click the <span class="bold">Main Menu</span> icon <img src="assets/main-menu-icon.png"> in the upper-right corner of <em>Adobe Workfront</em>, then click <span class="bold">Setup</span> <img src="assets/gear-icon-settings.png">.</li>
   </draft-comment>
   <li value="2" data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click the <span class="bold">Main Menu</span> icon <img src="assets/main-menu-icon.png"> in the upper-right corner of <em>Adobe Workfront</em>, then click <span class="bold">Setup</span> <img src="assets/gear-icon-settings.png">.</li> 
   <li value="3">Click <span class="bold">System</span> ><span class="bold"> Customer Info</span>.<br>If you have already generated an API key, your <em>Workfront</em> API Key displays under the Your User's API Key label.</li> 
   <li value="4"> <p>(Conditional) If you have not yet generated an API key, you need to generate one: </p> 
    <ol> 
     <li value="1"> <p>In the <span class="bold">API Key Settings</span> section, ensure that the <span class="bold">After Creation, API keys expire in</span> option is set to None.</p> <p>If you select an expiration period, the connector will stop working after the API Key expires. You will then to need to re-generate an API Key and update your <em>Workfront</em> configuration.</p> </li> 
     <li value="2"> <p>Under the <span class="bold">Your User's API Key</span> label, click <span class="bold">Generate API Key</span>.</p> <p>An API Key for <em>Workfront</em> generates and displays.</p> </li> 
    </ol> </li> 
   <li value="5">Copy the API Key to your clipboard.</li> 
   <li value="6">Open the browser tab for AEM and in the <span class="bold"><em>Workfront</em> API Key</span> box, paste the API Key you copied.</li> 
  </ol> </li> 
 <li value="9"> <p>(Conditional) Select the following options, if applicable for your configuration:<br><span class="bold">User Federated ID:</span> Select this option if your organization is using Federated IDs or Single Sign-On (SSO) when logging into <em>Workfront</em>.</p> <p><span class="bold">Ignore Email Domain:</span> Select this option if your AEM users do not use the domain name in their user ID.&nbsp;</p> <p><span class="bold">Restrict Access:</span> Select this option to specify the appropriate <em>Workfront</em> IP addresses that need to be added to your allowlist. For more information about the allowlist, see the <a href="../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md" class="MCXref xref">Configure your firewall's allowlist</a> section in the article <a href="../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md" class="MCXref xref">Configure your firewall's allowlist</a>.</p> </li> 
 <li value="10"> <p>Click <span class="bold">OK</span>.</p> <p>The <em>Workfront</em> Configuration page closes.</p> </li> 
 <li value="11"> <p>(Conditional) If no AEM API Key displays, click <span class="bold">Generate Key</span> to generate an API Key.</p> <p> <img src="assets/aemapikey-350x176.png" alt="AEMapiKey.png" style="width: 350;height: 176;"> </p> </li> 
 <li value="12"> <p>Copy the AEM API key to your clipboard.</p> <p>You will need the AEM API Key later when you configure <em>Workfront</em> to integrate with AEM Assets. For more information, see <a href="#configur2" class="MCXref xref">Configure Workfront to integrate with AEM assets</a>.</p> </li> 
 <li value="13">(Optional) To enable the synchronization of comments between AEM Assets and <em>Workfront</em>, click <span class="bold">Enable Comment Sync</span>.</li> 
 <li value="14"> <p>(Optional) To turn off comment synchronization, click <span class="bold">Disable Comment Sync.</span></p> <p>Or</p> <p> Delete the&nbsp;NOTE CREATE event subscription registered to your AEM instance.<br>For information on event subscriptions, see the <a href="../../wf-api/general/event-subs-api.md" class="MCXref xref">Event Subscription API</a> section in the article <a href="../../wf-api/general/event-subs-api.md" class="MCXref xref">Event Subscription API</a>.</p> </li> 
 <li value="15">Continue with <a href="#configur3" class="MCXref xref">Configure the AEM Externalizer</a>.</li> 
</ol>

### Configure the AEM Externalizer

The AEM Externalizer allows AEM to pass URLs in a format that can be used in *Workfront*. If not properly configured, *Workfront* cannot make calls to the AEM API, and the URLs linking AEM documents in *Workfront* will not work.

<ol> 
 <li value="1"> In AEM, click <span class="bold">Tools</span> > <span class="bold">Operations</span> ><span class="bold"> Web Console</span>. </li> 
 <li value="2"> Click <span class="bold">OSGI</span>, then click <span class="bold">Configuration</span> in the drop-down menu. </li> 
 <li value="3"> <p>In the configuration list, select<span class="bold"> Day&nbsp;CQ Link Externalizer.</span></p> <p>The Externalizer page displays.</p> </li> 
 <li value="4"> <p> In the <span class="bold">Domains</span> section, ensure the domain listed in the Author field is the domain name externally accessible to AEM users.</p> <p> The domain name in the author field should match the domain listed in the URL line of your AEM instance. </p> <p> <img src="assets/extenalizer-350x128.png" alt="Extenalizer.png" style="width: 350;height: 128;"> </p> </li> 
 <li value="5"> (Conditional) If necessary, update the domain in the Author field. </li> 
 <li value="6"> <p> Click <span class="bold">Save</span>.</p> <p>AEM Assets is now configured to link documents with <em>Workfront</em></p> </li> 
 <li value="7">Continue with <a href="#configur2" class="MCXref xref">Configure Workfront to integrate with AEM assets</a>.</li> 
</ol>

## Configure *Workfront* to integrate with AEM assets

After you install the *Workfront* for AEM Assets Connector (as described in [Install the Workfront for AEM Assets connector package](#installi))&nbsp;and configure AEM Assets (as described in [Configure AEM Assets to integrate with Workfront](#configur)), you need to configure *Workfront* to link documents between&nbsp;*Workfront* and AEM Assets.

<ol> 
 <li value="1"> <p>Log in to <em>Workfront</em> as a <em>Workfront administrator</em>. </p> <note type="tip">
   <em>Workfront</em> recommends creating a 
   <em>Workfront administrator</em> dedicated solely to your AEM integration. For more information about assigning the 
   <em>Workfront administrator</em> access level to a user, see 
   <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Grant users administrative access to certain areas</a>.
  </note> </li> <draft-comment>
  <li value="2" data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click the <span class="bold">Main Menu</span> icon <img src="assets/main-menu-icon.png"> in the upper-right corner of <em>Adobe Workfront</em>, then click <span class="bold">Setup</span> <img src="assets/gear-icon-settings.png">.</li>
 </draft-comment>
 <li value="2" data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click the <span class="bold">Main Menu</span> icon <img src="assets/main-menu-icon.png"> in the upper-right corner of <em>Adobe Workfront</em>, then click <span class="bold">Setup</span> <img src="assets/gear-icon-settings.png">.</li> 
 <li value="3">Click&nbsp;<span class="bold">Documents&nbsp;</span>>&nbsp;<span class="bold">Custom Integration.</span></li> 
 <li value="4">Click <span class="bold">Add Custom Integration</span>.</li> 
 <li value="5"> <p>In the&nbsp;<span class="bold">Name</span> box, specify the name of the custom integration.</p> <p>This is the name users see when using the integration within <em>Workfront</em>; for example, you could enter <em>"AEM Assets"</em> for the name.&nbsp;</p> </li> 
 <li value="6"> <p>In the&nbsp;<span class="bold">Base API URL</span> box, specify the URL for your AEM instance.</p> <p>The base API URL consists of the URL for your AEM instance followed by the path: /bin/webhooks/api/</p> <p> <img src="assets/mceclip3-350x130.png" alt="mceclip3.png" style="width: 350;height: 130;"> </p> </li> 
 <li value="7">In the&nbsp;<span class="bold">Authentication Type</span> drop-down menu,&nbsp;select <span class="bold">ApiKey.</span></li> 
 <li value="8">In the<span class="bold"> API Key</span> box, paste the AEM API Key you copied when you configured AEM Assets.</li> 
 <li value="9">Click <span class="bold">Save</span>.</li> 
 <li value="10"> <p>(Optional) Ensure the integration is marked Active.<br><img src="assets/aem-custom-integration-active-350x81.png" alt="aem_custom_integration_active.png" style="width: 350;height: 81;"></p> <p><em>Workfront</em> is now configured to work with AEM Assets.</p> <p>In order to access assets in AEM, each <em>Workfront</em> user who needs to use the connector must be set up as a user in AEM. For information on creating users, see&nbsp;<a href="#setting" class="MCXref xref">Set up users to use the connector</a>.</p> </li> 
</ol>

## Set up users to use the connector

In order for users to access the connector, they must have a user profile in AEM and belong to a *Workfront* group that has Access levels that include the Create and Delete permissions.

For more information about *Workfront* permissions, see [Create or modify custom access levels](../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

* [Set up users in AEM assets version 6.4](#setting2) 
* [Set up users in AEM assets versions 6.3 or older](#setting3)

### Set up users in AEM assets version 6.4

<ol> 
 <li value="1">Log in to AEM Assets as a <em>Workfront administrator</em>.</li> 
 <li value="2"> Click&nbsp;<span class="bold">Tools</span> ><span class="bold">&nbsp;</span><span class="bold">Security</span> ><span class="bold"> Users</span>.</li> 
 <li value="3">(Conditional) If the user does not have a user profile in AEM, create an AEM user profile. 
  <ol> 
   <li value="1">Click <span class="bold">Create User.</span></li> 
   <li value="2"><p>Enter the user's personal information.</p><p><img src="assets/64newuser-350x524.png" alt="64NewUser.png" style="width: 350;height: 524;"></p><p>The only required field is the ID field.&nbsp;The user's AEM ID must match their <em>Workfront</em> ID, which is the user's <em>Workfront</em> email address. </p><p>If you selected the&nbsp;Ignore Email Domain option when you configured AEM to integrate with <em>Workfront</em>, then the AEM ID will not match the <em>Workfront</em> email address.&nbsp;</p></li> 
  </ol></li> 
 <li value="4"> (Conditional) If the user has an AEM profile, open the user's AEM profile. 
  <ol> 
   <li value="1"><p>Click<span class="bold">&nbsp;User.</span></p><p>The User Management page displays.</p></li> 
   <li value="2"><p>Click the user you want to add, then click <span class="bold">Properties</span>.</p><p>The user's settings page displays.</p></li> 
  </ol></li> 
 <li value="5"> <p> Click the <span class="bold">Groups</span> tab. </p> <p> <img src="assets/groupstab.png"><![CDATA[      ]]></p> </li> 
 <li value="6"> <p>Ensure the user belongs to at least one <em>Workfront</em> group that has Access levels that include the Create and Delete permissions.</p> 
  <ol> 
   <li value="1"> <p>To add the user to an existing group, begin typing the group name in the <span class="bold">Type Group Name</span> box, then select the group when it appears in the drop-down menu.</p> <p>Or</p> <p>To select a group to which the user is a member, select a group in the <span class="bold">Groups that this user is a member of</span> section. </p> </li> 
  </ol> </li> 
 <li value="7">Click <span class="bold">Save.</span></li> 
</ol>

### Set up users in AEM assets versions 6.3 or older&nbsp;

<ol> 
 <li value="1">Log in to AEM Assets as a <em>Workfront administrator</em>.</li> 
 <li value="2"> Click <span class="bold">Tools</span> > <span class="bold">Security</span> ><span class="bold"> Users</span>.</li> 
 <li value="3">(Conditional) If the user does not have a user profile in AEM, create an AEM user profile. 
  <ol> 
   <li value="1">Click <span class="bold">Create User</span> in the upper-right corner of the User Management page.</li> 
   <li value="2"><p>Enter the user's personal information, then continue with Step 5.</p><p><img src="assets/mceclip4-350x474.png" alt="mceclip4.png" style="width: 350;height: 474;"></p><p>The only required fields are the ID, Password, and Retype&nbsp;Password fields.&nbsp;The user's AEM ID must match their <em>Workfront</em> ID, which is the user's <em>Workfront</em> email address. </p><p>If you selected the&nbsp;Ignore Email Domain option when you configured AEM to integrate with <em>Workfront</em>, then the AEM ID will not match the <em>Workfront</em> email address.&nbsp;</p></li> 
  </ol></li> 
 <li value="4"> <p>(Conditional) If the user has an AEM profile, open the user's AEM profile.</p> <p>The Edit Users Settings page displays.</p> </li> 
 <li value="5"> <p> (Conditional) If the user is not a member of a <em>Workfront</em> group, in the <span class="bold">Add User to Groups</span> section, begin typing the name of a <em>Workfront</em> group to which the user belongs, then select the group when it displays in the drop-down menu.</p> <p>The user must belong to at least one <em>Workfront</em> group that has Access levels that include the Create and Delete permissions. For information about <em>Workfront</em> groups, see <a href="../../administration-and-setup/manage-groups/groups-overview/groups.md" class="MCXref xref">Groups overview</a>. </p> </li> 
 <li value="6"> Click <span class="bold">Save</span> in the upper-right corner. </li> 
</ol>

