---
title: Access Needed for Adobe Workfront Planning as a Standalone Product
description: This article describes licenses, access levels and user capabilities for the Adobe Workfront Planning as a standalone product. 
last-update: 2026-04-01T14:02:40-04:00
git-commit-file: 8cc175490a6aa1db68b238edbdf9da9da7fbb258
---
<!--

Update metadata with this at release:
---
title: Access Required for Planning Standalone
description: This article describes how you can benefit from using the standalone version of Adobe Workfront Planning.
feature: Workfront Planning (******************ask Bob for a new feature???***********)
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
---
-->

# Access needed for Adobe Workfront Planning as a standalone product

>[!IMPORTANT]
>
>The information in this article refers to Adobe Workfront Planning, when purchased as a standalone product. Refer to this article when your company purchased an Adobe Workfront Planning only package, and they did not purchase a Workfront Workflow package. 
>
>For information about Adobe Workfront Planning when purchased together with a Workfront Workflow package, see [Get started with Adobe Workfront Planning](/help/quicksilver/planning/general/planning-overview.md). 

This article describes licenses, access levels and user capabilities for the Adobe Workfront Planning as a standalone product. 

## Workfront Planning packages

Your organization can purchase one of the following standalone Workfront Planning packages:

* Prime
* Select
* Ultimate

The following table describes what is included in each package:  

| Planning Capability | Select | Prime | Ultimate |
|---|---|---|---|
| Planning, orchestration, campaign management | ✓ | ✓ | ✓ |
| Unlimited workspaces | ✓ | ✓ | ✓ |
| Records per workspace | 25,000 | 500,000 | 1,000,000 |
| Total records (all workspaces) | 500,000 | 2,000,000 | Unlimited |
| Global Record Types and cross-workspace connections | — | ✓ | ✓ |
| Access to future features at release | Some | Some | Most |

## Workfront Planning package availability

<!--
the bullets repeat in the "Planning overview" article
-->

Workfront Planning is accessible when your organization purchases one of the following Workfront packages: 

* Workfront Workflow and Workfront Planning purchased together. Every user in the organization has a Workflow and a Planning license. This gives all users full access to all Workfront's features for both modules. 

* Workfront Workflow for everyone in your organization and Workfront Planning only for some users in your organization. This gives users full access to all Workflow's features and a more limited access to Planning features for the users who are assigned a Planning license.   

* Workfront Planning as a standalone product for users in your organization. This gives users no access to any Workfront Workflow features and access to Planning features.

For information about capabilities included in Planning as a standalone product, see the section "Functionality included in Workfront Planning as a standalone product" in the article [Get started with Adobe Workfront Planning as a standalone product](/help/quicksilver/planning/planning-sta/planning-sta-overview.md). 

## User license and access levels

<!-- should this be moved to the Manage users in Planning article??-->

Planning licenses are part of the access level assigned to users. 

For Planning as a standalone product, you cannot assign licenses to the access levels - they are already hard coded to be included in the access levels assigned to users. 

Depending on which Workfront Planning package combination your organization purchases, you might have one of the following access levels for your users: 

* **Planning Administrator**: Available for Workfront Planning packages. Planning Administrators are automatically assigned when users are added to the Admin Console. 
* **Planning Standard**: Available for all Workfront Planning packages. You can assign this access levels to users when you create them.

<!--
this is not available for Planning STA: 
* **Planning Contributor**: Available for the following customers: 

    * Customers that purchase equal amounts of Workflow and Planning packages together. In this case, Planning Contributors have limited access to Planning objects.
    * Customer that purchase unequal amounts of Workflow and Planning packages. In this case, Planning Contributors have read-only access to Planning objects.

--> 

Each standalone Planning license maps to a role in the system and controls what areas of the product are accessible.

The following table illustrates each Planning license type and its capabilities in Workfront Planning, when purchased as a standalone product: 

| Feature / License type | Planning Administrator | Planning Standard |
|---|---|---|
| Access level description | Full system access | Can manage workspaces and content |
| Planning area in the Main Menu | ✔ | ✔ |
| Users area in the Main Menu | ✔ | View only |
| Requests area in the Main Menu | ✔ | ✔ |
| Setup area in the Main Menu | ✔ |   |
| Manage Workspaces and their content | ✔ | ✔ |
| Share Planning data with teams | ✔ | ✔ |
| Submit requests | ✔ | ✔ |
| Create or edit users | ✔ |   |
| View users list | ✔ | View only |
| Setup > Teams | ✔ |   |
| Setup > Log In As | ✔ |   |
| Setup > Custom Quarters | ✔ |   |
| Setup > System > Customer info | ✔ |   |
| Setup > System > Preferences | ✔ |   |

