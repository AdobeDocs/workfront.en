---
user-type: administrator
product-area: system-administration
navigation-topic: configure-system-defaults
title: Create a Scorecard
description: A scorecard measures how well a project aligns with the previously established criteria of a portfolio. A scorecard often reflects an organization's mission, values, and strategic goals.Portfolio managers usually define the scorecard questions and answers to ensure they are meaningful and valuable during project prioritization and selection. An [!DNL Adobe Workfront] administrator builds the scorecards based on the recommendations from portfolio managers.
author: Lisa, Alina
feature: System Setup and Administration
role: Admin
exl-id: 89c9b450-72a6-4b72-98d1-22956696543a
---
# Create a scorecard

<!--Audited: 05/2025-->

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.-->

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. The same features will also be available in the Production environment for all customers after a week from the Preview release. </span>   

<span class="preview">For more information, see [Interface modernization](/help/quicksilver/product-announcements/product-releases/interface-modernization/interface-modernization.md). </span>-->

A scorecard measures how well a project aligns with the previously established criteria of a portfolio. A scorecard often reflects an organization's mission, values, and strategic goals.

As a portfolio manager, you can define the scorecard questions and answers to ensure they are meaningful and valuable during project prioritization and selection.

As a [!DNL Adobe Workfront] administrator, you can create scorecards based on the recommendations from portfolio managers.

The questions and answers chosen for a scorecard must be quantifiable in order to provide an alignment value to compare different projects.

You can create a scorecard in the following way:

* From scratch
* By copying an existing one

## Access requirements

+++ Expand to view access requirements for the functionality in this article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan*</td> 
   <td> <p>New: Ultimate</p>
   <p>Current: [!UICONTROL Business] or higher</p> 
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] license*</td> 
   <td><p>New: [!UICONTROL Standard]</p>
   <p>Current: [!UICONTROL Plan]</p>
   </td> 
  </tr> 
   <tr> 
   <td role="rowheader"><p>Access level</p></td> 
   <td><p>System Administrator</p>
   </td> 
  </tr>
 </tbody> 
</table>

*For information, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Create a scorecard from scratch

{{step-1-to-setup}}

1. Click **[!UICONTROL Scorecards]**, then click **[!UICONTROL New Scorecard]**. 

   The **New scorecard** box opens.

   ![New scorecard box](assets/new-scorecard-350x173.png)

1. Specify a **[!UICONTROL Scorecard Name]** and a **[!UICONTROL Description]**.

   The name displays when you are associating the scorecard with the project. The description displays next to the scorecard name in the scorecard list.

1. Click the **[!UICONTROL Add Question]** drop-down menu to open the [!UICONTROL scorecard question] section, then specify the following information for your question:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Question]</td> 
      <td>Type the question you want to include in the scorecard.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Points]</td> 
      <td>Type the maximum points possible for this question.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Negative Points]</td> 
      <td>Select this option to indicate that [!DNL Workfront] should subtract from the total possible points. Negative scores cannot be added to the maximum possible points of a scorecard.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Display Type]</td> 
      <td>Select <strong>[!UICONTROL Value(0-100)]</strong> if you want to display a numeric field in the scorecard where users can specify any value between 0-100.<p>Or, select <strong>[!UICONTROL Drop Down]</strong> or <strong>[!UICONTROL Radio Buttons]</strong> to create an answer users can specify using that control. Click <strong>[!UICONTROL Add Answer]</strong>, then type the <strong>[!UICONTROL Value]</strong> in percentage points for this answer, in case that it is fulfilled. If you choose 100%, the number of points allotted for this question is fully achieved. If you want to indicate that this answer carries only a portion of the total amount of points allotted to this question, select a lower percentage value. For example, if your question is valued at 10 points, and you want this answer to carry 5 of those points, choose 50% for your value.</p>
      <p>Select <strong>[!UICONTROL Default]</strong> if you to indicate that this answer is the default one.</strong></p>
     </tr> 
    </tbody> 
   </table>

1. Click **[!UICONTROL Add Question]** to add more questions and answers to your scorecard, following the same steps.

   >[!NOTE]
   >
   >You can reorder the questions in your scorecard by dragging and dropping the questions in the correct order.

1. Click **[!UICONTROL Save]**.

   This creates the scorecard and project managers can now attach it to their project business case. 

## Copy an existing scorecard

You can create a scorecard by copying and editing an existing one. 

{{step-1-to-setup}}

1. Click **[!UICONTROL Scorecards]** in the left panel. 
1. Select a scorecard in the list, then click the **Copy** icon ![Copy scorecard icon](assets/copy-scorecard-icon.png) at the top of the scorecard list. 
   
   The **Copy Scorecard** box opens.

   ![Copy scorecard box](assets/copy-scorecard-box.png)

1. Specify the following information:

   * **Scorecard**: Update the name of the scorecard.  By default, the name is automatically updated according to the following format: 

      `Original scorecard name (Copy)`
   * **Description**: Type additional information about the scorecard. 
1. Click **Save**.

   This creates a new scorecard with the same information as the original one. Project managers can now attach it to their project business case.

## Apply a scorecard to a project

A user with [!UICONTROL manage] permissions to a project can apply a scorecard to a project, after the scorecard has been created by the [!DNL Workfront] administrator.

A scorecard is added to a project as part of creating a business case for the project. For more information about adding a scorecard to a project, see [Apply a scorecard to a project and generate an Alignment Score](../../../manage-work/projects/define-a-business-case/apply-scorecard-to-project-to-generate-alignment-score.md).

For more information about project permissions, see [Share a project in [!DNL Adobe Workfront]](../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md).


