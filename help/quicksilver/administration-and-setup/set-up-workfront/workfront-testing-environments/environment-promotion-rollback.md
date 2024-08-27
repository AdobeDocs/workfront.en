---
user-type: administrator
content-type: how-to-procedural
product-area: system-administration
navigation-topic: workfront-testing-environments
title: Roll back an environment promotion package
description: The environment promotion capability is intended to provide the ability to move configuration-related objects from one environment to another. Learn how to roll back an installed promotion package from a target environment.
author: Becky
feature: System Setup and Administration
role: Admin
recommendations: noDisplay, noCatalog
---
# Roll back an environment promotion package

<span class="preview">The information on this page refers to functionality not yet generally available. It is available only in the Preview Sandbox environment.</span>

After you have installed a package, you can roll it back. This removes the changes that the package made in the target environment, and restores the affected objects to their previous configurations.

You can roll back a promotion package within 25 hours after it is installed. After 25 hours, the rollback functionality is no longer available for that install.

## Access requirements

You must have the following:

<table>
  <tr>
   <td><strong>[!DNL Adobe Workfront] plan</strong>
   </td>
   <td> <p>New: Prime or Ultimate</p><p>Or</p><p>Current: Not available</p>
   </td>
  </tr>
  <tr>
   <td><strong>[!DNL Adobe Workfront] licenses</strong>
   </td>
   <td> <p>[!UICONTROL Standard]</p><p>Or</p><p>Current: Not available</p>
   </td>
  </tr>
   <tr>
   <td>Access level configurations
   </td>
   <td>You must be a [!DNL Workfront] administrator.
   </td>
  </tr>
</table>

For more detail about the information in this table, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md). 

## Prerequisites

* An environment promotion package must be installed before it can be rolled back. 

  For instructions, see [Install an environment promotion package](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion-install-package.md).

* Fewer than 25 hours must have passed since the package was installed.

## Roll back an installed environment promotion package

1. Go to the environment where the package was installed. 
1. Click the **[!UICONTROL Main Menu]** icon ![Main Menu](/help/_includes/assets/main-menu-icon.png) in the upper-right corner of Adobe Workfront, or (if available), click the **[!UICONTROL Main Menu]** icon ![Main Menu](/help/_includes/assets/main-menu-icon-left-nav.png) in the upper-left corner, then click **[!UICONTROL Setup]** ![Setup icon](/help/_includes/assets/gear-icon-setup.png).
1. Select **Environment Promotion** in the left navigation.
1. Select the package that you want to roll back, and click **Deployments**.
1. Hover over the deployment (installation) that you want to roll back, then click Roll Back when it appears on the right of that deployment's line.

   Or

   Click on the deployment that you want to roll back, then click **Roll back package** in the upper-right corner of the screen.
   
   >[!IMPORTANT]
   >
   >The deployment must have occurred fewer than 25 hours before you roll it back. Installations more than 25 hours old cannot be rolled back.

1. (Optional) In the Rollback Preview area, view the changes that will occur when the deployment is rolled back. 
1. Click **Roll Back** in the upper-right corner of the screen.







