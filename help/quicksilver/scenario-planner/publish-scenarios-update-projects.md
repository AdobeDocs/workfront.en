---
product-area: enterprise-scenario-planner-product-area
keywords: publish,plans,projects,scenario,scenarios
navigation-topic: enterprise-scenario-planner-navigation-topic
title: Update or create projects by publishing initiatives in the Scenario Planner
description: You can create projects from existing initiatives as well as update projects previously linked to initiatives by publishing scenarios in the Adobe Workfront Scenario Planner.
author: Alina
feature: Workfront Scenario Planner
exl-id: 46d3666a-4454-4a84-8c02-a79f3947a18f
---
# Update or create projects by publishing initiatives in the [!DNL Scenario Planner]

Publishing a scenario from the [!DNL Adobe Workfront Scenario Planner] accomplishes the following:

* Creates projects from the initiatives on the scenario and links them together.
* Updates projects already linked to initiatives on the scenario with information from the linked initiative. Projects can also be linked to initiatives when you import them in to a plan. For information, see [Import projects to plans in the [!DNL Scenario Planner]](../scenario-planner/import-projects-to-plans.md)

## Access requirements

+++ Expand to view access requirements for the functionality in this article. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront] plan*</p> </td> 
   <td> <p>Current: [!UICONTROL Business] or higher</p>
   <p>New: Ultimate </p>
   </td> 
  </tr> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront] license*</p> </td> 
   <td> <p>New: Light or higher</p> 
   <p>Current: [!UICONTROL Review] or higher</p> </td> 
  </tr> 
  <tr> 
   <td>Product* </td> 
   <td> 
   <p>For the current Workfront plans: </p>
   <p>You must purchase an additional license for the [!DNL Adobe Workfront Scenario Planner] to access functionality described in this article.</p> <p>For information about access and permissions for the [!DNL Workfront Scenario Planner], see <a href="../scenario-planner/access-needed-to-use-sp.md" class="MCXref xref">Access needed to use the [!DNL Scenario Planner]</a>. </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>Access level </td> 
   <td> <p>[!UICONTROL Edit] access for the [!DNL Scenario Planner] and [!UICONTROL Projects]</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p>Object permissions </p> </td> 
   <td> <ul> 
     <li>[!UICONTROL Manage] permissions for the plan </li> 
     <li>[!UICONTROL Manage] permissions for published projects</li> 
    </ul> <p>For information on requesting additional access to a plan, see <a href="../scenario-planner/request-access-to-plan.md" class="MCXref xref">Request access to a plan in the [!DNL Scenario Planner]</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*For information, see [Access requirements to Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md). 

+++

## Prerequisites

Before you begin:

* You must create and save a plan before you can publish initiatives from it.
* The Allow users to create projects without using a template setting must be enabled in your Project Preferences area of the Setup. For information, see [Configure system-wide project preferences](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

## Considerations about publishing initiatives to projects

* You can publish only one scenario from a plan. 
* One initiative can be linked to only one project.
* One project can be linked to more than one initiative when the initiatives belong to different plans.

  >[!TIP]
  >
  >When a project exists on multiple plans and you publish information to the project from all plans, the latest publish overwrites the existing [!DNL Scenario Planner] information on the project.

* If initiatives were created on the plan by importing projects to the plan, publishing the initiative also updates the linked projects with initiative information.

  >[!TIP]
  >
  >You can import the same project into multiple plans. Publishing might overwrite initiative information on a project that is linked to multiple initiatives.

  For information about creating initiatives by importing projects, see [Import projects to plans in the [!DNL Scenario Planner]](../scenario-planner/import-projects-to-plans.md). 

* Any changes made to the project do not transfer to the linked initiative.

 

## Publish initiatives

>[!IMPORTANT]
>
>If you make any changes to initiatives on the plan, including resolve conflicts, you must republish the initiative in order for the new information to be visible on the project. This information displays on the projects linked to initiatives only when you publish the corresponding the initiative. For information about resolving conflicts between initiatives, see [Resolve initiative conflicts in the [!DNL Scenario Planner]](../scenario-planner/resolve-conflicts-in-sp.md)

{{step1-to-scenario-planner}}

1. (Optional and conditional) If you want to publish from an existing plan, click the **[!UICONTROL Filter]** icon ![](assets/filter-nwepng.png) in the upper-right corner of the plan and select one of the following options:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL All]</td> 
      <td>Displays all plans that you own or are shared with you. This is the default. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL My plans]</td> 
      <td>Displays plans that you created.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Shared with me]</td> 
      <td> <p>Displays plans you did not create but are shared with you.</p> <p>Important: You must have [!UICONTROL Manage] permissions to plans shared with you to be able to publish them. </p> </td> 
     </tr> 
    </tbody> 
   </table>

   ![](assets/plans-filters-dropdown-options-scenario-planer.png)

