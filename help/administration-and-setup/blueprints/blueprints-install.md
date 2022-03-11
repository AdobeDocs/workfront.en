---
filename: blueprints-install
user-type: administrator
content-type: reference
product-area: system-administration;workfront-integrations
navigation-topic: best-practices-catalog
title: Install a blueprint
description: The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview Sandbox environment.
---

# Install a blueprint

The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview Sandbox environment.

You can install a blueprint in your Production environment or a Sandbox environment.

## Access requirements

You must have the following access to perform the steps in this article:

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan</td> 
   <td> <p> Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>System administrator </p> </td> 
  </tr> 
 </tbody> 
</table>

## Where should I install a blueprint?

You can install your package in any of the following environments:

| Production |Production is your live environment.  |
|---|---|
| Sandbox Preview |The Sandbox Preview is a testing environment that serves as a replica of your live environment and is refreshed each weekend by Workfront. All support packages have access to the Sandbox Preview. For more information, see [The Adobe Workfront Preview Sandbox Environment](../../administration-and-setup/set-up-workfront/workfront-testing-environments/wf-preview-sandbox-environment.md) |
| Sandbox 1 & 2 |The Custom Refresh Sandbox is a separate testing environment which is refreshed manually by you. There is an additional cost to obtain the Custom Refresh Sandbox. For more information, see [The Adobe Workfront Custom Refresh Sandbox environment](../../administration-and-setup/set-up-workfront/workfront-testing-environments/wf-custom-refresh-sandbox-environment.md). |

>[!TIP]
>
>We recommend first installing the blueprint in a sandbox environment. That way, you can test the blueprint's content and make sure it’s a good fit for your organization without making changes to live data.

>[!NOTE]
>
>Certain blueprints are only available to install in the Preview environment for testing purposes. If you access Preview-only content in your Production environment, Sandbox 1, or Sandbox 2, the install button is not active, and you might see a warning message.  
>Also, the environment switching capability is limited when accessing Preview-only content, even when you are in the Preview environment.

## Install the blueprint

<ol> 
 <li value="1"> <p>Click the <span class="bold">Main Menu</span> icon <img src="assets/main-menu-icon.png"> in the upper-right corner of Adobe Workfront, then click <span class="uitext">Blueprints</span>.</p> </li> 
 <li value="2"> <p>Find the blueprint you want to install. You can filter by use case, maturity level, installation status, and type on the right-hand side.</p> </li> 
 <li value="3"> <p>(Optional) Click <span class="bold">Details</span> to learn how the blueprint works.</p> </li> 
 <li value="4"> <p>Click <span class="bold">Install</span>.</p> </li> 
 <li value="5"> <p>Choose to install on your production environment or a sandbox environment.<br>For more information, see the <a href="#where" class="MCXref xref">Where should I install a blueprint?</a> section in this article.</p> </li> 
 <li value="6"> <p>On the Configure page, you can choose to do one of the following: 
   <ul>
    <li>Install the blueprint as is and configure later. Click <span class="bold">Install as is</span>.</li>
    <li>Configure the blueprint before installation. Make your configuration selections, and click <span class="bold">Install blueprint</span>.<br>For more information, see <a href="../../administration-and-setup/blueprints/configure-template-package.md" class="MCXref xref">Configure a blueprint</a>.</li>
   </ul></p> <p><span class="preview">When the installation is complete, a message displays a list of the specific objects (such as roles, teams, or groups) that were successfully installed with the blueprint and any objects that failed to install.</span> </p> </li> 
</ol>

After installing the blueprint, some additional actions are needed to fully deploy it. For information, see [Actions to take after installing a blueprint](../../administration-and-setup/blueprints/best-next-actions-after-install.md).
