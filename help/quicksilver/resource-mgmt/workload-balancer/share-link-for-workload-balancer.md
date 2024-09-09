---
product-area: resource-management
navigation-topic: the-workload-balancer
title: Share the Workload Balancer with a Link
description: You can share the Workload Balancer with other users who might not have the Resourcing area available to them. For information about using the Workload Balancer, see Navigate the Workload Balancer.
author: Lisa
feature: Resource Management
exl-id: e2d6b1f8-bdc9-4a34-bdc3-b56f7aa2e7a5
---
# Share the Workload Balancer with a link

You can share the Workload Balancer with other users who might not have the Resourcing area available to them. For information about using the Workload Balancer, see [Navigate the Workload Balancer](../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

## Access requirements

+++ Expand to view access requirements for the functionality in this article.

You must have the following access to perform the steps in this article:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan</td> 
   <td> <p>Any </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license</td> 
   <td><p>New: Standard</p>
       <p>or</p>
       <p>Current: Plan, when using the Workload Balancer in the Resourcing area;</br>
       Work, when using the Workload Balancer of a team or project</p></td>
  </tr>
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>View or higher access to the following:</p> 
    <ul> 
     <li>Resource Management</li> 
     <li>Projects</li> 
     <li>Tasks</li> 
     <li>Issues</li> 
    </ul>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td>View or higher permissions to the projects, tasks, and issues</td> 
  </tr> 
 </tbody> 
</table>

For more detail about the information in this table, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Information included in the Workload Balancer when viewing it from a shared link

When you share a link to the Workload Balancer with other users, the following information is included with the shared link:

* The Assigned Work area of the Workload Balancer. 
* Project, task, user information. This includes the user allocation information. 
* The information displays according to the selected filter.

  >[!IMPORTANT]
  >
  >If you delete the filters after you shared the link, the users viewing the Workload Balancer from the link receive a warning that the filters were deleted. They view all users in the Assigned Work area. This is the default view for the Workload Balancer.

* The number of weeks previously selected.

The following options are available to the user viewing the Workload Balancer from a shared link to update themselves:

* The following timeline selections:

   * Today 
   * Back and forward icons
   * Calendar selection

* The Day, Week, and Month icons 
* The Settings icon
* The Show allocations icon

  For information about using these options, see [Navigate the Workload Balancer](../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md). 

* The Show role allocations icon

  This is available only for the Workload Balancer of a project.

The user who receives the shared link cannot do the following in the Workload Balancer from this link:

* Assign work items to users
* Manage user allocations
* Build new or update originally applied filters

## Access needed to view information in the Workload Balancer from a shared link

You need the following access to view information in the Workload Balancer from a shared link:

* A valid Adobe Workfront license and you must be logged in to Workfront. 
* At least&nbsp;View access to Resource Management in your Access Level. For information about granting Resource Management access, see [Grant access to Resource Management](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-resource-management.md). 
* View permissions to the projects, tasks, issues, and users displayed in the Workload Balancer.

## Share the Workload Balancer with other users from a link

1. Go to the Workload Balancer

   For information about accessing the Workload Balancer, see [Navigate the Workload Balancer](../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md). 

1. (Optional) Do one or more of the following:

   * Update the time period selection.
   * Click **Day, Week**, or **Month** to view daily, weekly, or monthly information.

     ![](assets/month-icon-on-toolbar-selected-wb-350x226.png)

   * Apply filters to the Unassigned and Assigned Work areas.

     For information about filtering information in the Workload Balancer, see [Filter information in the Workload Balancer](../../resource-mgmt/workload-balancer/filter-information-workload-balancer.md).

1. Click the **link icon** ![](assets/wb-shearable-link-icon-small.png).

   This adds the link to your clipboard. 

1. Do one of the following to share the link with others:

   * Paste it into an e-mail, chat message, or any other application and share that with other users. 
   * Add it to a custom section as an external page, add the custom section to a user's profile, or to a Layout Template, then share the Layout Template with users, teams, job roles, or groups.

     For information about creating an&nbsp;External Page, see [Embed an external web page in a dashboard](../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/embed-external-web-page-dashboard.md). For information about adding custom sections to a Layout Template, see [Customize the left panel using a layout template](../../administration-and-setup/customize-workfront/use-layout-templates/customize-left-panel.md).

     >[!IMPORTANT]
     >
     >When you add the Workload Balancer to the custom section of an object, the information in the Workload Balancer is not filtered by the object.&nbsp;The Workload Balancer displays the information filtered by the originally applied filters.
