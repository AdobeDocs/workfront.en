---
product-area: resource-management
keywords: working,team,staffing,resources
navigation-topic: the-workload-balancer
title: Locate the Workload Balancer
description: The Workload Balancer is available for multiple projects in the Resourcing area, for a team, for a project, and for a user.
author: Lisa
feature: Resource Management
exl-id: 88029c9d-b588-4d33-801a-04f49b12a6e8
---
# Locate the Workload Balancer

{{preview-fast-release-general}}

You can use the Workload Balancer to schedule resources for work or review their availability and current allocations.

You can access the Workload Balancer in the following ways:

* From several areas predefined by Adobe Workfront
* By adding it to a custom section

This article describes the areas where you can access the Workload Balancer.

>[!NOTE]
>
>Regardless of the method you use to access the Workload Balancer, navigating it, and managing resources is identical.
>
>For information about the Workload Balancer and how to use it for managing and scheduling your resources for work, see the following articles:
>
>* [Workload Balancer overview](../../resource-mgmt/workload-balancer/overview-workload-balancer.md)
>* [Navigate the Workload Balancer](../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md) 
>* [Overview of assigning work in the Workload Balancer](../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer.md)
>* [Manage user allocations in the Workload Balancer](../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md)

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
       Work, when using the Workload Balancer of a team or project</p>
       <p><span class="preview">Note: All users can access the Workload Balancer in their own user profiles, without any license requirements.</span></p></td>
  </tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>View or higher access to the following:</p> 
    <ul> 
     <li>Resource Management</li> 
     <li>Projects</li> 
     <li>Tasks</li> 
     <li>Issues</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td>View permissions or higher to the projects, tasks, and issues</td> 
  </tr> 
 </tbody> 
</table>

For more detail about the information in this table, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Access the Workload Balancer in predefined areas

The following sections illustrate where you can access the Workload Balancer within Workfront.

### Access the Workload Balancer for multiple projects in the Resourcing area

{{step1-to-resourcing}}

1. Click **Workload Balancer** in the left panel.
  
    ![Workload Balancer](assets/nwe-balancer-global.png)

    The Workload Balancer displays the following by information in the Resourcing area, by default:

    * **Unassigned Work**: No unassigned work items.
    * **Assigned Work**: All active users in the system.

      We recommend using filters when displaying users in the Assigned Work area. For more information, see [Filter information in the Workload Balancer](../workload-balancer/filter-information-workload-balancer.md). 

### Access the Workload Balancer for a team

For more information on teams in Workfront, see [Teams overview](/help/quicksilver/people-teams-and-groups/create-and-manage-teams/teams-overview.md).

{{step1-to-team}}

   Your Home Team's page displays. 
  
1. Click **Workload Balancer** in the left panel.

   ![Workload Balancer for team](assets/nwe-balancer-team-350x172.png)

   The Workload Balancer of a team displays the following information, by default:

   * **Unassigned Work**: Items assigned to the team and not assigned to users. 
   * **Assigned Work**: All members of the team with all their assignments. 
  
     >[!TIP]
     >
     >Team members might be assigned to work also assigned to the team or to work assigned to other teams or roles.

### Access the Workload Balancer for a project
  
{{step1-to-projects}}

1. Click the name of a project to open the project page.
1. Click **Workload Balancer** in the left panel.

   The Workload Balancer for the project displays.

   ![Workload Balancer for Project](assets/nwe-balancer-project-350x152.png)

   The Workload Balancer of a project displays the following by information, by default:

   * **Unassigned Work**: Items from the project that are assigned to job roles or teams and are not assigned to users.
   * **Assigned Work**: Users assigned to items on the project.

     >[!TIP]
     >
     >You can display all users in the system instead of only the ones on the project (in the Assigned Work area) by enabling the Show all users option. For information, see [Navigate the Workload Balancer](../workload-balancer/navigate-the-workload-balancer.md).

<div class="preview">

### Access the Workload Balancer for a user

All users have access to view the Workload Balancer on their own profiles. If you have access to the Resourcing area in Adobe Workfront, you can also view the Workload Balancer on all user profiles. For more information, see [Access needed to manage resources in the Workload Balancer](/help/quicksilver/resource-mgmt/workload-balancer/access-needed-manage-resources-balancer.md).

Workload Balancer data for a user is read-only. You can't assign work, unassign work, or adjust allocations at the user level.

All of the display settings are available for the Workload Balancer for a user. For more information, see [Navigate the Workload Balancer](/help/quicksilver/resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

1. Access the user profile.

   For your own profile: {{step1-click-profile-pic}}

   For another user's profile: Click the linked name of the user as it appears anywhere in the Workfront interface. User names are displayed in many areas, such as in a comment made by the user.

1. Click **Workload Balancer** in the left panel.

   The Workload Balancer for the user displays.

   ![Workload Balancer for a user](assets/workload-balancer-user.png)

   The Workload Balancer of a user displays the following by information, by default:

     * **Assigned Work**: The tasks and issues assigned to the specific user.

</div>

## Add the Workload Balancer to a custom section

You can add the Workload Balancer to any custom section.

Most customizations that you have already applied to the Workload Balancer are preserved when adding it to a custom section.

1. Access the Workload Balancer by going to any of the following areas:

   * The Resourcing area
   * A team
   * A project

1. Obtain a shareable link and copy it to your clipboard as described in [Share the Workload Balancer with a link](../../resource-mgmt/workload-balancer/share-link-for-workload-balancer.md).
1. Create a dashboard with an external page as described in [Embed an external web page in a dashboard](../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/embed-external-web-page-dashboard.md). Use the shareable link you obtained in Step 2 for the external page. 

   <!--
      (NOTE: ensure this stays correct)
      -->

1. Create a custom section as described in [Create custom tabs or sections](../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/create-custom-tabs.md) to place the dashboard on the custom tab.

   When accessing the Workload Balancer from the custom section, you can view it as if you were accessing it directly from one of its original areas listed in Step 1. 

   <!--
      (NOTE: ensure this stays correct)
     -->

1. (Optional) Share the custom tab in a Layout Template as described in  [Customize the left panel using a layout template](../../administration-and-setup/customize-workfront/use-layout-templates/customize-left-panel.md) .


<!--
For a team:

* From the Workload Balancer section of a team.

  You can adjust allocations and review or assign work from multiple projects to individual team members.

For a project:

  You can do the following when you use the Workload Balancer within a project:

   * Assign work on the project to users already assigned other work on the project.
   * Assign work to any user that might not be on the project.

   * View additional work that users are assigned to on other projects.
   * Adjust user allocations to work items.-->
