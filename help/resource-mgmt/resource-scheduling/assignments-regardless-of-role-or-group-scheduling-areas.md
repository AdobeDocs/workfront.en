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
>We are no longer developing the Resource Scheduling tools and they will soon be removed from *Adobe Workfront*. We recommend that you use the *Workload Balancer* for scheduling your resources. 
>
>For information about scheduling resources using the new *Workload Balancer*, see the section [The Workload Balancer](../../resource-mgmt/workload-balancer/workload-balancer.md).
>
>For more information about the timeline for removing the Resource Scheduling tools and replacing them with the *Workload Balancer*, see [Deprecation of Resource Scheduling tools in Adobe Workfront](../../resource-mgmt/resource-mgmt-overview/deprecate-resource-scheduling.md).

By default, assignments can be made only to users who have a role defined on their user profile that matches the role assignment of the task or issue that is being assigned to them.

You can configure *Adobe Workfront* to allow tasks and issues to be assigned to any user, regardless of whether that user has a role defined on their user profile that matches the role assignment of the task or issue that is being assigned to them. When you assign a user to a task or issue and that user does not have a role that matches the role assignment on the task or issue, the original role assignment is removed, and the role assignment changes to the role of the user you are assigning.

## Access requirements

You must have the following access to perform the steps in this article:

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><em>Adobe Workfront</em> plan*</td> 
   <td> <p>Any </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><em>Adobe Workfront</em> license*</td> 
   <td> <p><em>Work</em> or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level*</td> 
   <td> <p>View or higher access to&nbsp;Projects, Tasks, and Issues</p> <p>Note: If you still don't have access, ask your <em>Workfront administrator</em> if they set additional restrictions in your access level. For information on how a <em>Workfront administrator</em> can change your access level, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Contribute permissions or higher to the projects, tasks, and issues you update assignments for</p> <p>For information on requesting additional access, see <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects in Adobe Workfront</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your *Workfront administrator*.

## Allow assignments to users regardless of role

<ol> 
 <li value="1">Go to the scheduling timeline for multiple projects, for an individual project, or for a team: 
  <ul>
   <li><p><b>For multiple projects</b>:&nbsp; <draft-comment>
      <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
       Click the 
       <span class="bold">Main Menu</span> icon 
       <img src="assets/main-menu-icon.png"> in the upper-right corner of 
       <em>Workfront</em>, click 
       <span class="bold">Resourcing > <em>Workload Balancer</em></span>, then select 
       <span class="bold">Scheduling</span> in the upper-left drop-down menu. 
      </MadCap:conditionalText>
     </draft-comment><MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
      Click the 
      <span class="bold">Main Menu</span> icon 
      <img src="assets/main-menu-icon.png"> in the upper-right corner of 
      <em>Workfront</em>, click 
      <span class="bold">Resourcing > <em>Workload Balancer</em></span>, then select 
      <span class="bold">Scheduling</span> in the upper-left drop-down menu. 
     </MadCap:conditionalText></p></li>
   <li><p><b>For an individual project</b>: <draft-comment>
      <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
        Go to a project, click the 
       <span class="bold"><em>Workload Balancer</em></span> section in the left panel, then select 
       <span class="bold">Scheduling</span> from the upper-left drop-down menu. 
      </MadCap:conditionalText>
     </draft-comment><MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
       Go to a project, click the 
      <span class="bold"><em>Workload Balancer</em></span> section in the left panel, then select 
      <span class="bold">Scheduling</span> from the upper-left drop-down menu. 
     </MadCap:conditionalText></p></li>
   <li><p><b>For a team</b>: <draft-comment>
      <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
        Click the 
       <span class="bold">Main Menu</span> icon 
       <img src="assets/main-menu-icon.png"> in the upper-right corner of 
       <em>Workfront</em>, then click 
       <span class="bold">Teams</span>, select a team, click
       <span class="bold"> <em>Workload Balancer</em></span> in the left panel, then select
       <span class="bold"> Scheduling</span> from the upper-left drop-down menu. 
      </MadCap:conditionalText>
     </draft-comment><MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
       Click the 
      <span class="bold">Main Menu</span> icon 
      <img src="assets/main-menu-icon.png"> in the upper-right corner of 
      <em>Workfront</em>, then click 
      <span class="bold">Teams</span>, select a team, click
      <span class="bold"> <em>Workload Balancer</em></span> in the left panel, then select
      <span class="bold"> Scheduling</span> from the upper-left drop-down menu. 
     </MadCap:conditionalText></p></li>
  </ul></li> 
 <li value="2">Click the <span class="bold">Settings</span> icon on the scheduling timeline.</li> 
 <li value="3">Disable the option <span class="bold">Limit Assignments to Users with Matching Role</span>.</li> 
 <li value="4">Click <span class="bold">Return to Scheduling</span>.</li> 
