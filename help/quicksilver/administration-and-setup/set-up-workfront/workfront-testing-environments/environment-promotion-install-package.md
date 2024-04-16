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
>To install a package, you must be logged in to the environment where you want to install the package. This This is the environment that you are copying objects **to**.

1. Go to the environment where you want to install the package. 
1. Click the **[!UICONTROL Main Menu]** icon ![Main Menu](/help/_includes/assets/main-menu-icon.png) in the upper-right corner of Adobe Workfront, or (if available), click the **[!UICONTROL Main Menu]** icon ![Main Menu](/help/_includes/assets/main-menu-icon-left-nav.png) in the upper-left corner, then click **[!UICONTROL Setup]** ![Setup icon](/help/_includes/assets/gear-icon-setup.png).
1. Select **System** in the left navigation, then select **Environment Promotion**.
1. Select the package from the displayed list.
1. To install the package, click **Install** at the upper-right of the screen. 
1. Map each object in the package to the corresponding object in the target environment.

   For more information, see [Mapping](#mapping) in this article


## Mapping

Each object type is listed in the left navigation and on a card. The card displays objects of that type and whether those objects exist in the target environment. You can determine how these objects will move to the target environment. 

* Create new: Create a new object in the target environment. If the object exists in the target environment, you can create a new object with a new name. If it does not exist in the target environment, you can create the object with a new name or with the name that the object has in the package. 
* Use existing: The object in the package is not installed, and the object that already existed in the target environment is unchanged.
* Overwrite existing: (Not currently available) The object in the package replaces the existing object in the target environment.
* Do not use: The object in the package is not installed in the target environment. If you select Do not use, an error message will appear detailing how this choice will affect other objects or fields.

Default values are `Create new` if the object does not exist in the target environment, and `Use existing` if the object does exist in the target environment. You can revert to the default mapping by clicking **Reset to default mapping**.



<!--
## Collisions

A collision occurs when <!--???--.

In Workfront, a potential collision is marked with a blue dot. You can select 

You can select whether to show all package contents, or collisions only.

## Comparison tool

-->