For information about assigning users access levels, see [Manage Users in Adobe Workfront Planning as a standalone product](/help/quicksilver/planning/planning-sta/manage-users-in-planning-sta.md).

## Navigation areas and access level dependencies

Depending on the Planning license, users might have different areas available in their global navigation. 

<!--
>[!NOTE]
>
>Workfront-specific toolbar actions (Search, Recents, Favorites, Notifications) are not available in the Workfront header for any Standalone user.
-->

### Planning Administrator navigation overview

<!--
Managing your Adobe Workfront Planning instance is similar to managing an Adobe Workfront with Planning instance, but there are some differences.
-->

A user with a Planning Administrator access level  has the following capabilities: 

* Has full manage access to the system.
* Can create and edit users, manage teams, configure custom quarters, and access all Setup sub-pages.

    For information, see:

    * [Manage users in Adobe Workfront Planning as a standalone product](/help/quicksilver/planning/planning-sta/manage-users-in-planning-sta.md)
    * [Manage teams in Adobe Workfront Planning as a standalone product](/help/quicksilver/planning/planning-sta/manage-teams-in-planning-sta.md)
* Can submit and manage requests. 

    For information, see [Adobe Workfront Planning requests: article index](/help/quicksilver/planning/requests/requests-article-index.md). 
* Has the following areas in the Main menu: 

    * **Planning**: Has full capabilities for Planning objects, to create, delete, share, and connect them. 
    * **Users**: You can add users and edit their profiles.
    * **Requests**
    * **Setup**
* Has the following sections in the Setup area: 

    * **Teams**: You can add, remove, or edit teams. Editing is limited to team name, description, and members; no filter, view, grouping, or export controls are available.
    * **Log In As**: Impersonate another user for troubleshooting purposes.
    * **Custom Quarters**: Configure custom fiscal quarters that appear in Planning timeline views.
    * System

* Has the following sections in the System area:

    * **Customer Info**: View customer and organization details.
    * **Preferences**: Review and configure system-level preferences.

### Planning Standard navigation overview

A user with a Planning Standard access level  has the following capabilities: 

* Can manage workspaces and their content.
* Can submit and manage requests. 

    For information, see [Adobe Workfront Planning requests: article index](/help/quicksilver/planning/requests/requests-article-index.md). 
* Planning Standard users can access the following areas in the Main menu:

    * **Planning**
    * **Users**: They have view-only access to users. They cannot create or edit users. <!--not sure if this is still true-->
    * **Requests**

* Have no access to Setup or any of its sections.

## Configure Access Levels for Planning as a standalone product

Access levels are built-in when you purchase Planning as a standalone product and you cannot configure them for Planning users.

To assign access levels to users, as a Planning Administrator: 

* Create users in the Adobe Console. 

    The following scenarios exist:

    * Users added to the Adobe Console as Administrators receive a Planning Administrator access level in Workfront Planning. 
    * Users added to the Adobe Console as users can be assigned a Planning Standard access level in Workfront Planning. This is the only access available to assign to new users in Workfront Planning as a standalone product. 

For more information, see [Manage users](/help/quicksilver/planning/planning-sta/manage-users-in-planning-sta.md). 

## Grant permissions in Workfront Planning as a standalone product

You can share the following objects in Workfront Planning as a standalone product:

* Workspaces
* Record types
* Records
* Views

Sharing objects in Planning as a standalone product is identical to sharing them in Planning when purchased together with a Workflow package. 

For more information, see [Adobe Workfront Planning access information: article index](/help/quicksilver/planning/access/access-information.md). 

<!--

I took this out because there is NO Contributor for true STA: 

### Planning Contributor user experience

>[!IMPORTANT]
>
>Planning Contributor access level is only available for customers that purchase both Workfront Planning and a Workfront Workflow package together. 
>
>If they purchase unequal numbers of packages for the two modules, the Planning Contributor license is read-only. 

When standalone Workfront Planning users purchase a Workflow package, they receive a read-only Planning Contributor license by default. 

For more information, see [Get started with Adobe Workfront Planning as a standalone product](/help/quicksilver/planning/planning-sta/planning-sta-overview.md).

A user with a Planning Standard access level has the following capabilities: 

* View-only access to Planning data, equivalent to the Contributor license in Workfront.
* Can access the following areas in the Main menu:
    * **Planning**
    * **Requests**
* Can submit requests.
* No access to the Users list.
* No access to Setup or any of its sub-pages.

-->

<!-- 
this was moved from the STA general article - some information is already above - take out here what is not needed or add above: 

## Package overview

The following packages are available for Workfront Planning as a standalone product:

* Select
* Prime
* Ultimate

The following table describes what is included in each package:  

