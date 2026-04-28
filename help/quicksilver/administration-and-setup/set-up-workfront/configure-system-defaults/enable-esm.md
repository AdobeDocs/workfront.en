---
user-type: administrator
product-area: system-administration;projects
navigation-topic: configure-system-defaults
title: Enable Adobe enterprise storage for Your Organization
description: You can enable Adobe enterprise storage for your organization to use a unified storage solution for all Adobe products.
author: Courtney
feature: System Setup and Administration
role: Admin
exl-id: 48b581c7-a21a-45de-95c5-eafb0713b42e
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
---
# Enable Adobe enterprise storage for your organization

Adobe enterprise storage is a unified storage solution for all Adobe products. It is a cloud-based storage solution that serves as the central repository for assets across Adobe enterprise products.

Adobe enterprise storage is enabled by default for new customers and can be enabled for existing customers upon contract renewal.

For more information about Adobe enterprise storage, see [Adobe enterprise storage overview](/help/quicksilver/review-and-approve-work/esm-overview.md).

## Access requirements

+++ Expand to view access requirements for the functionality in this article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront package</td> 
   <td><p>Any Workflow package</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license</td> 
   <td><p>Standard</p> <p>Plan</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td>You must be a Workfront administrator. </td> 
  </tr> 
 </tbody> 
</table>

For information, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md). 

+++

## Enable Adobe enterprise storage for your organization

To enable Adobe enterprise storage for your organization:

{{step-1-to-setup}}

1. Select **System** in the left navigation, then select **Preferences**.
1. Scroll down to the **Storage preferences** section.
1. In the Default drop-down menu, select **Adobe enterprise storage**.
1. (Optional) If you want to use a combination of Adobe enterprise storage and Legacy Workfront Storage, select the **Allow user to select storage provider** checkbox.

    >[!NOTE]
    >
    >Enabling this option allows users to select the storage provider when they create a new project. enterprise storage is labeled as "New project" since it is the default storage provider. Legacy Workfront Storage is labeled as "Legacy project".
    >
    >![new project and legacy project options](assets/new-esm-project.png)

1. In the Applies to drop-down menu, choose one of the following options:

    - **Entire organization**: This option applies the default storage provider to your entire Workfront environment. Any time a user creates a new project, the default storage provider will be used.
    - **Specific groups**: This option applies the default storage provider only to specific groups within your organization. Any time a user in the specified groups creates a new project, the default storage provider will be used

1. Click **Save**.

    >[!NOTE]
    >
    >Existing projects keep the storage model they were created with. For example, projects that use Adobe enterprise storage continue to use Adobe enterprise storage after you change the default storage preference.
