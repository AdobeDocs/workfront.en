---
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: Show Role allocation for Projects and Initiatives in the Workload Balancer
description: After you connect projects and initiatives, you can manage their resource allocation side-by-side to ensure they
author: Alina
feature: Workfront Scenario Planner
exl-id: cdc3a1b0-7021-4853-9b51-c3682fd55430
---
# Show role allocation for projects and initiatives in the [!UICONTROL Workload Balancer]

<!--Audited: 07/2024-->

After you connect projects and initiatives, you can manage their resource allocation side-by-side to ensure they match. This avoids overallocating or underutilizing them.

This article describes how you can reconcile resources using the [!UICONTROL Role Allocation] panel in [!UICONTROL Workload Balancer] of a project.

For general information about reconciling resources between projects and initiatives, including prerequisites, see [Overview of reconciling resource allocations between projects and initiatives](../scenario-planner/overview-reconcile-allocations-between-projects-initiatives.md).

## Access requirements

+++ Expand to view access requirements for the functionality in this article. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront] package</p> </td> 
   <td> 
   <p>Workfront Ultimate</p>
<p><b>NOTE</b></p>
<p>Speak with your Workfront representative if you have a different Workfront package.</p>
   </td> 
  </tr> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront] license</p> </td> 
   <td> <p>[!UICONTROL Light] or higher</p> 
   <p>[!UICONTROL Review] or higher</p> </td> 
  </tr> 
    <tr> 
   <td>Access level configurations</td> 
   <td> <p>View or higher access to Projects.</p></td> 
  </tr> 
  <tr> 
   <td> <p>Object permissions </p> </td> 
   <td> <p> View or higher permission to a project.</p></td> 
  </tr> 
 </tbody> 
</table>

For more information about access to the Scenario Planner, see [Access needed to use the [!DNL Scenario Planner]]( ../scenario-planner/access-needed-to-use-sp.md).

For information about Workfront access requirements, see [Access requirements to Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md). 

+++

<!--Old:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront] plan*</p> </td> 
   <td> <ul></li>
   <li><p>New: Ultimate </p></li>
   <p>The Scenario Planner is not available for the new Workfront Select or Workfront Prime plans. </p>
   <li><p>Current: [!UICONTROL Business] or higher</p></ul>
   </td> 
  </tr> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront] license*</p> </td> 
   <td> <p>New: Light or higher</p> 
   <p>Current: [!UICONTROL Review] or higher</p> </td> 
  </tr> 
  <tr> 
   <td>Product* </td> 
   <td> <ul><li><p>For the new Workfront plans:</p><p> Adobe Workfront</li></p>
   <li><p>For the current Workfront plans: </p>
   <p>Adobe Workfront</p> <p>Adobe Workfront Scenario Planner</p></li></ul>
   
   <p>For more information, see <a href="../scenario-planner/access-needed-to-use-sp.md" class="MCXref xref">Access needed to use the [!DNL Scenario Planner]</a>. </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>Access level </td> 
   <td> <p>View or higher access to Projects.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p>Object permissions </p> </td> 
   <td> <p> View or higher permission to a project.</p> </td> 
  </tr> 
 </tbody> 
</table>-->

## Show role allocation for projects and initiatives in the [!UICONTROL Workload Balancer]

If your company has purchased a [!DNL Workfront Scenario Planner] license, you can reconcile the resource allocations between the initiative and the project linked to it in the project-level [!UICONTROL Workload Balancer].

1. (Conditional) Connect a project with an initiative using one of the methods described in the following articles:

   * [Import projects to plans in the [!DNL Adobe Workfront Scenario Planner]](import-projects-to-plans.md).
   * [Update or create projects by publishing initiatives in the [!DNL Adobe Workfront Scenario Planner]](publish-scenarios-update-projects.md). 

   >[!IMPORTANT]
   >
   >If you make changes to resources on the initiative, you must re-publish the scenario that the initiative belongs to in order for the latest resource information from the initiative to update on the project.

