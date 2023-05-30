---
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: Overview of reconciling resource allocations between projects and initiatives
description: Overview of reconciling resource allocations between projects and initiatives
author: Alina
feature: Workfront Scenario Planner
exl-id: 82cd9641-1213-436c-935a-2f04a0425e9c
---
# Overview of reconciling resource allocations between projects and initiatives

>[!IMPORTANT]
>
>Your organization must purchase an additional license for the [!DNL Adobe Workfront Scenario Planner] so that you can view initiative information on a project. For information about obtaining the [!DNL Workfront Scenario Planner], see [Access needed to use the Scenario Planner](../scenario-planner/access-needed-to-use-sp.md) .

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: two more articles were added to split content from here according to where the reconciling can happen) </p>
-->

You can connect projects with initiatives to ensure your strategic plans and the actual work are in sync. As you outline your strategic plans and initiatives in the [!DNL Scenario Planner] and you plan the actual work in a project, you can ensure your resources on both the project and the initiatives match, so you won't either overallocate or underutilize them.

## Prerequisites

Before you begin, you must have the following:

* A plan in the [!DNL Scenario Planner] with an initiative connected to a project. 
* Required job role allocations for the initiative. 
* Tasks or issues on the project that have Planned Hours and are assigned to one of the following:

   * Job roles
   * Users associated with job roles

## Connect projects and initiatives

>[!NOTE]
>
>You can create initiatives and connect them to projects only if your organization has purchased an additional license for the [!DNL Workfront Scenario Planner].

You can connect projects with initiatives by doing one of the following:

* Import projects into a plan, as new initiatives

  For more information, see [Import projects to plans in the [!DNL Scenario Planner]](../scenario-planner/import-projects-to-plans.md).

* Publish initiatives to projects

  For more information, see [Update or create projects by publishing initiatives in the [!DNL Scenario Planner]](../scenario-planner/publish-scenarios-update-projects.md) .

Both processes create a connection between the projects and their corresponding initiatives. After connecting them, you can manage their resource allocations by comparing them and ensuring that they match.

## Considerations about reconciling resources on linked projects and initiatives

>[!NOTE]
>
>You can view initiatives, connect them to projects, and view their resource allocations on a project only if your organization has purchased an additional license for the [!DNL Workfront Scenario Planner].

* You can assign users, teams, and job roles to work items on a project and you can assign job roles to initiatives. As a result, you can only reconcile job roles between projects and initiatives.

  >[!TIP]
  >
  >To reconcile the users' time on a project with role allocations on the initiatives you must associate users with job roles.

* You can view initiative job role allocation on a linked project in the following areas of the project:

   * [!DNL Scenario Planner] section of the [!UICONTROL Project Details] area on a project. For more information, see the following articles:

      * [Update or create projects by publishing initiatives in the [!DNL Scenario Planner]](../scenario-planner/publish-scenarios-update-projects.md) 
      * [Manage information in the project [!UICONTROL Overview] area](../manage-work/projects/manage-projects/understand-project-overview-area.md)

     >[!TIP]
     >
     >You cannot see job role information from the project and the initiative side-by-side in the [!DNL Scenario Planner] section of the [!UICONTROL Project Details].

   * The [!UICONTROL Role Allocation] panel in the following areas:

      * [!IUCONTROL Workload Balancer] of the project

        For information about how to view and reconcile the allocations of roles between the initiative and the linked project in the [!IUCONTROL Workload Balancer], see [Show role allocation for projects and initiatives in the [!IUCONTROL Workload Balancer]](../scenario-planner/show-role-allocation-workload-balancer.md). 
      
      * [!UICONTROL Tasks] section

        For information about how to reconcile the allocations of roles between the initiative and the linked project in the [!UICONTROL Tasks] section, see [Show role allocation for projects and initiatives in the task list](../scenario-planner/show-role-allocation-task-list-nwe.md).

     >[!TIP]
     >
     >You can see job role information from the project and the initiative side-by-side in [!UICONTROL Role Allocation] panel.

* You cannot view job role allocation for a project on a linked initiative. For more information, see [Import projects to plans in the [!DNL Scenario Planner]](../scenario-planner/import-projects-to-plans.md). 

  <!--
  <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
  (NOTE: this might change - project job role visibility into initiative)
  </MadCap:conditionalText>
  -->