1. (Optional) Click the **[!UICONTROL Search]** icon ![](assets/search-icon.png) and start typing the name of a plan to quickly find it in the list.
1. (Conditional) To publish from a new plan, create a plan.

   For information about creating plans, see [Create and edit plans in the [!DNL Scenario Planner]](../scenario-planner/create-and-edit-plans.md) . 

1. (Optional) Click the name of an existing plan and create new scenarios for the plan.

   For information about creating scenarios for a plan, see [Create and compare plan scenarios in the [!DNL Scenario Planner]](../scenario-planner/create-and-compare-scenarios-for-a-plan.md). 

1. (Optional) Update the initiatives of an existing or a new plan or create new ones.

   For information about creating initiatives, see [Create and edit initiatives in the [!DNL Scenario Planner]](../scenario-planner/create-and-edit-initiatives.md).

1. Click **[!UICONTROL Save plan]**. 
1. Select the scenario you want to publish from the **[!UICONTROL Initial scenario]** drop-down menu, then click **[!UICONTROL Go to Publish]** ![](assets/go-to-publish-button-icon.png) in the upper-right corner.

   Or

   Click **[!UICONTROL Compare scenarios]**, hover over the scenario card that you want to publish from, then click **[!UICONTROL Go to Publish]** ![](assets/go-to-publish-button-icon.png).

   The [!UICONTROL Publish initiatives] page displays, showing a list of all initiatives in the scenario. If any of the initiatives was previously published, the project icon ![](assets/project-icon-sp.png) displays after their name and the **[!UICONTROL Last published]** date is populated in the list.

   >[!TIP]
   >
   >Initiatives that have been created by importing projects also display the project icon ![](assets/project-icon-sp.png) to the right of their name

   ![](assets/project-icons-and-last-published-date-in-publish-initiative-page-350x63.png)

1. (Optional and conditional) If you want to publish from an existing plan, click the **[!UICONTROL Filter]** icon ![](assets/filter-nwepng.png) in the upper-right corner of the plan and select one of the following options:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL All]</td> 
      <td>Displays all initiatives of the selected scenario. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Published]</td> 
      <td>Displays initiatives that you or another user published before. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Unpublished]</td> 
      <td> <p>Displays unpublished initiatives. </p> </td> 
     </tr> 
    </tbody> 
   </table>

   ![](assets/initiatives-fitler-in-publishing-screen-scenario-planner.png)

1. (Optional) Click the **[!UICONTROL Search]** icon ![](assets/search-icon.png) and start typing the name of an initiative to quickly find it in the list.
1. Select one or multiple initiatives to publish and create or update projects from them, then click **[!UICONTROL Publish initiatives]**.

   This creates a new project from each selected initiatives or updates the existing connected projects, if the published initiatives were already linked to a project.

   >[!TIP]
   >
   >New projects have the same name as the published initiatives.

1. (Conditional) Do one of the following:

   * If you published one initiative, click **[!UICONTROL See associated project]** to open the project created or updated from the initiative. 
   * If you published more than one initiative, click **[!UICONTROL See associated projects]** to open a list of projects published from initiatives. [!DNL Workfront] applies the [!DNL Scenario Planner] Projects filter to the list of projects by default. The projects published most recently display at the top of the list.

     ![](assets/scenario-planner-filter-after-publishing-initiatives-350x81.png)

