---
content-type: reference
product-area: resource-management
keywords: workload,balancer
navigation-topic: resource-management-overview
title: Deprecation of Resource Scheduling tools in Adobe Workfront
description: We are currently in the process of deprecating all Scheduling tools from Adobe Workfront and replacing them with the Workload Balancer.
author: Alina
feature: Resource Management
exl-id: 7fa644cd-cf6a-40f8-ae28-bf222bb45d3f
---
# Deprecation of Resource Scheduling tools in Adobe Workfront

We are currently in the process of removing all Scheduling tools from Adobe Workfront and replacing them with the Workload Balancer.

>[!IMPORTANT]
>
>We are no longer implementing new feature functionality for the current Scheduling solution and we no longer consider nor prioritize defects for a fix in this area of Adobe Workfront.

This article describes the timeline for this deprecation and it compares the functionality of the Scheduling tools and that of the Workload Balancer to indicate which Scheduling capabilities are already supported in the Workload Balancer. 

We have been announcing a more exact timeline through the Announcement Center at key milestones during the deprecation process and this article has been updated as this process continues.

>[!NOTE]
>
>The changes described in this article do not affect any other resource management tools. For example, they do not affect the [!UICONTROL Resource Planner] or the [!UICONTROL Utilization] report.

## How you should prepare

For detailed information about how you should prepare for the transition between Scheduling and the Workload Balancer, see [Migrate from Resource Scheduling to the Workload Balancer](../../resource-mgmt/resource-mgmt-overview/migrate-resource-scheduling-to-workload-balancer.md).

If you currently use Scheduling tools we recommend that you discontinue them and start using the Workload Balancer. 

![The global Resource Scheduling area](assets/resource-scheduler-global-350x127.png)

