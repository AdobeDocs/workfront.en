---
title: Enable a Workfront Planning Workspace to GenStudio for Performance Marketing
description: If you already have a workspace in Adobe Workfront Planning, you can enable it for GenStudio for Performance Marketing instead of recreating your data. 
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 0747fb80-496f-41c0-b469-1203e1605f05
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/wHSc0Neshdl-Owh1siw72wdO-H1hnEPy-dAk91tDOrI
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
---
# Enable a Workfront Planning workspace to GenStudio for Performance Marketing

{{planning-important-intro}}

<!-- add to TOC and mini TOC-->

<!--
Better metadata, at publishing:
---
title: Promote a Workfront Planning workspace to GenStudio
description: The GenStudio for Performance Marketing workspace is available in Adobe Workfront Planning when your company has purchased both products and your instance of Workfront is integrated with your company's instance of GenStudio. You can promote a Workfront Planning workspace to GenStudio and have its information visible and updated from both systems.
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
---
-->
In addition to Workfront Planning, if your company also purchased Adobe GenStudio for Performance Marketing, the GenStudio workspace is available in Adobe Workfront Planning when your instance of Workfront is integrated with your company's instance of GenStudio. 

If you already have a workspace in Workfront Planning, you can enable it for GenStudio instead of recreating your data. 

Enabling a workspace links it to an Adobe storage project and maps its record types and fields to the GenStudio workspace schema. After you complete the configuration, you can open the workspace's records in GenStudio.

Consider the following: 

* You must have access to both Workfront Planning and GenStudio for Performance Marketing. 
* You must have an Adobe cloud storage project to link to the workspace. An organization administrator can create one in the Adobe Admin Console. 
  
    For information, see [Manage Adobe storage](https://helpx.adobe.com/business/enterprise/manage-storage-assets/manage-storage/manage-adobe-storage.html). <!--ensure this site still works-->


## Enable a Workfront Planning workspace to GenStudio 

1. In Workfront Planning, open the workspace you want to enable.
1. Click the **More** menu ![More menu](assets/more-menu.png) to the right of the workspace name, then click **Enable GenStudio**.

    The **Make workspace GenStudio** enabled box opens with the following steps:
    
    1. **ACPC Project**:  Select the **ACPC Project** (Adobe cloud storage project) you want to sync with this workspace, then click **Next**. Users access the workspace in GenStudio through this project.

        ![Make workspace GenStudio enabled - ACPC project step](assets/make-workspace-genstudio-enabled-box-acpc-step.png)

    1. **Record Types**: Map the workspace's record types to the six record types that GenStudio requires: 
    
        * Campaigns
        * Products
        * Personas
        * Channels
        * Regions
        * Activations
      
        For each one, open the list and select the matching Planning record type, or select **Add new** to create it, then click **Next**.

        ![Make workspace GenStudio enabled - Record types step](assets/make-workspace-genstudio-enabled-box-record-types-step.png)
    
    1. **Fields**: Map the fields for each record type. Use the tabs at the top of the dialog to move between record types. For each field, select the matching Planning field, or select **Add new** to create it.

        Repeat the field setup for all record types. 

        ![Make workspace GenStudio enabled - Fields step](assets/make-workspace-genstudio-enabled-box-fields-step.png)

    1. Review and address any warnings. 
    
        For example, a new field can become the primary field for the record type or a field alias that's already in use is renamed (if you already have a field named "Regions", the imported one might become "Regions 2"). 
      
        Mapping a **Status** field adds the required options.
 
    1. Click **Publish**. 
    
        A confirmation message appears when the workspace is enabled. Mapped record types are marked in the workspace. 

        The record types mapped to be accessible from GenStudio have a new **Adobe** icon on their cards. 

        ![Campaigns record type with Adobe icon](assets/campaigns-record-type-card-with-adobe-icon.png)
      
1. Open GenStudio, and select **Campaigns**, then click the **ACPC project** you originally configured for this setup in the lower-left corner of the screen. Review the imported record types and fields. 

    >[!TIP]
    >
    >You see only the records that your ACPC project membership allows.
