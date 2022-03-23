---
filename: assignments-regardless-of-role-or-group-scheduling-areas
product-area: resource-management;user-management
navigation-topic: resource-scheduling
title: Allow user assignments regardless of role and group membership in the Scheduling areas
description: We are no longer developing the Resource Scheduling tools and they will soon be removed from Adobe Workfront. We recommend that you use the Workload Balancer for scheduling your resources.
---

# Allow user assignments regardless of role and group membership in the Scheduling areas

>[!NOTE]
>
>We are no longer developing the Resource Scheduling tools and they will soon be removed from Adobe Workfront. We recommend that you use the Workload Balancer for scheduling your resources. 
>
>For information about scheduling resources using the new Workload Balancer, see the section [The Workload Balancer](../../resource-mgmt/workload-balancer/workload-balancer.md).
>
>For more information about the timeline for removing the Resource Scheduling tools and replacing them with the Workload Balancer, see [Deprecation of Resource Scheduling tools in Adobe Workfront](../../resource-mgmt/resource-mgmt-overview/deprecate-resource-scheduling.md).

By default, assignments can be made only to users who have a role defined on their user profile that matches the role assignment of the task or issue that is being assigned to them.

You can configure Adobe Workfront to allow tasks and issues to be assigned to any user, regardless of whether that user has a role defined on their user profile that matches the role assignment of the task or issue that is being assigned to them. When you assign a user to a task or issue and that user does not have a role that matches the role assignment on the task or issue, the original role assignment is removed, and the role assignment changes to the role of the user you are assigning.

## Access requirements

You must have the following access to perform the steps in this article:

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Work or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level*</td> 
   <td> <p>View or higher access to&nbsp;Projects, Tasks, and Issues</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Contribute permissions or higher to the projects, tasks, and issues you update assignments for</p> <p>For information on requesting additional access, see <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects in Adobe Workfront</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your Workfront administrator.

## Allow assignments to users regardless of role

1. Go to the scheduling timeline for multiple projects, for an individual project, or for a team:

  * **For multiple projects**:&nbsp; Click the **Main Menu** icon ![](assets/main-menu-icon.png) in the upper-right corner of Workfront, click **Resourcing > Workload Balancer**, then select **Scheduling** in the upper-left drop-down menu. 
  * **For an individual project**:  Go to a project, click the **Workload Balancer** section in the left panel, then select **Scheduling** from the upper-left drop-down menu. 
  * **For a team**:  Click the **Main Menu** icon ![](assets/main-menu-icon.png) in the upper-right corner of Workfront, then click **Teams**, select a team, click**Workload Balancer** in the left panel, then select**Scheduling** from the upper-left drop-down menu.

1. Click the **Settings** icon on the scheduling timeline.
1. Disable the option **Limit Assignments to Users with Matching Role**.
1. Click **Return to Scheduling**.

## Allow assignments to users regardless of group membership

By default, assignments can be made only to users who are members of the group that is associated with the project (this is the group that is defined when editing the project).

>[!IMPORTANT]
>
>This setting takes into account only the members of the group associated with the project, and not any members of any subgroups of that group.

You can configure Workfront to allow tasks and issues to be assigned to any user, regardless of whether that user is a member of the group that is associated with the project where the task or issue resides.

1. Go to the scheduling timeline for multiple projects, for an individual project, or for a team:

  * **For multiple projects**:&nbsp; Click the **Main Menu** icon ![](assets/main-menu-icon.png) in the upper-right corner of Workfront, click **Resourcing > Workload Balancer**, then select **Scheduling** in the upper-left drop-down menu. 
  * **For an individual project**:  Go to a project, click the **Workload Balancer** section in the left panel, then select **Scheduling** from the upper-left drop-down menu. 
  * **For a team**:  Click the **Main Menu** icon ![](assets/main-menu-icon.png) in the upper-right corner of Workfront, then click **Teams**, select a team, click**Workload Balancer** in the left panel, then select**Scheduling** from the upper-left drop-down menu.

  *

1. Click the **Settings** icon on the scheduling timeline.
1. Disable the option **Limit Assignments to the Group Associated with the Project**.
1. Click **Return to Scheduling**.

&nbsp;
