---
filename: deactivate-job-roles
user-type: administrator
product-area: system-administration;user-management
navigation-topic: organization-setup
title: Deactivate job roles
description: As an Adobe Workfront administrator or a user with administrative access to Job Roles, you can deactivate job roles that become obsolete in your system. When you deactivate a job role instead of deleting it, you can keep any historical information that is associated with it.
---

# Deactivate job roles

As an  `Adobe Workfront administrator` or a user with administrative access to Job&nbsp;Roles, you can deactivate job roles that become obsolete in your system. When you deactivate a job role instead of deleting it, you can keep any historical information that is associated with it.

You can also reactivate job roles that have previously been deactivated.

## Access requirements

You must have the following:

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><span>Adobe Workfront</span> plan*</td> 
   <td> <p>Any </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><span>Adobe Workfront</span> license*</td> 
   <td> <p><span>Plan</span> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Administrative access to Job roles</p> <p>Note: If you still don't have access, ask your <span>Workfront administrator</span> if they set additional restrictions in your access level. For information on how a <span>Workfront administrator</span> can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your `Workfront administrator`.

## The impact of deactivating job roles

If you deactivate a job role, it no longer displays in the following areas:

<ul> 
 <li> <p>The Assignments typeahead field (for tasks, template tasks, issues, approvals, and routing rules)</p> </li> 
 <li> <p>The Assignments fields in lists and reports</p> </li> 
 <li> <p>User profiles</p> <note type="note">
   When you add a new role to a user, a deactivated job role doesn't display. But it does continue to display in the Primary Role and Other Roles fields if the user was associated with the job role before it was deactivated.
  </note> </li> 
 <li> <p>The Sharing dialog box for objects, including layout template assignment</p> </li> 
 <li> <p>Typeahead fields in custom forms</p> </li> 
 <li> <p>The Pool Members field in&nbsp;Resource Pools</p> </li> 
 <li> <p>The Job&nbsp;Role field of a Billing Rate edit screen when a user is overriding billing rates for projects</p> </li> 
 <li> <p>The Add assignment to Kanban board dialog box in a project</p> </li> 
 <li> <p>The Job&nbsp;Role field of a plan or an initiative when someone is using the <span>Adobe Workfront Scenario Planner</span>. </p> <p>This is available only in <span>the new Adobe Workfront experience</span> and requires an additional license. For information about the <span>Workfront Scenario Planner</span>, see <a href="../../../scenario-planner/scenario-planner-overview.md" class="MCXref xref">The Adobe Workfront Scenario Planner overview</a>. </p> </li> 
</ul>

>[!TIP]
>
>Deactivated roles always display in filters in lists, reports, and other tools such as the `Workload Balancer`.

## Considerations before deactivating a job role

It is better to deactivate rather than delete job roles that become obsolete so that you can keep all the historical information associated with roles you may have used in the past.

>[!NOTE]
>
>Any work assigned to the job role prior to deactivation remains assigned.

We recommend that you do the following before deactivating an unused job role:

<ul> 
 <li> <p>Build reports for any objects that are assigned to the role you plan to deactivate and reassign them to an active job role. For information about building reports, see <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-report.md" class="MCXref xref">Create a report</a>. </p> <note type="tip">
   You can create a report to filter for any tasks or issues where the deactivated role is assigned. Then use the report to reassign outstanding tasks or issues to an active role. 
  </note> </li> 
 <li> <p>Take an inventory of all approval processes, current approval paths, and routing rules or other objects that are assigned to the job role you plan to deactivate and reassign them to an active role.</p> <note type="tip">
   When using request queues, if you deactivate a job role assigned as the default assignee in a routing rule, the role remains and requests are still routed to the deactivated role. We recommend updating routing rules with active roles before you deactivate the team. 
  </note> <p>For information about creating approval processes and routing rules, see the following articles:</p> 
  <ul> 
   <li> <p><a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md" class="MCXref xref">Create an approval process for work items</a> </p> </li> 
   <li> <p><a href="../../../manage-work/requests/create-and-manage-request-queues/create-routing-rules.md" class="MCXref xref">Create Routing Rules</a> </p> </li> 
  </ul> </li> 
</ul>

## Deactivate a job role

1. In the left panel, click `Job Roles.`
1. (Optional) In the `Filter` drop-down menu, select `Active` to display only active job roles. 
1. Click the name of the job role that you want to deactivate.
1. In the `Is Active` drop-down menu, select `No`. 
1. Click `Save Changes`.

   The job role is deactivated and can no longer be assigned to work, associated with layout templates, and so on. For information about all uses of job roles in  `Workfront`, see [Job role overview](../../../administration-and-setup/set-up-workfront/organizational-setup/job-role-overview.md).