</ol>

## Allow assignments to users regardless of group membership

By default, assignments can be made only to users who are members of the group that is associated with the project (this is the group that is defined when editing the project).

>[!IMPORTANT]
>
>This setting takes into account only the members of the group associated with the project, and not any members of any subgroups of that group.

You can configure *Workfront* to allow tasks and issues to be assigned to any user, regardless of whether that user is a member of the group that is associated with the project where the task or issue resides.

<ol> 
 <li value="1">Go to the scheduling timeline for multiple projects, for an individual project, or for a team: 
  <ul>
   <li><p><b>For multiple projects</b>:&nbsp; <draft-comment>
      <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
       Click the 
       <span class="bold">Main Menu</span> icon 
       <img src="assets/main-menu-icon.png"> in the upper-right corner of 
       <em>Workfront</em>, click 
       <span class="bold">Resourcing > <em>Workload Balancer</em></span>, then select 
       <span class="bold">Scheduling</span> in the upper-left drop-down menu. 
      </MadCap:conditionalText>
     </draft-comment><MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
      Click the 
      <span class="bold">Main Menu</span> icon 
      <img src="assets/main-menu-icon.png"> in the upper-right corner of 
      <em>Workfront</em>, click 
      <span class="bold">Resourcing > <em>Workload Balancer</em></span>, then select 
      <span class="bold">Scheduling</span> in the upper-left drop-down menu. 
     </MadCap:conditionalText></p></li>
   <li><p><b>For an individual project</b>: <draft-comment>
      <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
        Go to a project, click the 
       <span class="bold"><em>Workload Balancer</em></span> section in the left panel, then select 
       <span class="bold">Scheduling</span> from the upper-left drop-down menu. 
      </MadCap:conditionalText>
     </draft-comment><MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
       Go to a project, click the 
      <span class="bold"><em>Workload Balancer</em></span> section in the left panel, then select 
      <span class="bold">Scheduling</span> from the upper-left drop-down menu. 
     </MadCap:conditionalText></p></li>
   <li><p><b>For a team</b>: <draft-comment>
      <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
        Click the 
       <span class="bold">Main Menu</span> icon 
       <img src="assets/main-menu-icon.png"> in the upper-right corner of 
       <em>Workfront</em>, then click 
       <span class="bold">Teams</span>, select a team, click
       <span class="bold"> <em>Workload Balancer</em></span> in the left panel, then select
       <span class="bold"> Scheduling</span> from the upper-left drop-down menu. 
      </MadCap:conditionalText>
     </draft-comment><MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
       Click the 
      <span class="bold">Main Menu</span> icon 
      <img src="assets/main-menu-icon.png"> in the upper-right corner of 
      <em>Workfront</em>, then click 
      <span class="bold">Teams</span>, select a team, click
      <span class="bold"> <em>Workload Balancer</em></span> in the left panel, then select
      <span class="bold"> Scheduling</span> from the upper-left drop-down menu. 
     </MadCap:conditionalText></p></li>
  </ul>
  <ul>
   <li><br></li>
  </ul></li> 
 <li value="2">Click the <span class="bold">Settings</span> icon on the scheduling timeline.</li> 
 <li value="3">Disable the option <span class="bold">Limit Assignments to the Group Associated with the Project</span>.</li> 
 <li value="4">Click <span class="bold">Return to Scheduling</span>.</li> 
</ol>

&nbsp;
