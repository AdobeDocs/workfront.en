---
filename: assignments-regardless-of-role-or-group-scheduling-areas
product-area: resource-management;user-management
navigation-topic: resource-scheduling
title: Allow user assignments regardless of role and group membership in the Scheduling areas
description: We are no longer developing the Resource Scheduling tools and they will soon be removed from Adobe Workfront. We recommend that you use the Workload Balancer for scheduling your resources.
---

# Allow user assignments regardless of role and group membership in the Scheduling areas

>[!IMPORTANT]
>
>You're currently viewing the Adobe Workfront Classic version of this document. Adobe Workfront Classic is no longer supported. All Adobe Workfront Classic functionality, along with this documentation, will be removed in July 2022. Please transition to the the new Adobe Workfront experienceas soon as possible, and switch to the new Adobe Workfront experience version of this document.

>[!NOTE]
>
>We are no longer developing the Resource Scheduling tools and they will soon be removed from Adobe Workfront. We recommend that you use the Workload Balancer for scheduling your resources. 
>
>For information about scheduling resources using the new Workload Balancer, see the section [The Workload Balancer](../../resource-mgmt/workload-balancer/workload-balancer.md).
>
>For more information about the timeline for removing the Resource Scheduling tools and replacing them with the Workload Balancer, see [Deprecation of Resource Scheduling tools in Adobe Workfront](../../resource-mgmt/resource-mgmt-overview/deprecate-resource-scheduling.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(NOTE:&nbsp;***LINKED TO THE UI FROM Resource Scheduling (People> Teams>Working On>Settings>Limit Assignments to the Group Associated with the Project) - ALSO FROM THE WORKING ON TAB OF TEAMS and AT THE PROJECT STAFFING TAB TOO)</p>
<p>NOTE: Alina; broken off the original article; retitle, reformat, relink sections) </p>
</div>
-->

By default, assignments can be made only to users who have a role defined on their user profile that matches the role assignment of the task or issue that is being assigned to them.

You can configure Adobe Workfront to allow tasks and issues to be assigned to any user, regardless of whether that user has a role defined on their user profile that matches the role assignment of the task or issue that is being assigned to them. When you assign a user to a task or issue and that user does not have a role that matches the role assignment on the task or issue, the original role assignment is removed, and the role assignment changes to the role of the user you are assigning.

## Access requirements

You must have the following access to perform the steps in this article:

<table> 
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
   <td> <p>Contribute permissions or higher to the projects, tasks, and issues you update assignments for</p> <p>For information on requesting additional access, see <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your Workfront administrator.

## Allow assignments to users regardless of role

![](assets/resource-scheduling-schedulingtab-350x282.png)

1. Go to the scheduling timeline for multiple projects, for an individual project, or for a team:

   * **For multiple projects**:&nbsp; Click **People** in the Global Navigation Bar, click the **Workload Balancer** tab, then click **Switch back to Scheduling**.  
   * **For an individual project**:  Go to a project, then click the **Staffing** tab (the Staffing tab might be located under the **More** menu), then ensure that the **Scheduling** tab is selected and click **Switch back to Scheduling**. 
   * **For a team**:  Click **People** in the Global Navigation Bar, click the **Teams** tab, select the team from the drop-down menu, then click the **Working On** subtab and click **Switch back to Scheduling**.

1. Click the **Settings** icon on the scheduling timeline.
1. Disable the option **Limit Assignments to Users with Matching Role**.
1. Click **Return to Scheduling**.

## Allow assignments to users regardless of group membership

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Alina: **^ This section is linked to the UI in a tooltip inside the Settings of the scheduler. do not rename/ remove/ edit the tag!!) </p>
-->

By default, assignments can be made only to users who are members of the group that is associated with the project (this is the group that is defined when editing the project).

>[!IMPORTANT]
>
>This setting takes into account only the members of the group associated with the project, and not any members of any subgroups of that group.

You can configure Workfront to allow tasks and issues to be assigned to any user, regardless of whether that user is a member of the group that is associated with the project where the task or issue resides.

![](assets/resource-scheduling-schedulingtab-350x282.png)

1. Go to the scheduling timeline for multiple projects, for an individual project, or for a team:

   * **For multiple projects**:&nbsp; Click **People** in the Global Navigation Bar, click the **Workload Balancer** tab, then click **Switch back to Scheduling**.  
   * **For an individual project**:  Go to a project, then click the **Staffing** tab (the Staffing tab might be located under the **More** menu), then ensure that the **Scheduling** tab is selected and click **Switch back to Scheduling**. 
   * **For a team**:  Click **People** in the Global Navigation Bar, click the **Teams** tab, select the team from the drop-down menu, then click the **Working On** subtab and click **Switch back to Scheduling**.

1. Click the **Settings** icon on the scheduling timeline.
1. Disable the option **Limit Assignments to the Group Associated with the Project**.
1. Click **Return to Scheduling**.

&nbsp;
