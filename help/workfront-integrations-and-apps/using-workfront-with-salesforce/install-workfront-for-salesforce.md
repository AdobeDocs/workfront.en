---
filename: install-workfront-for-salesforce
product-area: workfront-integrations
navigation-topic: workfront-for-salesforce
title: Install Adobe Workfront for Salesforce
description: To install the app before it becomes available in the Salesforce AppExchange, see Installing Workfront for Salesforce before It Becomes Available in the AppExchange Marketplace.
---

# Install *Adobe Workfront* for Salesforce

To install the app before it becomes available in the Salesforce AppExchange, see [Installing Workfront for Salesforce before It Becomes Available in the AppExchange Marketplace](#install-before-available-in-appexchange).

As a Salesforce and *Adobe Workfront administrator*, you can install *Workfront* for Salesforce to allow your Salesforce users to submit *Workfront* requests and automatically create projects without ever leaving Salesforce.

For a general understanding about what you can expect by installing *Workfront* for Salesforce, see [Adobe Workfront for Salesforce overview](../../workfront-integrations-and-apps/using-workfront-with-salesforce/workfront-for-salesforce-overview.md).

* [Prerequisites for Installing and Using Workfront for Salesforce](#prerequisites) 
* [Installing Workfront for Salesforce](#installing-the-app)

## Access requirements

You must have the following access to use the functionality described in this article:

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><em>Adobe Workfront</em> plan*</td> 
   <td> <p>Pro or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><em>Adobe Workfront</em> license*</td> 
   <td> <p>Plan</p> </td> 
  </tr> <draft-comment>
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td role="rowheader">Access level configurations*</td> 
    <td> <p>[Insert any access level configurations needed] <draft-comment>
       <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
        Example: Edit access to Documents
       </MadCap:conditionalText>
      </draft-comment><MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
       Example: Edit access to Documents
      </MadCap:conditionalText></p> <p>Note: If you still don't have access, ask your <em>Workfront administrator</em> if they set additional restrictions in your access level. For information on how a <em>Workfront administrator</em> can modify your access level, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> <draft-comment>
      <p data-mc-conditions="QuicksilverOrClassic.Draft mode">You must be a <em>Workfront administrator</em>. For information on <em>Workfront administrators</em>, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Grant a user full administrative access</a>.</p>
     </draft-comment><p data-mc-conditions="QuicksilverOrClassic.Draft mode">You must be a <em>Workfront administrator</em>. For information on <em>Workfront administrators</em>, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Grant a user full administrative access</a>.</p> <draft-comment>
      <p data-mc-conditions="QuicksilverOrClassic.Draft mode">You must be a <em>group administrator</em>. For more information on <em>group administrators</em>, see <a href="../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">Group administrators</a>.</p>
     </draft-comment><p data-mc-conditions="QuicksilverOrClassic.Draft mode">You must be a <em>group administrator</em>. For more information on <em>group administrators</em>, see <a href="../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">Group administrators</a>.</p> </td> 
   </tr>
  </draft-comment>
  <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>[Insert any access level configurations needed] <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
      Example: Edit access to Documents
     </MadCap:conditionalText></p> <p>Note: If you still don't have access, ask your <em>Workfront administrator</em> if they set additional restrictions in your access level. For information on how a <em>Workfront administrator</em> can modify your access level, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> <p data-mc-conditions="QuicksilverOrClassic.Draft mode">You must be a <em>Workfront administrator</em>. For information on <em>Workfront administrators</em>, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Grant a user full administrative access</a>.</p> <p data-mc-conditions="QuicksilverOrClassic.Draft mode">You must be a <em>group administrator</em>. For more information on <em>group administrators</em>, see <a href="../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">Group administrators</a>.</p> </td> 
  </tr> <draft-comment>
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td role="rowheader">Object permissions</td> 
    <td> <p>[Insert permissions needed and specify the object] <draft-comment>
       <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
        Example: View access or higher on Documents
       </MadCap:conditionalText>
      </draft-comment><MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
       Example: View access or higher on Documents
      </MadCap:conditionalText></p> <p>For information on requesting additional access, see <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects in Adobe Workfront</a>.</p> </td> 
   </tr>
  </draft-comment>
  <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>[Insert permissions needed and specify the object] <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
      Example: View access or higher on Documents
     </MadCap:conditionalText></p> <p>For information on requesting additional access, see <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects in Adobe Workfront</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your *Workfront administrator*.

## Prerequisites for Installing and Using *Workfront* for Salesforce

* You must have a Salesforce instance with access to a system administrator account in order to install the app.
* You must have a *Workfront* instance with access to a system administrator account in order to configure the integration.
* Salesforce users must have a *Workfront* account in order to be able to

  * Create *Workfront* requests from Salesforce or
  * View *Workfront* requests or projects in Salesforce.

## Installing *Workfront* for Salesforce

You must be a Salesforce and a *Workfront* system administrator to install and configure *Workfront* for Salesforce.&nbsp;

The following subsections describe how to install *Workfront* for your Salesforce Production environment. You can follow the same steps to install *Workfront* for your Salesforce Sandbox environment.

* [Installing Workfront for Salesforce before It Becomes Available in the AppExchange Marketplace](#install-before-available-in-appexchange) 
* [Installing Workfront for Salesforce in the Salesforce Classic Framework](#installing-the-app-classic) 
* [Installing Workfront for Salesforce in the Salesforce Lightning Experience Framework](#installing-the-app-lightning-experience)

### Installing *Workfront* for Salesforce before It Becomes Available in the AppExchange Marketplace

<!--
<p style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">This section needs to be removed when our app is accepted by Salesforce and added to their store.</p>
-->

This section needs to be removed when our app is accepted by Salesforce and added to their store.

*Workfront* for Salesforce will be available in the Salesforce AppExchange soon.

To install the app before it's available:

1. In your Production environment, go to

   https://login.salesforce.com/packaging/installPackage.apexp?p0=04t4K000002aUZY

   In your Sandbox environment, go to

   https://test.salesforce.com/packaging/installPackage.apexp?p0=04t4K000002aUZY

<ol data-mc-continue="true"> 
 <li value="2"> <p>Check the <span class="bold">Yes, grant access to these third-party web sites</span> box.<br></p> <p> <img src="assets/salesforce-grant-access-350x249.png" alt="salesforce_grant_access.png" style="width: 350;height: 249;"> <br> </p> <p> A loading screen displays and the installation might take a while.</p> </li> 
 <li value="3">Click <span class="bold">Done</span> when the installation completes.<br></li> 
 <li value="4">Navigate to <span class="bold">Setup>Security Controls>Remote Site Settings</span>.</li> 
 <li value="5">(Conditional) If you do not see your <em>Workfront</em> URL listed in the <span class="bold">All Remote Sites</span> list, click <span class="bold">New Remote Site</span>.</li> 
 <li value="6"> <p>Specify the <span class="bold">Remote Site Name</span>. <br></p> <p>For example, <i><em>Workfront</em></i>.</p> </li> 
 <li value="7"> <p>Specify the <span class="bold">Remote Site URL</span>.<br></p> <p>For example, <i>yourDomain.my.workfront.com</i>.</p> </li> 
 <li value="8"> <p>Click <span class="bold">Save</span>.<br></p> <p>The <em>Workfront</em> app is now installed on your Salesforce instance and the <span class="bold">WorkfrontOpportunities</span> and <span class="bold">WorkfrontAccounts</span> Visualforce Pages have been created in your environment.<br></p> <p>Salesforce users can use the app once you add the <em>Workfront</em> section to their Opportunity or Account page layouts.<br>For information about configuring the <em>Workfront</em> section for users, see <a href="../../workfront-integrations-and-apps/using-workfront-with-salesforce/configure-wf-section-for-salesforce-users.md" class="MCXref xref">Configure the Adobe Workfront section for Salesforce users</a>.</p> </li> 
</ol>

### Installing *Workfront* for Salesforce in the Salesforce Classic Framework

<ol> 
 <li value="1">Log in to Salesforce as a system administrator.</li> 
 <li value="2">Go to <span class="bold">Setup. </span></li> 
 <li value="3">In the<span class="bold"> Build </span>section, click <span class="bold">AppExchange Marketplace</span>.</li> 
 <li value="4"> In the <span class="bold">Search AppExchange Apps</span> box, type <span class="bold"><em>Workfront</em></span>. </li> 
 <li value="5"> Click the app when you find it, then click <span class="bold">Get It Now</span>. </li> 
 <li value="6"> Click <span class="bold">Install in Production </span>to install the <em>Workfront</em> app in your Salesforce Production environment.&nbsp;(recommended) </li> 
 <li value="7"> Select the <span class="bold">I have read and agree to the terms and conditions</span> field after you have read and agreed with the terms and conditions. </li> 
 <li value="8"> Click <span class="bold">Confirm and Install</span>. </li> 
 <li value="9">Select <span class="bold">Install for All Users</span> (recommended), then click <span class="bold">Install</span>.&nbsp;</li> 
 <li value="10"> (Conditional) If asked if you want to approve a third party access, you must select&nbsp;<span class="bold">Yes, grant access to these third-party web sites</span>, then click <span class="bold">Continue</span>.&nbsp; </li> 
 <li value="11"> <p> Click <span class="bold">Done</span> when the installation completes.&nbsp; </p> <p>The <em>Workfront</em> app is listed under <span class="bold">Installed Packages</span>.</p> <p> <img src="assets/salesforce-classic-installed-packages-350x129.png" alt="salesforce_classic_Installed_Packages.png" style="width: 350;height: 129;"> </p> </li> 
 <li value="12">Navigate to <span class="bold">Setup>Security Controls>Remote Site Settings</span>.</li> 
 <li value="13">(Conditional) If you do not see your <em>Workfront</em> URL listed in the <span class="bold">All Remote Sites</span> list, click <span class="bold">New Remote Site</span>.<br><img style="font-size: small;width: 350;height: 176;" src="assets/salesforce-remote-site-edit-350x176.png" alt="salesforce_remote_site_edit.png"></li> 
 <li value="14">Specify the <span class="bold">Remote Site Name</span>. <br>For example,&nbsp;<i><em>Workfront</em></i>.</li> 
 <li value="15">Specify the <span class="bold">Remote Site URL</span>.<br>For example, <i>yourDomain.my.workfront.com</i>.</li> 
 <li value="16">Click <span class="bold">Save</span>.<br>The <em>Workfront</em> app is now installed on your Salesforce instance and the <span class="bold">WorkfrontOpportunities</span> and <span class="bold">WorkfrontAccounts</span> Visualforce Pages have been created in your environment.<br>Salesforce users cannot yet use the app until you add the <em>Workfront</em> section to their Opportunity or Account page layouts.<br>For information about configuring the <em>Workfront</em> section for users, see <a href="../../workfront-integrations-and-apps/using-workfront-with-salesforce/configure-wf-section-for-salesforce-users.md" class="MCXref xref">Configure the Adobe Workfront section for Salesforce users</a>.</li> 
</ol>

### Installing *Workfront* for Salesforce in the Salesforce Lightning Experience Framework

<ol> 
 <li value="1">Log in to Salesforce as a system administrator.</li> 
 <li value="2">Click the&nbsp;<span class="bold">Setup icon</span>, then click <span class="bold">Setup</span>.</li> 
 <li value="3">In the<span class="bold"> PLATFORM TOOLS </span>section, expand <span class="bold">Apps.</span></li> 
 <li value="4">Click <span class="bold">AppExchange Marketplace</span>.</li> 
 <li value="5"> In the <span class="bold">Search AppExchange Apps</span> box, type <span class="bold"><em>Workfront</em></span>. </li> 
 <li value="6"> Click the app when you find it, then click <span class="bold">Get It Now</span>. </li> 
 <li value="7"> Click <span class="bold">Open Login Screen</span>.<br>You must sign in with your <em>Workfront administrator</em> account for Salesforce. </li> 
 <li value="8"> Click <span class="bold">Allow</span>. </li> 
 <li value="9"> In the <span class="bold">Install in This Org</span> box, click <span class="bold">Install Here&nbsp;</span>to install <em>Workfront</em> in your Salesforce Production environment.&nbsp;(recommended) </li> 
 <li value="10"> Select the <span class="bold">I have read and agree to the terms and conditions</span> field after you have read and agreed with the terms and conditions. </li> 
 <li value="11"> Click <span class="bold">Confirm and Install</span>. </li> 
 <li value="12">Select <span class="bold">Install for All Users</span> (recommended), then click <span class="bold">Install</span>.&nbsp;</li> 
 <li value="13"> (Conditional) If asked if you want to approve a third party access, you must select <span class="bold">Yes, grant access to these third-party web sites</span>, then click <span class="bold">Continue</span>. </li> 
 <li value="14"> <p> Click <span class="bold">Done</span> when the installation completes.&nbsp; </p> <p>The <em>Workfront</em> app is listed under <span class="bold">Installed Packages</span>.</p> <p>&nbsp; <img src="assets/salesforce-lightning-installed-packages-350x171.png" alt="salesforce_lightning_Installed_packages.png" style="width: 350;height: 171;"></p> </li> 
 <li value="15">Navigate to <span class="bold">Setup. </span></li> 
 <li value="16">In the <span class="bold">SETTINGS </span>section, expand<span class="bold"> Security.&nbsp;</span></li> 
 <li value="17">Click <span class="bold">Remote Site Settings</span>.</li> 
 <li value="18"> <p>(Conditional) If you do not see your <em>Workfront</em> URL listed in the <span class="bold">All Remote Sites</span> list, click <span class="bold">New Remote Site</span>.</p> <p> <img src="assets/salesforce-remote-site-settings-lightning-350x136.png" alt="Salesforce_remote_site_settings_lightning.png" style="width: 350;height: 136;"> </p> </li> 
 <li value="19"> <p>Specify the <span class="bold">Remote Site Name</span>. <br></p> <p>For example,&nbsp;<em><em>Workfront</em></em>.</p> </li> 
 <li value="20"> <p>Specify the <span class="bold">Remote Site URL</span>.<br></p> <p>For example, <em>yourDomain.my.workfront.com</em>.</p> </li> 
 <li value="21"> <p>Click <span class="bold">Save</span>.<br></p> <p>The <em>Workfront</em> app is now installed on your Salesforce instance, and the <span class="bold"><em>Workfront</em></span> component is now added to your environment.<br></p> <p>Salesforce users can use the <em>Workfront</em> app once you add the <em>Workfront</em> section to their Opportunity or Account page layouts.<br>For information about configuring the <em>Workfront</em> section for users, see <a href="../../workfront-integrations-and-apps/using-workfront-with-salesforce/configure-wf-section-for-salesforce-users.md" class="MCXref xref">Configure the Adobe Workfront section for Salesforce users</a>.&nbsp;</p> </li> 
</ol>

