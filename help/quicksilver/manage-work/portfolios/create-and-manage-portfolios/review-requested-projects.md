---
product-area: portfolios;projects
navigation-topic: create-and-manage-portfolios
title: Review Requested Projects
description: Project requests display as projects with a status of [!UICONTROL Requested] in Adobe Workfront. This article describes how to review project requests.
author: Alina
feature: Work Management, Strategic Planning
exl-id: 1acfb885-0da3-495d-ba66-e80e339e90de
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/TedrcHAXyGEp4suJFPRv5p-kgXdFzyKr9h5Vqp4q3E8
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
    internal-label: Work management
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
    internal-label: Administration
subfeature_v2:
  - id: b04e3dc0-3a59-45b1-aa02-b0b6d5f87eff
    internal-label: Approvals
  - id: c10f2e93-7a58-4212-aa24-684c265ebe76
    internal-label: Requests
  - id: f0dd7b45-76b5-49d4-afe3-39f436b6fbd3
    internal-label: Projects
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
---
# Review Requested Projects

<!--Audited: 10/2025-->

When multiple project requests are submitted for review, the project management office or portfolio committee can meet to review submitted requests and determine project request approvals. Project requests display as projects with a status of [!UICONTROL Requested] in [!DNL Adobe Workfront].

You can submit a project request for review by doing one of the following:

* Change the project status to **[!UICONTROL Requested]**.
* Complete the [!UICONTROL Business Case] of the project and submit it for approval.\
   For more information about completing a Business Case for a project, see [Create a Business Case for a project](../../../manage-work/projects/define-a-business-case/create-business-case.md).

You can review requested projects in the following areas of [!DNL Adobe Workfront]:

* In a project report
* Within a portfolio

## Access requirements

+++ Expand to view access requirements for the functionality in this article. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] package</td> 
   <td><p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] license</td> 
   <td> <p>[!UICONTROL Standard] </p> 
   <p>[!UICONTROL Plan]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>[!UICONTROL View] access or higher to Portfolios</p> <p>[!UICONTROL Edit] access to Projects</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>[!UICONTROL View] permissions or higher on the portfolio</p> <p>[!UICONTROL Manage] permissions on the projects to update their status</p>  </td> 
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
   <td><p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] license*</td> 
   <td> <p>[!UICONTROL Plan] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>[!UICONTROL View] access or higher to Portfolios</p> <p>[!UICONTROL Edit] access to Projects</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>[!UICONTROL View] permissions or higher on the portfolio</p> <p>[!UICONTROL Manage] permissions on the projects to update their status</p>  </td> 
  </tr> 
 </tbody> 
</table>
-->

## Review Requested Projects in a project report

You can build a report for projects to see what projects have a status of [!UICONTROL Requested].

For more information about approving project requests by building a project report, see the [[!UICONTROL Approving the Business Case by Building a Project Report]](../../../manage-work/projects/define-a-business-case/approve-business-case.md#build-a-report) section in [Approve a Business Case](../../../manage-work/projects/define-a-business-case/approve-business-case.md). 

## Review Requested Projects within a portfolio

1. Go to the portfolio whose requested projects you want to review.
1. Click **[!UICONTROL Projects]** in the left panel
1. From the **[!UICONTROL Filter]** drop-down menu, select **[!UICONTROL Requested]**.

   Only projects with a status of **[!UICONTROL Requested]** display in the list.

   >[!TIP]
   >
   > In addition to having a Status of **[!UICONTROL Requested]**, projects must be associated with the selected Portfolio to display in this list.

1. Click the name of a project in the list to open it.
1. Click **[!UICONTROL Project Details]** in the left panel.
1. Do either one of the following:

   * Click **[!UICONTROL Business Case]**, then click **[!UICONTROL Approve]** or **[!UICONTROL Reject]** in the [!UICONTROL Business Case Summary] area to approve or reject the Business Case.

      ![approve_or_reject_business_case.png](assets/approve-or-reject-business-case-350x563.png)

      The project status is changed to **[!UICONTROL Approved]** if the Business Case is approved.

      The project status is changed to **[!UICONTROL Rejected]** if the Business case is rejected.

      >[!NOTE]
      >
      >There are no notifications that alert the user who submitted the approval of the business case whether their project request was approved or rejected. 

      Or

   * Change the status of the project to any other status in the **[!UICONTROL Status]** drop-down menu.

      ![Change project status from dropdown](assets/project-status-change-from-drop-down-in-header-nwe-350x294.png)
    

 
