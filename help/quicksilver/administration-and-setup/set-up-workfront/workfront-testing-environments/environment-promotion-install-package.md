---
user-type: administrator
content-type: how-to-procedural
product-area: system-administration
navigation-topic: workfront-testing-environments
title: Install an environment promotion package
description: The environment promotion capability is intended to provide the ability to move configuration-related objects from one environment to another. Learn how to install an environment promotion package into a target environment.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: fe213fe7-5bb8-479c-926b-761cbdd7ba4e
---
# Install an environment promotion package

After you have created a package, you can install it in a different environment.

You must install a package in the environment that you want to copy objects **to**. For example, if you are configuring a project in your Custom Refresh Sandbox environment and promoting it to your Production environment, you must install the package in your Production environment.

>[!IMPORTANT]
>
>* If your Custom Refresh Sandbox is refreshed while you are configuring object for environment promotion, that configuration will be lost in the refresh. We recommend that you do not refresh your Custom Refresh Sandbox unless all outstanding environment promotion objects and packages have been successfully promoted.
>* Objects created in the target environment as part of package installation do **not** have the same ID as the object in the original environment. This is due to the fact that IDs are assigned by the system when objects are created.

## Access requirements

You must have the following:

<table>
  <tr>
   <td><strong>[!DNL Adobe Workfront] plan</strong>
   </td>
   <td> Prime or Ultimate (New plans only)
   </td>
  </tr>
  <tr>
   <td><strong>[!DNL Adobe Workfront] licenses</strong>
   </td>
   <td> [!UICONTROL Standard]
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

An environment promotion package must be created before it can be installed. 

For instructions, see [Create or edit an environment promotion package](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion-create-package.md).

## Package status for installation

A package must be in ACTIVE status to be installed in your production environment.

We recommend moving the package to TESTING status and installing in another sandbox to test the package.  If this test is successful, with no errors, move the package to ACTIVE to install it in your production environment.  

To edit a package's status: 

1. Select the package as described in  [Edit or assemble an existing package](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion-create-package.md#create-or-edit-an-environment-promotion-package) in the article Create and edit environment promotion packages.
1. Click **Edit Package**.
1. Click **Status**.
1. Select the desired status from the drop-down menu.

For more information on statuses, see [Environment Promotion Statuses](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion-in-wf.md#environment-promotion-statuses) in the article Overview of moving objects between Workfront environments.

## Install a package

>[!NOTE]
>
>* To install a package, you must be logged in to the environment where you want to install the package. This is the environment that you are copying objects **to**.

1. Go to the environment where you want to install the package. 
1. Click the **[!UICONTROL Main Menu]** icon ![Main Menu](/help/_includes/assets/main-menu-icon.png) in the upper-right corner of Adobe Workfront, or (if available), click the **[!UICONTROL Main Menu]** icon ![Main Menu](/help/_includes/assets/main-menu-icon-left-nav.png) in the upper-left corner, then click **[!UICONTROL Setup]** ![Setup icon](/help/_includes/assets/gear-icon-setup.png).
1. Select **System** in the left navigation, then select **Environment Promotion**.
1. Select the package from the displayed list.
1. For each object that has a collision, select how to resolve the collision.

   To resolve a collision, click the drop-down arrow next to the object type, and select the action that you want to take.

   For more information, see [Collisions](#collisions) in this article
1. To deploy the package into the new environment, click **Deploy** at the upper-right of the screen. 

## Collisions

A collision is an object found in the target environment of an installation that matches one of the objects being installed from the source environment. Collisions are detected by comparing the names and IDs of the source objects against objects in the target environment. Collisions are also detected by comparing source objects against records of previously installed objects.

When a collision occurs, you can select how to resolve the collision. Collisions are resolved on the object level.

You can view collisions by clicking on the drop-down next to each object type. Collisions are displayed in the Collision column. 

>[!NOTE]
>
>Detected collisions may not be the objects that you want to override or use in your installation. We reccomend validating detected collisions to ensure that the installation targets are correct.

To resolve a collision, select an action in the Deployment Action column, or use the default action that is already displayed.

* **Create with new name**: Create a new object in the target environment. If the object exists in the target environment, you can create a new object with a new name. If it does not exist in the target environment, you can create the object with a new name or with the name that the object has in the package. 
* **Use existing**: The object in the package is not installed, and the object that already existed in the target environment is unchanged.
* **Overwrite**: The object in the package replaces the existing object in the target environment.

   You can also choose objects to overwrite even if a collision is not detected.

   For details on how overwriting affects parent and child objects, see [Overwriting parent and child objects](#overwriting-parent-and-child-objects) in this article.
<!--
* Do not use: The object in the package is not installed in the target environment. If you select Do not use, an error message will appear detailing how this choice will affect other objects or fields.
-->

Default values are `Create new` if the object does not exist in the target environment, and `Use existing` if the object does exist in the target environment. You can revert to the default mapping by clicking **Reset to default mapping**.

## Overwriting parent and child objects

Some objects in your promotion package may have child objects. For example, a project (parent) has tasks (children). When overwriting a parent object, child objects are handled as follows:

* Child objects that exist in both the package and the target will be updated in the target to match the package.
* Child objects that exist in the package but not the target will be created.
* Child objects that exist in the target but not the package will remain unchanged.

This functionality affects the following parent and child objects:

|Parent object|Child objects|
|---|---|
|Project|Task<br>QueueDef (Queue Definition)<br>RoutingRule |
|Template|TemplateTask<br>QueueDef (Queue Definition)<br>RoutingRule |
|Parameter (Custom form field)|ParameterOption (Custom form field option)|
|CalendarInfo|CalendarSection|
|QueueDef (Queue Definition)|QueueTopicGroup<br>QueueTopic|