Nearly all capabilities previously available in the Scheduling areas are now available in the Workload Balancer. For information, see the section [Feature availability](#feature-availability) in this article. You can continue scheduling your resources for work exclusively in the Workload Balancer. 

![The global Workload Balancer area](assets/workload-balancer-pti-350x111.png)

## Information that will not transfer to the Workload Balancer

The following information will not transfer from the Scheduling tools to the Workload Balancer:

* **Daily allocations for users**: You should not use both Scheduling and the Workload Balancer at the same time to adjust the same user allocations. If you have managed user allocations in the Scheduling tools, the adjusted daily allocations do not transfer to the Workload Balancer. Similarly, if you have adjusted user allocations in the Workload Balancer, they do not transfer to the Scheduling tools. We strongly encourage you to ensure that the daily allocations are accurate in the Workload Balancer to prepare for this transition. For information, see [Manage user allocations in the Workload Balancer](../workload-balancer/manage-user-allocations-workload-balancer.md).
* **Filters**: If you have saved filters in the Scheduling areas, they do not transfer to the Workload Balancer. You must recreate the filters in the Workload Balancer. For information, see [Filter information in the Workload Balancer](../workload-balancer/filter-information-workload-balancer.md). 

## Deprecation timeline highlights

>[!IMPORTANT]
>
>Use this article to understand the latest timeline for deprecating the Scheduling tools. Any updates to this timeline will be communicated in this article and in Announcement Center messages.

The following is a timeline for the deprecation process of Resource Scheduling tools:

* [2020.4 release (November 2020)](#2020-4-release-november-2020) 
* [2021.4 release (October 2021)](#2021-4-release-october-2021) 
* [2022.4 - 2023.1 releases (October 2022 - January 2023)](#20224-release-october-2022-tentative)

### 2020.4 release (November 2020) {#2020-4-release-november-2020}

* New feature functionality is no longer implemented for the Scheduling solution
* Only High and Critical severity defects will be prioritized for a fix
* New Workload Balancer capabilities added to Workfront

### 2021.4 release (October 2021) {#2021-4-release-october-2021}

* Workload Balancer is set as default for any first-time user of Workfront
* Enhanced filters that can be shared and include additional fields

### 2022.4 - 2023.1 releases (October 2022 - January 2023) 

* No defects will be prioritized for a fix during and after the 2022.4 or 2023.1 releases
* <span class="preview"> All Scheduling areas are removed from the Preview environment </span> (**October 20, 2022**)
* All Scheduling areas are removed from the Production environment (**January, 2023**)
* The Workload Balancer is the only resource scheduling tool available in Workfront (after **January, 2023**)

## Feature availability {#feature-availability}

Unless otherwise specified, all Resource Scheduling features have been or will be available in the Workload Balancer. For information about the Workload Balancer, see [Overview of the Workload Balancer](../../resource-mgmt/workload-balancer/overview-workload-balancer.md).

In addition to existing features, the Workload Balancer has or will have new functionality that did not exist in the Resource Scheduling tools, as shown in the following table: 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td rowspan="2"><span style="font-weight: normal;"><b>Features</b></span> </td> 
   <td rowspan="2"> <b>Resource Scheduling tools feature availability</b></td> 
   <td colspan="3"><b>Workload Balancer feature availability</b></td> 
  </tr> 
  <tr> 
   <td><b>Available now</b></td> 
   <td><b>Available soon</b></td> 
   <td><b>Not planned</b></td> 
  </tr> 
  <tr> 
   <td> <p>Access tool from the Resourcing area</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>&nbsp;</td> 
   <td>&nbsp;</td> 
  </tr> 
  <tr> 
   <td>Separate areas for unassigned and assigned work</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>&nbsp;</td> 
   <td>&nbsp;</td> 
  </tr> 
  <tr> 
   <td>Apply and create filters for unassigned and assigned work</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>&nbsp;</td> 
   <td>&nbsp;</td> 
  </tr> 
  <tr> 
   <td>Access work items directly from the tool</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>&nbsp;</td> 
   <td>&nbsp;</td> 
  </tr> 
  <tr> 
   <td>Manually assign or unassign tasks and issues</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>&nbsp;</td> 
   <td>&nbsp;</td> 
  </tr> 
  <tr> 
   <td>Adjust individual allocations</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>&nbsp;</td> 
   <td>&nbsp;</td> 
  </tr> 
  <tr> 
   <td>Include issue time</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>&nbsp;</td> 
   <td>&nbsp;</td> 
  </tr> 
  <tr> 
   <td>Display projected dates </td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>&nbsp;</td> 
   <td>&nbsp;</td> 
  </tr> 
  <tr> 
   <td>Display completed work</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>&nbsp;</td> 
   <td>&nbsp;</td> 
  </tr> 
  <tr> 
   <td>Show user time off, weekends, and schedule exceptions</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>&nbsp;</td> 
   <td>&nbsp;</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><span>Quickly assign users based on roles*</span> </td> 
   <td>✓</td> 
   <td><span>✓</span> </td> 
   <td>&nbsp;</td> 
   <td>&nbsp;</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><span>Quickly replace users*</span> </td> 
   <td>✓</td> 
   <td><span>✓</span> </td> 
   <td>&nbsp;</td> 
   <td>&nbsp;</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><span>Quickly unassign users*</span> </td> 
   <td>✓</td> 
   <td><span>✓</span> </td> 
   <td>&nbsp;</td> 
   <td>&nbsp;</td> 
  </tr> 
  <tr> 
   <td><span>Access tool from a team</span> </td> 
   <td>✓</td> 
   <td><span>✓</span> </td> 
   <td>&nbsp;</td> 
   <td>&nbsp;</td> 
  </tr> 
  <tr> 
   <td><span>Access tool from a project</span> </td> 
   <td>✓</td> 
   <td><span>✓</span> </td> 
   <td>&nbsp;</td> 
   <td>&nbsp;</td> 
  </tr> 
  <tr>
   <td>Work-license users can adjust user allocations when accessing the Workload Balancer from a project </td> 
   <td>✓</td> 
   <td>✓</td> 
   <td></td> 
   <td></td> 
  </tr> 
  <tr> 
   <td>Display issues in the Unassigned Work area</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td></td> 
   <td></td> 
  </tr> 
  <tr> 
   <td><span>Assign and unassign tasks and issues by dragging and dropping*</span> </td> 
   <td>✓</td> 
   <td><span>✓</span> </td> 
   <td>&nbsp;</td> 
   <td>&nbsp;</td> 
  </tr> 
  <tr> 
   <td>Visible to all Plan users, without being designated a Resource Manager on the project.</td> 
   <td>&nbsp;</td> 
   <td>✓</td> 
   <td>&nbsp;</td> 
   <td>&nbsp;</td> 
  </tr> 
  <tr> 
   <td>Group information by project</td> 
   <td>&nbsp;</td> 
   <td>✓</td> 
   <td>&nbsp;</td> 
   <td>&nbsp;</td> 
  </tr> 
  <tr> 
   <td>Share the Workload Balancer with users with no access to the Resourcing area</td> 
   <td>&nbsp;</td> 
   <td>✓</td> 
   <td>&nbsp;</td> 
   <td>&nbsp;</td> 
  </tr> 
  <tr> 
   <td>Display and adjust allocations by week</td> 
   <td>&nbsp;</td> 
   <td>✓</td> 
   <td>&nbsp;</td> 
   <td>&nbsp;</td> 
  </tr> 
  <tr> 
   <td>Access users directly from the tool</td> 
   <td>&nbsp;</td> 
   <td>✓</td> 
   <td>&nbsp;</td> 
   <td>&nbsp;</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>Access more information about work items without navigating away, using the Summary panel*</td> 
   <td>&nbsp;</td> 
   <td>✓</td> 
   <td>&nbsp;</td> 
   <td>&nbsp;</td> 
  </tr> 
  <tr> 
   <td>Display and adjust allocation as a percentage value </td> 
   <td>&nbsp;</td> 
   <td>✓</td> 
   <td>&nbsp;</td> 
   <td>&nbsp;</td> 
  </tr> 
  <tr> 
   <td>Display the difference between the available and allocated time</td> 
   <td>&nbsp;</td> 
   <td>✓</td> 
   <td>&nbsp;</td> 
   <td>&nbsp;</td> 
  </tr> 
  <tr> 
   <td>Display user availability in a chart</td> 
   <td>&nbsp;</td> 
   <td>✓</td> 
   <td>&nbsp;</td> 
   <td>&nbsp;</td> 
  </tr> 
  <tr> 
   <td>Color-code work items and projects by Project Status</td> 
   <td>&nbsp;</td> 
   <td>✓</td> 
   <td>&nbsp;</td> 
   <td>&nbsp;</td> 
  </tr> 
  <tr> 
   <td>Automatically update Planned Hours as you adjust user allocation (for tasks with a Simple Duration Type)</td> 
   <td>&nbsp;</td> 
   <td>✓</td> 
   <td>&nbsp;</td> 
   <td>&nbsp;</td> 
  </tr> 
  <tr> 
   <td><span>Suggest assignments based on the user's assignment pattern, existing Role or Team assignments</span> </td> 
   <td>&nbsp;</td> 
   <td><span>✓</span> </td> 
   <td>&nbsp;</td> 
   <td>&nbsp;</td> 
  </tr> 
  <tr> 
   <td>Enhanced filters that can be shared and include additional fields</td> 
   <td>&nbsp;</td> 
   <td>✓</td> 
   <td>&nbsp;</td> 
   <td>&nbsp;</td> 
  </tr> 
  <tr> 
   <td><span>Make advanced assignments</span> </td> 
   <td>&nbsp;</td> 
   <td><span>✓</span> </td> 
   <td>&nbsp;</td> 
   <td>&nbsp;</td> 
  </tr>

   <tr> 
   <td><span>Color-code work items by projects and project status</span> </td> 
   <td>&nbsp;</td> 
   <td><span>✓</span> </td> 
   <td>&nbsp;</td> 
   <td>&nbsp;</td> 
    
   <tr> 
   <td>Add users to the project team (relocated to the <b>People</b> tab of the project) </td> 
   <td>✓</td> 
   <td>✓</td> 
   <td></td> 
   <td>&nbsp;</td> 

  </tr>
   <tr> 
   <td>Automatically assign tasks and issues</td> 
   <td>✓</td> 
   <td>&nbsp;</td> 
   <td>&nbsp;</td> 
   <td>✓</td> 
  </tr> 

 </tbody> 
</table>

*These features are available only in the new Adobe Workfront experience.
