---
title: Use Environment Promotion for Adobe Workfront Planning
description: You can copy Workfront Planning workspaces, record types, fields, and views from one Workfront environment to another using Environment Promotion capabilities. Instead of rebuilding everything by hand, you assemble the configuration into a package in the source environment and install it in the target environment.
author: Alina, Becky
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
---

# Use Environment Promotion for Adobe Workfront Planning 

<!--add to TOC-->
<!--add to miniTOC-->

<!--
Not sure if this bit will ever be needed because this only exists when both Preview and Prod have the features in parity. Features released here always come to both environments at the same time: 

<span class="preview">The information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the release to Preview, the same features are also available monthly in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>
-->

{{planning-important-intro}}

<!--if Lilit says this is not for STA, break the intro and specify that; she is checking on this-->

You can copy Workfront Planning workspaces, record types, fields, and views from one Workfront environment to another using Environment Promotion capabilities. 

Instead of rebuilding everything by hand, you assemble the configuration into a package in the source environment and install it in the target environment.

Using Environment Promotion with Planning is similar to using it for Workfront. For more information, see the "Environment Promotion" section in the article [Adobe Workfront testing environments](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/wf-testing-environments.md). 

## Considerations about using Environment Promotion with Planning 

* You must be a Workfront administrator to use Environment Promotion. 
* The following are imported through environment promotion:

    * Workspaces
    * Workspace sections
    * Record types
    * Fields
    * Views
    * Hierarchies
    * Sharing settings for all objects
    * Automations <!--this might not be part of it; Lilit is checking-->
    * Request forms
    * Business rules
    * Connected objects
    * Objects that the workspace depends on or that other objects are shared with, such as group, teams, job roles. The following scenarios exist: 
    
        * If an object with the same name already exists in the target environment, Workfront flags a conflict and you decide how to handle it.
        * If a team or a group that an object is shared with does not exist in the target environment, the promotion creates it.
* For each object, you can do the following:

    * Create it as a new object
    * Use the existing object but create it with a new name
    * Overwrite an existing object. Overwriting replaces the configuration in the target.

* Installation can take a few minutes. You can roll back an installation from the results page if needed.
* We recommend to test the process before proceeding, when possible. You can install to a sandbox or Preview environment before promoting it to Production.

## Access requirements 

+++ Expand to view access requirements for the functionality in this article. 

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront packages</p></td> 
   <td> 
<p>Prime or Ultimate Workflow package with a Prime or Ultimate Planning package</p>
<p>Prime or Ultimate Planning package when purchased as a standalone product</p>
   </td> 
   </tr>
  <tr> 
   <td role="rowheader"><p>Adobe Workfront license</p></td> 
   <td><p>Workflow Standard</p>    
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Planning license</p></td> 
   <td><p>Planning Standard</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Access level configuration</p></td> 
   <td> <p>You must add both a Workflow and a Planning license type to the access level when you have both a Workflow and a Planning package</p>  
   <p>You must be a System Administrator</p> 
</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Object permissions</p></td> 
   <td>   <p>Manage permissions to workspaces</p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p>  
   </td> 
  </tr>  
</tbody> 
</table> 

 For more information about Workfront access requirements, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Import Planning configuration using Environment Promotion

The following are the main steps to promote Planning configuration to another environment: 

* [Create a package in the source environment](#create-a-package-in-the-source-environment) 
* [Make the package ready to install](#make-the-package-ready-to-install)
* [Install the package in the target environment](#install-the-package-in-the-target-environment)
* [Verify the results](#verify-the-results)

Follow the instructions in the following sections to copy a Planning configuration between two Workfront environments. 

### Create a package in the source environment 

1. Have a source environment where your desired configuration is in place. 
1. In the source environment, click the **Main Menu** ![Main Menu](assets/main-menu-shell.png), then go to **Setup** > **System** > **Environment Promotion**. 
    The **Configuration Packages** list shows existing packages with their status, source environment, and where they were deployed.
1. Click **Create package**.

    >[!TIP]
    >
    >A package needs at least one object before it can be assembled and installed.
1. On the **Package Details** tab, enter a **Name** and a **Description** for the package. The source environment is already filled in with the current (source) environment. 
1. In the list of object types on the left, select **Planning workspace**.
1. Search for the workspace you want to promote, select its checkbox, and click **Add Planning workspace**. The workspace appears under **Package Contents**.

    ![Workspace selected for Environment Promotion](assets/workspace-selected-for-environment-promotion.png)
1. Click **Save and assemble**. 

    Workfront assembles the package and adds an entry on the package's **Updates** tab. You can review what the package includes on the Contents tab.
1. (Conditional and optional) Click **Save and close** instead if you want to finish later.
1. (Optional) Click **Contents** to review the contents of the package or click **Deployments** to see if this package has been deployed multiple times.

    Continue to make the package ready to install. 

### Make the package ready to install

Before installing the package in the target environment, we recommend you test it in a testing environment. 

1. After the package has finished building as described in the previous section, click **Package Details**, and click **Edit**, set the **Status** to **Testing**, then click **Save and close**. 

    >[!TIP]
    >
    >After building the package its status is set to **Draft**. The **Active** status is not available until you have tested the package first. 
1. (Recommended) Click **Install** and choose one of the testing environments available to deploy it there and test the configuration.

    >[!TIP]
    >
    >The Production environment is not available as one of the options when the status is set to **Testing**.

1. After you install it in a testing environment, click **Edit** again, and set the **Status** to  **Active**, then click **Save and close**.

    >[!TIP]
    >
    >Installing the package in a testing environment is similar to installing it in Production, as described in the following section. 

    Continue with the following section to install the package in your target environment. 


### Install the package in the target environment

1. On the package page, after you have verified it, click **Install**.
1. In the **Target environment** list, select the environment to deploy to (for example, your Production environment), and click **Continue**. The default target is the current environment.
1. On the **Package info** page, confirm the source environment and the environment you are deploying to.
1. In the **Object mapping** section, expand each object grouping, such as **Group** and **Planning workspace**, to review the objects.
1. For each object, review the **Collision** and **Status** columns, then choose a **Deployment action** from the list. Choose from the following options: 

    * **Create new**: Adds the object to the target. Use this when no collision is detected.
    * **Use existing**: Maps the object to one that already exists in the target, such as a group with the same name.
    * **Create with new name**: Adds the object under a name you specify.
    * **Overwrite**: Replaces the existing object in the target with the one from the package.
1. (Optional) To change several objects at once, select their checkboxes, choose an action in the Deployment action list at the top of the group, and click Apply to selected. Use the filters above the list, such as Show only errors, to focus on specific objects.
1. Resolve any error indicators. If you select **Use existing** for an object, you must also select the object it maps to.  Otherwise, the status shows an error and **Deploy** stays unavailable.
1. Click **Deploy**, then **Deploy** to confirm.

    Workfront shows an installation page with the message **This package is being installed**. This may take a few minutes.

    When the installation finishes, the page shows a success message, the environment where the package was installed, and a list of the installed objects, with a status for each, such as **Used existing** or **Installed (Create new)**.
1. (Optional) Click **Roll back installation**, if needed to revert the installation and remove the configuration from the target environment. 

    Continue to verify the results of the installation. 

### Verify the results

1. Go to the target environment > **Main Menu** > **Planning** and find the imported workspace.
1. Open the record types and views to confirm the fields and layout match the source. Records are not included, so tables are empty.


