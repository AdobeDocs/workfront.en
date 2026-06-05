---
title: Workspaces Overview
description: A workspace is a collection of record types used by a team and represents the team's work lifecycle. You can fully customize workspaces in Adobe Workfront Planning to match your organizational units' workflows.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: b80d5ccf-4d22-49f2-89b6-bb9678a353c2
TQID: https://experienceleague.adobe.com/Hh1Gh4ex1dLrPhsmqiLv3x5NAU0yKzIwcsV4hEogXTo
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
    internal-label: Admin
---
# Workspaces overview

<span class="preview">The information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

{{planning-important-intro}}

A workspace is a collection of record types used by an organizational unit and it represents the unit's work lifecycle and processes. You can fully customize workspaces in Adobe Workfront Planning. 

<!--update screenshot with production, it was broken at Preview-->

![Workspaces landing page admin account](assets/workspaces-landing-page-admin-account.png)

## Considerations about workspaces

* You can create workspaces for specific organizational units within your organization, to match the unique way each unit works. 
* Workfront Planning does not come with any preconfigured workspaces. You must create them according to the needs of your organization. 
* You can create workspaces in the following ways: 

    * From scratch
    * Using a template. Templates contain a preconfigured number of record types and their fields. 
    * Using the AI-powered Planning Designer. This feature is currently in Beta.
    * Using a multi-workspace template bundle.

    For information, see [Create workspaces](/help/quicksilver/planning/architecture/create-workspaces.md). 
    
* Workspaces are frameworks within which your organizational units (a team, group, department, or division) work. They cannot be associated with fields. Only the record types within  a workspaces can be associated with fields. 

    For information, see [Record types overview](/help/quicksilver/planning/architecture/overview-of-record-types.md). 
* Workspaces display in the following tabs in the Planning area:  

    * **Workspaces I'm on**: Displays workspaces you created or workspaces that are shared with you.
    * **Other workspaces**: Displays all other workspaces in the system. This is only available for System Administrators.
    * <span class="preview">**Sample workspaces**: Displays built-in examples of best-practice workspaces. You cannot edit the workspaces, record types, or add records or fields, but you can add, edit, and share views with others.</span>

    >[!NOTE]
    >
    ><span class="preview">We recommend to not edit the sample workspaces, but instead to use them as a reference to create your own. Use the multi-workspace template bundle to create workspaces identical to the ones listed in the Sample workspaces tab. For information, see the section "Create multiple workspaces using a best-practice multi-workspace template bundle" in the article [Create workspaces](/help/quicksilver/planning/architecture/create-workspaces.md). </span>  
    
<!--
No longer the case - they match now: 

* For all other users:

* **Workspaces I'm on**: Workspaces they created (for Standard-license users) and workspaces others shared with them display in the Workspaces area.

<div class="preview"> 

* **Sample workspaces**: Displays built-in examples of best-practice workspaces. You cannot edit the workspaces, record types, or add records, but you can add, edit, and share views with others.

</div>
-->
    
    

* The record types that a workspace contains should reflect the work lifecycle and concepts of an organizational unit. 

    For example, if a unit's work objects are campaigns, products, and regions, that unit's workspace should contain the record types of Campaign, Product, and Region. 
* When you create a workspace, only you have the permission to access and manage your workspace. You must share it with other users in order for them to collaborate with you in the same space. 

    For information, see [Share a workspace](/help/quicksilver/planning/access/share-workspaces.md). 
    
    System administrators can manage all workspaces, even the ones that they did not create. 

<!--make this live with the GA: * There is no limit for how many workspaces you can create in your environment. However, we recommend not to have too many workspaces, as they could become hard to manage and your workflows might be too fragmented.-->

* There are limits on how many workspace objects you can create in your instance of Workfront Planning. For information, see [Adobe Workfront Planning object limitations overview](/help/quicksilver/planning/general/limitations-overview.md).
