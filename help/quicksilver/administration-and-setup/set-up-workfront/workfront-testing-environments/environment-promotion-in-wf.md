---
user-type: administrator
content-type: overview;how-to-procedural
product-area: system-administration
navigation-topic: workfront-testing-environments
title: Move objects from one environment to another within Workfront
description: The Environment Promotion capability is intended to provide the ability to move configuration-related objects from one environment to another. It does not support the ability to move transactional objects (with limited exceptions).
author: Becky
feature: System Setup and Administration
role: Admin
hide: yes
hidefromtoc: yes
recommendations: noDisplay, noCatalog
---
# Move objects from one [!DNL Workfront] environment to another within Workfront

This article will be instructions on how to do this in the UI.

Maybe split into overview and instructions depending on how complicated instructions are. 

Maybe more (conflicts, installation separate from creation, etc.)

Copy included objects from API article

Add a list of possible statuses: build etc. Table in other article under [Update specific properties of a package](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion.md#update-specific-properties-of-a-package)

Sections or possibly articles: 

## Create a package

1. Go to the environment that you want to create the package in. This is the environment that you are copying objects **from**.
1. Click the **[!UICONTROL Main Menu]** icon ![Main Menu](/help/_includes/assets/main-menu-icon.png) in the upper-right corner of Adobe Workfront, or (if available), click the **[!UICONTROL Main Menu]** icon ![Main Menu](/help/_includes/assets/main-menu-icon-left-nav.png) in the upper-left corner, then click **[!UICONTROL Setup]** ![Setup icon](/help/_includes/assets/gear-icon-setup.png).
1. Select **System** in the left navigation, then select **Environment Promotion**.
1. Click **Create Package**.

   The New Promotion Package page opens.

1. in the **Package name** field, enter a name for the package.
1. In the **Description** field, enter a description for this package. 
1. To add an object to the package, click **Add Objects** in the left navigation and select the type of object you want to add.
1. Select one or more objects from the list, or type the name in the search bar and select the object when it appears in the list. 
1. Click **Add to package**.

   The object that you have added appears in the Package Contents area on the right of the page.

1. To add another object, repeat steps 7-9.
1. (Optional) To remove an object from the package, hover over the object in the Package Contents area, then click the X next to the object.
1. After you have added all of the desired objects to the package, click **Save and Close** to save the package without assembling it.

   Or

   Click **Save and Extract** to save and assemble the package.

## Edit or assemble an existing package

1. Go to the environment that you want to create the package in. This is the environment that you are copying objects **from**.
1. Click the **[!UICONTROL Main Menu]** icon ![Main Menu](/help/_includes/assets/main-menu-icon.png) in the upper-right corner of Adobe Workfront, or (if available), click the **[!UICONTROL Main Menu]** icon ![Main Menu](/help/_includes/assets/main-menu-icon-left-nav.png) in the upper-left corner, then click **[!UICONTROL Setup]** ![Setup icon](/help/_includes/assets/gear-icon-setup.png).
1. Select **System** in the left navigation, then select **Environment Promotion**.
1. Select the package from the displayed list.
1. (Conditional) To see archived (disabled) packages, enable the **Show retired packages** option.
1. To view the contents, including all objects and their sub-objects, click **Contents**.
1. To view previous installations and installation attempts of this package, click **Deployments**.
1. To edit the package, click **Edit Package** at the upper-right of the screen.
1. To extract the package, click **Deploy Package** at the upper-right of the screen.




## Install a package