| Capability | Select | Prime | Ultimate |
|---|---|---|---|
| Planning, orchestration, campaign management | ✓ | ✓ | ✓ |
| Unlimited workspaces | ✓ | ✓ | ✓ |
| Records per workspace | 25,000 | 500,000 | 1,000,000 |
| Total records (all workspaces) | 500,000 | 2,000,000 | Unlimited |
| Global Record Types and cross-workspace connections | — | ✓ | ✓ |
| Access to future features at release | Some | Some | Most |

## Licensing overview

Consider the following about Workfront Planning licenses:

* Your organization can purchase Workfront Planning licenses without requiring Workfront or Workflow licenses.
* You can add users to Workfront Planning using the Adobe Experience Platform.

    For more information, see [Manage users](/help/quicksilver/planning/planning-sta/manage-users-in-planning-sta.md). 
* Workfront Planning users are limited to Planning-only capabilities and do not receive access to any Workfront areas or capabilities.

The following access levels are hard-coded in Workfront Planning and cannot be modified: 

* Planning Administrator
* Planning Standard 

>[!IMPORTANT]
>
>In a Workfront Planning context, a user must hold a **Planning Standard** license to access the product. 

For more information, see [Access needed for Adobe Workfront Planning as a standalone product](/help/quicksilver/planning/planning-sta/access-needed-for-planning-sta.md). 

## How licensing works for customers with a Planning and Workfront combined package

Consider the following if you have both the Workfront Workflow and Planning packages:

* A Planning Contributor read-only license is available for users in Planning. 
* Any Workfront access level (including Light or Contributor) can be paired with either a Planning Standard or Planning Contributor access level, regardless of the Workfront Workflow license type.

    For example, a user with a Workfront Contributor license can still hold a Planning Standard license and have full Planning management capabilities.

### Mixed License access matrix

When a customer has both Planning and Workfront packages, access levels are determined by the combination below:

| Access Type | Planning License | Workflow License | License Origin |
|---|---|---|---|
| Default | Read Only | Workfront Light | Workfront |
| Default | Read Only | Workfront Standard | Workfront |
| Default | Read Only | Workfront Contributor | Workfront |
| Default | Read Only | Workfront External | Workfront |
| Default | Planning Standard | Workfront Contributor | Planning |
| — | Planning Standard | Workfront Light | Either Planning or Workfront |
| — | Planning Standard | Workfront Standard | Either Planning or Workfront |

Consider the following if your organization has purchased Workfront with Planning:

* Adding a new user to Planning or Workfront automatically creates default (read-only) access in the other product.
* You can upgrade the access in the opposite product. For more information, contact your account representative.

### Upgrading from standalone Planning to a Planning with a Workflow package

#### Workfront Planning with a Workfront Workflow package

When you add a Workfront Planning Standalone package to an existing Workflow license, the following changes take effect automatically:

* Planning Administrators are promoted to System Administrators.
* Non-admin Planning users (Standard and Contributor) receive Workflow Contributor licenses.
* All existing Planning data is preserved.
* All newly provisioned Workfront users are auto-assigned Planning Contributor (read-only) licenses.

#### License mapping when you upgrade to a Planning with Workflow package

| Before (Planning Standalone) | After (Workfront + Planning) |
|---|---|
| Planning Administrator | System Administrator |
| Planning Standard | Workflow Contributor |
| Planning Contributor | Workflow Contributor |

Planning and Workflow licenses remain separate after the upgrade. A Planning Standard user can hold a Workflow Contributor license, and a Planning Contributor user can hold a Workflow Standard license — these are assigned independently based on need.

All users receive an email notification when they gain access to the additional Workflow capabilities in Workfront.

-->

<!--
I took out the last column on this table and added above:

| Feature / Access | Planning Administrator | Planning Standard | Planning Contributor |
|---|---|---|---|
| Access level description | Full system access | Can manage workspaces and content | View-only access to Planning data when Planning packages are in unequal numbers to Workflow licenses. This license is not available for Planning as a standalone product.|
| Planning area in the Main Menu | ✔ | ✔ | ✔ |
| Users area in the Main Menu | ✔ | View only |   |
| Requests area in the Main Menu | ✔ | ✔ | ✔ |
| Setup area in the Main Menu | ✔ |   |   |
| Manage Workspaces and their content | ✔ | ✔ |   |
| Submit requests | ✔ | ✔ | ✔ |
| Create or edit users | ✔ |   |   |
| View users list | ✔ | View only |   |
| Setup > Teams | ✔ |   |   |
| Setup > Log In As | ✔ |   |   |
| Setup > Custom Quarters | ✔ |   |   |
| Setup > System > Customer info | ✔ |   |   |
| Setup > System > Preferences | ✔ |   |   |

-->