1. Go to the following areas to view initiative information on the project:

   * **The [!UICONTROL Updates] section**: An update publishes to indicate that the project was created or updated from the initiative. The update contains the name of the initiative that created or updated the project and the linked name of the plan that contains the initiative. You can click the name of the plan in the update to open the plan in the [!DNL Scenario Planner].

     ![](assets/update-stream-confirmation-of-publish-on-project-350x65.png)

   * **The [!UICONTROL Overview] area of the [!UICONTROL Project Details] section**: A new [!DNL Scenario Planner] section is created in this area that contains information from the linked initiative.

     ![](assets/scenario-planner-on-project-details-350x135.png)

     The following initiative information is published in the [!DNL Scenario Planner] area of the [!UICONTROL Project Details] section:

     <table style="table-layout:auto"> 
      <col> 
      <col> 
      <tbody> 
       <tr> 
        <td role="rowheader"><span>[!UICONTROL Initiative Duration]</span> </td> 
        <td><span>The duration of the corresponding initiative when the project is linked to an initiative. This field is not editable.</span> </td> 
       </tr> 
       <tr> 
        <td role="rowheader"><span>[!UICONTROL Last Published Date]</span> </td> 
        <td><span>The date when the project was last published from a corresponding initiative.</span> </td> 
       </tr> 
       <tr> 
        <td role="rowheader"><span>[!UICONTROL Initiative Start Date]</span> </td> 
        <td><span>The first day of the start month of the initiative, when the project is linked to an initiative.</span> </td> 
       </tr> 
       <tr> 
        <td role="rowheader"><span>[!UICONTROL Initiative End Date]</span> </td> 
        <td><span>The last day of the end month of the initiative, when the project is linked to an initiative. </span> </td> 
       </tr> 
       <tr> 
        <td role="rowheader"><span>[!UICONTROL Initiative Job Roles in FTEs and Hours]</span> </td> 
        <td> <p>Information about the associated job roles and their time allocations for the initiative. This includes:</p> 
         <ul> 
          <li>Job Role name</li> 
          <li>Number of FTEs</li> 
          <li> <p>Number of Hours for all FTEs</p> <p>You can estimate the amount of job roles needed for your plan or initiative using hours or FTEs.</p> <p>For more information, see <a href="../scenario-planner/create-and-edit-plans.md" class="MCXref xref">Create and edit plans in the Scenario Planner</a>. </p> </li> 
         </ul> 
      <p><b>TIP</b> 
      
      If the number of job role is different for each month in the initiative, this field displays the maximum amount of roles needed for the initiative. For example, if you need 1 Consultant for January and 2 for February, the column displays 2FTE and the corresponding amount of hours for 2 FTEs for all months.</p> </td> 
       </tr> 
      </tbody> 
     </table>

     >[!NOTE]
     >
     >All users with [!UICONTROL View] access to the project can see the [!DNL Scenario Planner] section in the [!UICONTROL Overview] area. You can control whether this area displays in the [!UICONTROL Details] section by using a layout template. If users do not have a layout template associated with them, this area displays by default. 
     >
     >   
     >   
     >   * For information about adding or removing areas in the [!UICONTROL Details] section using a layout template, see [Customize the [!UICONTROL Details] view using a layout template](../administration-and-setup/customize-workfront/use-layout-templates/customize-details-view-layout-template.md). 
     >   * For more information about viewing information in the [!UICONTROL Overview] area of the [!UICONTROL Project Details], see [[!UICONTROL Manage] information in the project [!UICONTROL Overview] area](../manage-work/projects/manage-projects/understand-project-overview-area.md).
     >   
     >

   * **The [!UICONTROL Role Allocation] panel in the [!UICONTROL Workload Balancer] or the task list of the project**: Information about role allocation on the initiative populates in this area, in addition to role allocations on the project.

     For more information, see [Overview of reconciling resource allocations between projects and initiatives](../scenario-planner/overview-reconcile-allocations-between-projects-initiatives.md).

     ![](assets/role-allocation-panel-350x174.png)

     Any changes to the dates or resources of the project do not affect the corresponding initiative or any of the areas on the project that contain initiative information. 
   
   * **The [!UICONTROL Resource Budgeting] area of the [!UICONTROL Business Case] of the project**: A new option for managing project resources using [!DNL Scenario Planner] information is added in the [!UICONTROL Resource Budgeting] area of the [!UICONTROL Business Case] of the project.

     For more information, see [Budget resources in the [!UICONTROL Business Case] using the [!DNL Scenario Planner]](../manage-work/projects/define-a-business-case/budget-resources-in-business-case-use-scenario-planner.md).

     ![](assets/sp-in-business-case-selected-350x110.png)

1. (Optional) Review the following information in the [!DNL Scenario Planner] after you published a scenario:

   * The published scenario becomes the first scenario after you publish initiatives from it. 
   * You cannot publish from any other scenario after you have published a scenario at least once. 
   * The [!UICONTROL Go to Publish] option is removed from all other scenarios after at least one initiative has been published from a scenario. 
   * A green indicator displays next to the published initiatives' project icons in the plan.

     ![](assets/indicator-for-published-initiative-icon-350x119.png)

   * A green "Published" indicator displays at the top of the scenario and on the scenario card and the Published field is populated on the scenario card indicating the number of initiatives in the scenario that have been published.

     ![](assets/published-scenario-highlighted-350x632.png)

     >[!TIP]
     >
     >If all the projects published from the scenario's initiatives are deleted, the indication that the scenario has been published is removed. For information, see [Delete projects](../manage-work/projects/manage-projects/delete-projects.md).

1. (Optional) Update information on the initiative and repeat the process described above to republish the initiative and update initiative information on the linked project.

   For information about editing initiatives, see [Create and edit initiatives in the [!DNL Scenario Planner]](../scenario-planner/create-and-edit-initiatives.md).

 
