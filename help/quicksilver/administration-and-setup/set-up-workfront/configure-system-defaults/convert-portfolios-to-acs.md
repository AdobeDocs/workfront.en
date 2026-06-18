---
user-type: administrator
product-area: system-administration;projects
navigation-topic: configure-system-defaults
title: Convert legacy portfolios to Adobe cloud storage
description: Convert existing legacy Workfront storage portfolios to Adobe cloud storage from the Storage Preferences area in System Preferences.
author: Courtney
feature: System Setup and Administration
role: Admin
---
# Convert legacy portfolios to Adobe cloud storage

As a Workfront administrator, you can convert existing legacy Workfront storage portfolios to Adobe cloud storage from the Storage Preferences area in System Preferences. After a portfolio is converted, it behaves like any other Adobe cloud storage portfolio.

For more information about how converted portfolios behave and how their child objects are affected, see [Object portability](/help/quicksilver/review-and-approve-work/workfront-storage.md#object-portability) in [Move to Workfront on Adobe cloud storage](/help/quicksilver/review-and-approve-work/workfront-storage.md).

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

## Before you convert a portfolio

Before you convert a legacy Workfront storage portfolio, consider the following:

* The conversion affects only the portfolio itself. Child projects and programs that use legacy Workfront storage stay on legacy storage. 
    >[!NOTE]
    >
    >A child legacy program converts to Adobe cloud storage automatically only when someone manually adds an Adobe cloud storage project to it.
* Documents and document folders on the portfolio remain on legacy Workfront storage after the conversion.
* After the conversion, you can't add legacy Workfront storage projects to the portfolio.

## Convert legacy portfolios to Adobe cloud storage

To convert one or more legacy Workfront storage portfolios to Adobe cloud storage:

{{step-1-to-setup}}

1. Select **System** in the left navigation, then select **Preferences**.

1. Scroll down to the **Storage Preferences** section.

1. In the **Select portfolios to convert to Adobe cloud storage** field, select one or more legacy Workfront storage portfolios.

1. Click **Save**.

   A confirmation message appears describing what happens when a portfolio is converted:

   * You can no longer move legacy Workfront storage projects into the portfolio.
   * All new projects created in the portfolio use Adobe cloud storage.
   * Frame.io is the viewer for documents in the portfolio's Adobe cloud storage projects.
   * Child projects that use legacy Workfront storage stay on legacy storage.
   * Child programs stay on legacy storage.

1. Click **Convert** to confirm.

   The selected portfolios are converted to Adobe cloud storage.
