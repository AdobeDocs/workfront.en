---
product-area: portfolios
navigation-topic: create-and-manage-portfolios
title: Delete and Deactivate Portfolios
description: Portfolios are collections of projects or programs in Adobe Workfront. You can delete or deactivate a portfolio if you find that it's irrelevant for your system.
author: Alina
feature: Work Management, Strategic Planning
exl-id: f88669d2-e8e9-4905-a771-1427b1fd32b2
---
# Delete and deactivate portfolios

<!--Audited: 08/2025-->

Portfolios are collections of projects or programs in [!DNL Adobe Workfront]. You can delete or deactivate a portfolio if you find that it's irrelevant for your system.

We recommend deactivating a portfolio that no longer needs to be associated with future projects instead of deleting it, to keep the historic information on the projects that are currently associated with the portfolio and its programs.

## Access requirements

+++ Expand to view access requirements.Expand to view access requirements for the functionality in this article. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] package</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] license</td> 
   <td> <p>[!UICONTROL Standard]</p>
   <p>[!UICONTROL Plan]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>[!UICONTROL Edit] access to Projects and Portfolios</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>[!UICONTROL Manage] permissions on the portfolio </p> </td> 
  </tr> 
 </tbody> 
</table>

For more detail about the information in this table, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--Old:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan</td> 
   <td> <p>Any </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] license</td> 
   <td> <p>[!UICONTROL Standard]</p>
   <p>[!UICONTROL Plan]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>[!UICONTROL Edit] access to Projects and Portfolios</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>[!UICONTROL Manage] permissions on the portfolio </p> </td> 
  </tr> 
 </tbody> 
</table>

For more detail about the information in this table, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).
-->

## Overview of deleting and deactivating portfolios

Consider the following when deciding whether to delete or deactivate portfolios:

* Deleting a portfolio deletes the programs associated with it.

   >[!IMPORTANT]
   >
   >You do not need to have any permissions to programs to be able to delete the portfolio.

* Deleting a portfolio does not delete the projects associated with it.
* You cannot recover deleted portfolios.
* Deactivating a portfolio ensures that the name of the portfolio and its programs can no longer be assigned to projects when creating a project.
* Deactivating a portfolio that is already attached to a project does not remove it from the project. If you remove a deactivated portfolio from a project you must reactivate it before you can reattach it to the project.

## Delete a portfolio

{{step1-to-portfolios}}

1. Do one of the following:

   * Select the portfolio in the list, then click the **[!UICONTROL Delete]** icon ![Delete icon](assets/delete.png).
   * Click the portfolio to open it, then click the **More** menu ![More menu](assets/more-icon.png) to the right of the portfolio name, then **Delete Portfolio**. 
1. Click **[!UICONTROL Yes, Delete It]** to confirm.

   The portfolio is deleted and cannot be recovered. 

## Deactivate a portfolio

When you deactivate a portfolio, you can still access it from the [!UICONTROL Portfolios] area, but it no longer displays in the list of portfolios when users try to add it to a project.

>[!NOTE]
>
>Depending on how your [!DNL Workfront] or group administrator configures your layout template, the [!UICONTROL Portfolios] area might not display in the [!UICONTROL Main Menu]. For more information, see [Customize the Main Menu using a layout template](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-main-menu.md).

{{step1-click-main-menu}}

1. Click **[!UICONTROL Portfolios]** .
1. Click the name of the portfolio.
1. Click the **More** menu ![More menu](assets/more-icon.png) to the right of the portfolio name, then click **[!UICONTROL Deactivate Portfolio]**.
   The portfolio is immediately deactivated. 
1. (Optional) Click the **More** menu ![More menu](assets/more-icon.png) to the right of the portfolio name, then click **[!UICONTROL Activate Portfolio]** to reactivate it. 


