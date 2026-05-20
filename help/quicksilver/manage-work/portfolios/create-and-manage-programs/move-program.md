---
product-area: programs
navigation-topic: create and manage programs
title: Add an Existing Program to a Portfolio
description: You can add existing programs to a portfolio. Because programs cannot exist in two different portfolios, adding an existing program permanently moves it from one portfolio to another.
author: Alina
feature: Work Management, Strategic Planning
exl-id: 73dbe277-12d2-4041-8a02-91ccf5f8b465
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
---
# Add an existing program to a portfolio

<!--Audited: 05/2026-->

<!--
<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. The same features will also be available in the Production environment for all customers after a week from the Preview release. </span>   

<span class="preview">For more information, see [Interface modernization](/help/quicksilver/product-announcements/product-releases/interface-modernization/interface-modernization.md). </span>
-->

You can add existing programs to a portfolio. Because programs cannot exist in two different portfolios, adding an existing program permanently moves it from one portfolio to another. 

## Access requirements

+++ Expand to view access requirements for the functionality in this article.

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
   <td> <p>[!UICONTROL Standard]</p><p>[!UICONTROL Plan]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>[!UICONTROL Edit] access to [!UICONTROL Portfolios] and [!UICONTROL Programs] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>[!UICONTROL Manage] permissions to the portfolio and the program</p> </td> 
  </tr> 
 </tbody> 
</table>

*For information, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md). 

+++

<!--
Old:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] license*</td> 
   <td> <p>New: [!UICONTROL Standard] </p><p>Or </p><p>Current: [!UICONTROL Plan] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>[!UICONTROL Edit] access to Portfolios and Programs </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>[!UICONTROL Manage] permissions to the portfolio and the program</p> </td> 
  </tr> 
 </tbody> 
</table>
-->

## Add an existing program to a portfolio

>[!NOTE]
>
>When your organization uses both legacy Workfront and Adobe cloud storage for documents, the following scenarios exist: 
>
>
>* When you add an Adobe cloud storage program to a legacy Workfront storage portfolio and the portfolio has no documents attached to it, the portfolio is converted to Adobe cloud storage. 
>* When you add an Adobe cloud storage program to a legacy Workfront storage portfolio and the portfolio has documents attached to it, the portfolio documents storage remains on Workfront storage. However, the legacy Workfront storage icon ![Legacy Workfront storage icon](assets/legacy-storage-project-icon.png) is removed from the portfolio.
>* You cannot add a legacy Workfront storage program to an Adobe cloud storage portfolio. 
>
>For more information, see [Document management overview for projects and related objects](/help/quicksilver/manage-work/projects/manage-projects/manage-documents-on-projects.md).
>
>Not all Workfront instances have both types of document storages.

To add an existing program to another portfolio: 

1. Go to a portfolio, then click **[!UICONTROL Programs]** in the left panel.
1. Click **[!UICONTROL New Program]**.
1. Click **[!UICONTROL Existing Program]**.

   The **Add programs** box opens. <!--check screen shot - I logged changes for this casing-->

   ![Add program box](assets/add-programs-box.png)

   >[!IMPORTANT]
   >
   >Adding an existing program carries all projects associated with that program to the portfolio. Be careful not to unintentionally move projects this way.

1. In the **[!UICONTROL Add programs to this portfolio]** field, type the name of a program, then select it when it displays in the list. <!--see the name of this field, I suggested changes here-->

   You can add more than one program.

1. (Optional) Click the **Delete** icon ![Delete icon](assets/delete-icon.png) next to the name of a program if you decide not to add it to the portfolio.

1. Click **[!UICONTROL Add programs]**. 

   The program displays in the **[!UICONTROL Programs]** tab on the portfolio you selected.