1. Go to the project where you want to review the allocation of job roles for the project as well as for the associated initiative. 
1. Click [!UICONTROL Workload Balancer] in the left panel.

   You might have to click **[!UICONTROL Scheduling]**, then **[!UICONTROL Switch to Workload Balancer]**. 

1. Do one of the following:

   * Click **[!UICONTROL Month]** to view the Workload Balancer by month, click the drop-down menu next to a month in the timeline ![Dropdown next to month](assets/drop-down-next-to-month-month-view-wb.png), then click **[!UICONTROL More]**. 
   * Click the **[!UICONTROL Show role allocation]** icon ![Show role allocation](assets/show-role-allocation-icon.png) in the upper-right corner of the toolbar.

   The [!UICONTROL Role Allocation] panel displays.

   ![Role allocation panel](assets/role-allocation-panel-months-collapsed-350x319.png)

   >[!CAUTION]
   >
   >Although you can view the [!UICONTROL Role Allocation] panel even if your organization did not purchase a [!DNL Workfront Scenario Planner] license, you cannot view information about initiatives' job roles.

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: ensure this step stays 5 to match the mention of it in the section below)</p>
   -->

1. Review the following information in the **[!UICONTROL Project Totals]** area of the Role Allocation panel: 

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Job Role]</td> 
      <td> <p>The names of the job roles associated with any of the following:</p> 
       <ul> 
        <li> <p>tasks on the project</p> </li> 
        <li> <p>issues on the project</p> </li> 
        <li> <p>initiative linked to the project</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Initiative Hours]</td> 
      <td>The number of required hours associated with each job role on the initiative for the total duration of the initiative. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Planned Hours]</td> 
      <td>The number of Planned Hours associated with each job role in the tasks or issues on the project for the total duration of the project. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Variance]</td> 
      <td> <p>The difference between the hours required on the initiative and the planned hours associated with work on the project. [!DNL Workfront] calculates the [!UICONTROL Variance] using this formula:</p> <p><code>Role Allocation Variance = Initiative Hours - Planned Hours</code> </p> <p>When resources are planned for more hours than required on the initiative, the [!UICONTROL Variance] is negative and it displays in red. This means your resources are overallocated. </p> </td> 
     </tr> 
    </tbody> 
   </table>

   >[!TIP]
   >
   >Planned Hours from the project do not display in the following scenarios: 
   >
   >   
   >   
   >   * When tasks or issues are not assigned to job roles, or users with a job role associated with them.
   >   * When tasks or issues have a [!UICONTROL Duration] of zero. 
   >   
   >

1. (Optional) If the [!UICONTROL Variance] column shows that your resources are overallocated, adjust one of the following:

   * Lower the number of Planned Hours for one job role that shows overallocated or add more resources to the tasks and distribute more Planned Hours to the new resources. You can update assignments or the number of Planned Hours on tasks or issues when editing them. For more information see the following articles:

      * [Edit tasks](../manage-work/tasks/manage-tasks/edit-tasks.md) 
      * [Edit issues](../manage-work/issues/manage-issues/edit-issues.md)

     >[!NOTE]
     >
     >You must have additional access and permissions to edit tasks and issues.

   * Increase the number of required hours for role that shows the overallocation on the initiative. For more information, see [Create and edit initiatives in the [!DNL Adobe Workfront Scenario Planner]](create-and-edit-initiatives.md).

     >[!NOTE]
     >
     >You must have additional access and permissions to edit plans.

1. (Optional) Click the drop-down icon to expand one of the months in the [!UICONTROL Role Allocation] panel or in the timeline of the [!UICONTROL Workload Balancer].

   ![Expand month in role allocation panel](assets/month-expanded-highlighted-role-allocation-panel-wb-350x145.png)

   The same type of information displayed in the [!UICONTROL Project Totals] area also displays for each month.

   >[!TIP]
   >
   >The months listed in the [!UICONTROL Role Allocation] panel are the months in the timeline displayed on the screen in the [!UICONTROL Workload Balancer]. Scroll back and forward on the timeline to view additional months.

   <!--
   <li value="8" data-mc-conditions="QuicksilverOrClassic.Draft mode"> <p> </p> </li>
   -->

 
