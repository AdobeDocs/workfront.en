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
hide: yes
hidefromtoc: yes
recommendations: noDisplay, noCatalog
exl-id: fe213fe7-5bb8-479c-926b-761cbdd7ba4e
---
# Install an environment promotion package

>[!NOTE]
>
>To install a package, you must be logged in to the environment where you want to install the package. This is the environment that you are copying objects **to**.

1. Go to the environment where you want to install the package. 
1. Click the **[!UICONTROL Main Menu]** icon ![Main Menu](/help/_includes/assets/main-menu-icon.png) in the upper-right corner of Adobe Workfront, or (if available), click the **[!UICONTROL Main Menu]** icon ![Main Menu](/help/_includes/assets/main-menu-icon-left-nav.png) in the upper-left corner, then click **[!UICONTROL Setup]** ![Setup icon](/help/_includes/assets/gear-icon-setup.png).
1. Select **System** in the left navigation, then select **Environment Promotion**.
1. Select the package from the displayed list.
1. For each object that has a collision, select how to resolve the collision.

   To resolve a collision, click the dropdown arrow next to the object type, and select the action that you want to take.

   For more information, see [Collisions](#collisions) in this article
1. To deploy the package into the new environment, click **Deploy** at the upper-right of the screen. 

## Collisions

Collisions occur when an object that is part of the installation package has the same name as an object that already exists in the target environment. When this occurs, you can select how to resolve the collision. Collisions are resolved on the object level.

You can view collisions by clicking on the dropdown next to each object type. Collisions are displayed in the Collision column. 

To resolve a collision, select an action in the Deployment Action column, or use the default action that is already displayed.

* **Create with new name**: Create a new object in the target environment. If the object exists in the target environment, you can create a new object with a new name. If it does not exist in the target environment, you can create the object with a new name or with the name that the object has in the package. 
* **Use existing**: The object in the package is not installed, and the object that already existed in the target environment is unchanged.
* **Overwrite**: The object in the package replaces the existing object in the target environment.

   You can also choose objects to overwrite even if a collision is not detected.

   FOr details on how overwriting affects parent and child objects, see 
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

