---
filename: blueprints-install
user-type: administrator
content-type: reference
product-area: system-administration;workfront-integrations
navigation-topic: best-practices-catalog
title: Install a blueprint
description: You can install a blueprint in your Production environment or a Sandbox environment.
---

# Install a blueprint

You can install a blueprint in your Production environment or a Sandbox environment.

## Access requirements

You must have the following access to perform the steps in this article:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront plan</strong></td> 
   <td> <p> Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront license</strong></td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Access level configurations</strong></td> 
   <td> <p>System administrator</p> </td> 
  </tr> 
 </tbody> 
</table>

## Where should I install a blueprint? {#where-should-i-install-a-blueprint}

You can install your package in any of the following environments:

<table style="table-layout:auto">
        <tr>
        <td><strong>Production</strong></td>
        <td>Production is your live environment.</td>
    </tr>
    <tr>
        <td><strong>Sandbox Preview</strong></td>
        <td>The Sandbox Preview is a testing environment that serves as a replica of your live environment and is refreshed each weekend by Workfront. All support packages have access to the Sandbox Preview. For more information, see <a href="help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/wf-preview-sandbox-environment.md">The Adobe Workfront Preview Sandbox Environment</a>.</td>
    </tr>
    <tr>
        <td><strong>Sandbox 1 &amp; 2</strong></td>
        <td>The Custom Refresh Sandbox is a separate testing environment which is refreshed manually by you. There is an additional cost to obtain the Custom Refresh Sandbox. For more information, see <a href="help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/wf-custom-refresh-sandbox-environment.md">The Adobe Workfront Custom Refresh Sandbox environment</a>.</td>
    </tr>
</table>

>[!TIP]
>
>We recommend first installing the blueprint in a sandbox environment. That way, you can test the blueprint's content and make sure it's a good fit for your organization without making changes to live data.

>[!NOTE]
>
>Certain blueprints are only available to install in the Preview environment for testing purposes. If you access Preview-only content in your Production environment, Sandbox 1, or Sandbox 2, the install button is not active, and you might see a warning message.  
>Also, the environment switching capability is limited when accessing Preview-only content, even when you are in the Preview environment.

## Install the blueprint

1. Click the **Main Menu** icon ![](assets/main-menu-icon.png) in the upper-right corner of Adobe Workfront, then click **Blueprints**.
1. Find the blueprint you want to install. You can filter by use case, maturity level, installation status, and type on the right-hand side.
1. (Optional) Click **Details** to learn how the blueprint works.
1. Click **Install**.
1. Choose to install on your production environment or a sandbox environment.  
   For more information, see the [Where should I install a blueprint?](#where-should-i-install-a-blueprint) section in this article.
1. On the Configure page, you can choose to do one of the following:

   * Install the blueprint as is and configure later. Click **Install as is**.
   * Configure the blueprint before installation. Make your configuration selections, and click **Install blueprint**.  
     For more information, see [Configure a blueprint](../../administration-and-setup/blueprints/configure-template-package.md).

   When the installation is complete, a message displays a list of the specific objects (such as roles, teams, or groups) that were successfully installed with the blueprint and any objects that failed to install.

After installing the blueprint, some additional actions are needed to fully deploy it. For information, see [Actions to take after installing a blueprint](../../administration-and-setup/blueprints/best-next-actions-after-install.md).
