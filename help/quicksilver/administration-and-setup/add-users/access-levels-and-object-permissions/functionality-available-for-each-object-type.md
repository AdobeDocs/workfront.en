---
user-type: administrator
content-type: reference
product-area: system-administration
keywords: access,model,funnel,diagram,levels,permissions
navigation-topic: access-levels
title: Functionality Available for Each Object Type for Various Access Levels
description: The following tables lists the functionality available for each object type in the various access levels.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 91b1b448-5a0b-4e64-a59e-458c8387ecbc
---
# Functionality available for each object type for various access levels

{{highlighted-preview}}

The following tables lists the functionality available for each object type in the various access levels.

It also indicates which actions Workfront administrators can disable or enable using an access level.

>[!NOTE]
>
>This article describes functionality available to access levels in the current Workfront package model. To see functionality available in the new package model, see [Functionality available for each object type for new access levels](/help/quicksilver/administration-and-setup/add-users/how-access-levels-work/functionality-available-for-objects.md).

## Projects

Only users with a Plan license can be granted full access to projects. 

| Action |Planner |Worker |Reviewer |Requestor |External user |
|---|---|---|---|---|---|
| Create |✓&#42; |  |  |  |  |
| Copy |✓&#42; |  |  |  |  |
| Delete |✓&#42; |  |  |  |  |
| Share |✓&#42; |✓&#42; |  |  |  |
| Share system-wide |✓&#42; |  |  |  |  |
| View |✓&#42; |✓&#42; |✓&#42; |  |  |
| Add a custom form |✓ |  |  |  |  |
| Update custom fields |✓ |✓ |  |  |  |
| Add an approval process |✓ |  |  |  |  |
| Approve a project |✓ |✓ |✓ |  |  |
| Add document |✓ |✓ |✓ |  |  |
| Add issue |✓ |✓ |  |  |  |
| Add tasks |✓ |✓ |  |  |  |
| Give updates/comments |✓ |✓ |✓ |  |  |
| Change status |✓ |  |  |  |  |
| Log hours |✓ |✓ |  |  |  |
| Edit assignments |✓ |✓ |  |  |  |
| Manage a baseline |✓ |  |  |  |  |
| Manage risks |✓ |  |  |  |  |
| Manage finance |✓ |  |  |  |  |
| Add/edit expenses |✓ |✓ |  |  |  |
| Attach templates |✓ |  |  |  |  |
| Save as a template |✓ |  |  |  |  |
| Add/edit a business case |✓ |  |  |  |  |
| Edit project details |✓ |  |  |  |  |
| Edit staffing |✓ |  |  |  |  |
| Export to MS Project |✓ |✓ |✓ |  |  |
| Recalculate finance/timeline |✓ |  |  |  |  |
| Set queue properties |✓ |  |  |  |  |



&#42; Using an access level, Workfront administrators can disable or enable this functionality. For more information, see [Configurable access to functionality for each object type](../../../administration-and-setup/add-users/access-levels-and-object-permissions/configurable-functionality-in-each-access-level-by-object-type.md).

## Tasks

| Action |Planner |Worker |Reviewer |Requestor |External user |
|---|---|---|---|---|---|
| Create |✓&#42; |✓&#42; |  |  |  |
| Delete |✓&#42; |✓&#42; |  |  |  |
| Share |✓&#42; |✓&#42; |  |  |  |
| Share system-wide |✓&#42; |  |  |  |  |
| View |✓&#42; |✓&#42; |✓&#42; |✓&#42; |  |
| Add predecessors |✓ |✓ |  |  |  |
| Add issues |✓ |✓ |  |  |  |
| Edit a task (excluding status) |✓ |✓ |  |  |  |
| Change task status |✓ |✓ |  |  |  |
| Add documents |✓ |✓ |✓ |  |  |
| Copy a task |✓ |✓ |  |  |  |
| Move a task |✓ |✓ |  |  |  |
| Log hours |✓ |✓ |  |  |  |
| Accept an assignment |✓ |✓ |  |  |  |
| Make an assignment |✓ |✓ |Only in in-line edit |Only in in-line edit |  |
| Attach a custom form |✓ |✓ |  |  |  |
| Edit custom fields |✓ |✓ |  |  |  |
| Create an approval process |✓ |✓ |  |  |  |
| Approve a task |✓ |✓ |✓ |  |  |
| Edit finances |✓ |  |  |  |  |
| Add/edit expenses |✓ |✓ |  |  |  |
| View finance |✓ |✓ |✓ |  |  |
| Updates/comments |✓ |✓ |✓ |  |  |

{style="table-layout:auto"}

&#42; Using an access level, Workfront administrators can disable or enable this functionality. For more information, see [Configurable access to functionality for each object type](../../../administration-and-setup/add-users/access-levels-and-object-permissions/configurable-functionality-in-each-access-level-by-object-type.md).

## Issues

| Action |Planner |Worker |Reviewer |Requestor |External user |
|---|---|---|---|---|---|
| Create  |✓&#42; |✓&#42; |✓&#42; |✓&#42; |  |
| Edit |✓ |✓ |✓ |✓ |  |
| Delete |✓&#42; |✓&#42; |✓&#42; |✓&#42; |  |
| Share |✓&#42; |✓&#42; |✓&#42; |✓&#42; |  |
| Share system-wide  |✓&#42; |  |  |  |  |
| View |✓&#42; |✓&#42; |✓&#42; |✓&#42; |  |
| Attach custom forms |✓ |✓ |✓ |✓ |  |
| Edit custom fields |✓ |✓ |✓ |✓ |  |
| Approve issues |✓ |✓ |✓ |✓ |  |
| Add an approval process |✓ |✓ |✓ |✓ |  |
| Add documents |✓ |✓ |✓ |✓ |  |
| Copy issues |✓ |✓ |✓ |✓ |  |
| Move issues |✓ |✓ |✓ |✓ |  |
| Log hours |✓ |✓ |  |  |  |
| Convert an issue to a project |✓ |✓ |  |  |  |
| Convert an issue to a to task |✓ |  |  |  |  |
| Accept assignments |✓ |✓ |  |  |  |
| Make assignments |✓ |✓ |  |  |  |
| Add updates and comments |✓ |✓ |✓ |✓ |  |



&#42; Using an access level, Workfront administrators can disable or enable this functionality. For more information, see [Configurable access to functionality for each object type](../../../administration-and-setup/add-users/access-levels-and-object-permissions/configurable-functionality-in-each-access-level-by-object-type.md).

## Portfolios

Only users with a Plan license can have full access to portfolios. 

| Action |Planner |Worker |Reviewer |Requestor |External user |
|---|---|---|---|---|---|
| Create |✓&#42; |  |  |  |  |
| Delete |✓&#42; |  |  |  |  |
| Share |✓&#42; |  |  |  |  |
| Share system-wide |✓&#42; |  |  |  |  |
| View |✓&#42; |✓&#42; |✓&#42; |  |  |
| Edit details |✓ |  |  |  |  |
| Attach custom forms |✓ |  |  |  |  |
| Edit custom fields |✓ |  |  |  |  |
| Add and remove projects |✓ |  |  |  |  |
| Approve projects |✓ |  |  |  |  |
| Portfolio optimization |✓ |  |  |  |  |
| Add documents |✓ |✓ |✓ |  |  |
| Add updates and comments |✓ |✓ |✓ |  |  |



&#42; Using an access level, Workfront administrators can disable or enable this functionality. For more information, see [Configurable access to functionality for each object type](../../../administration-and-setup/add-users/access-levels-and-object-permissions/configurable-functionality-in-each-access-level-by-object-type.md).

## Programs

Only users with a Plan license can have full access to programs. 

| Action |Planner |Worker |Reviewer |Requestor |External user |
|---|---|---|---|---|---|
| Create |✓&#42; |  |  |  |  |
| Delete |✓&#42; |  |  |  |  |
| Share |✓&#42; |  |  |  |  |
| Share system-wide |✓&#42; |  |  |  |  |
| View |✓&#42; |✓&#42; |✓&#42; |  |  |
| Edit details |✓ |  |  |  |  |
| Attach custom forms |✓ |  |  |  |  |
| Edit custom fields |✓ |  |  |  |  |
| Add and remove projects |✓ |  |  |  |  |
| Approve projects |✓ |  |  |  |  |
| Portfolio Optimization |✓ |  |  |  |  |
| Add documents |✓ |✓ |✓ |  |  |
| Add Add updates and comments |✓ |✓ |✓ |  |  |



&#42; Using an access level, Workfront administrators can disable or enable this functionality. For more information, see [Configurable access to functionality for each object type](../../../administration-and-setup/add-users/access-levels-and-object-permissions/configurable-functionality-in-each-access-level-by-object-type.md).

## Reports, dashboards, and calendars

Users with a Plan license can have full access to reports. All other Access Levels have View access to reports.

| Action |Planner |Worker |Reviewer |Request |External user |
|---|---|---|---|---|---|
| Create |✓&#42; |  |  |  |  |
| Delete |✓&#42; |  |  |  |  |
| View built-in reports |✓&#42; |  |  |  |  |
| Share |✓&#42; |✓ |✓ |  |  |
| Share calendars and reports publicly |✓&#42; |  |  |  |  |
| Share system-wide |✓&#42; |  |  |  |  |
| View |✓&#42; |✓&#42; |✓&#42; |✓&#42; |✓&#42; |
| Edit |✓ |  |  |  |  |
| Copy |✓ |  |  |  |  |

{style="table-layout:auto"}

&#42; Using an access level, Workfront administrators can disable or enable this functionality. For more information, see [Configurable access to functionality for each object type](../../../administration-and-setup/add-users/access-levels-and-object-permissions/configurable-functionality-in-each-access-level-by-object-type.md).

>[!NOTE]
>
>Requestors can view only reports that have been shared with them

## Filters, views, and groupings

<table> 
 <col> 
 </col> 
 <col> 
 </col> 
 <col> 
 </col> 
 <col> 
 </col> 
 <col> 
 </col> 
 <col> 
 </col> 
 <thead> 
  <tr> 
   <th> <p>Action</p> </th> 
   <th> <p>Planner</p> </th> 
   <th> <p>Worker</p> </th> 
   <th> <p>Reviewer</p> </th> 
   <th> <p>Requestor</p> </th> 
   <th>External user<br></th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Create</td> 
   <td>✓*</td> 
   <td>✓*</td> 
   <td>✓*</td> 
   <td>✓*</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Delete</td> 
   <td>✓*</td> 
   <td>✓*</td> 
   <td>✓*</td> 
   <td>✓*</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Share</td> 
   <td>✓*</td> 
   <td>✓*</td> 
   <td>✓*</td> 
   <td>✓*</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Share system-wide</td> 
   <td>✓*</td> 
   <td>✓*</td> 
   <td>✓*</td> 
   <td>✓*</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>View</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Edit</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>

&#42; Using an access level, Workfront administrators can disable or enable this functionality. For more information, see [Configurable access to functionality for each object type](../../../administration-and-setup/add-users/access-levels-and-object-permissions/configurable-functionality-in-each-access-level-by-object-type.md).

## Documents

| Action |Planner |Worker |Reviewer |Requestor |External user |
|---|---|---|---|---|---|
| Create |✓&#42; |✓&#42; |✓&#42; |✓&#42; |  |
| Delete (documents and folders) |✓&#42; |✓&#42; |✓&#42; |✓&#42; |  |
| Share |✓&#42; |✓&#42; |✓&#42; |✓&#42; |  |
| Share publicly (externally) |✓&#42; |  |  |  |  |
| Share system-wide |✓&#42; |✓&#42; |  |  |  |
| View |✓&#42; |✓&#42; |✓&#42; |✓&#42; |✓&#42; |
| Edit details |✓ |✓ |✓ |✓ |  |
| Download |✓ |✓ |✓ |✓ |✓ |
| Checkout |✓ |✓ |✓ |✓ |  |
| Add approvers |✓ |✓ |✓ |✓ |  |
| Approve documents |✓ |✓ |✓ |✓ |✓ |
| Attach custom forms |✓ |✓ |✓ |✓ |  |
| Edit custom fields |✓ |✓ |✓ |✓ |  |
| Move to (object) |✓ |✓ |✓ |✓ |  |
| Send to (integration) |✓ |✓ |✓ |✓ |  |
| Add updates and comments |✓ |✓ |✓ |✓ |  |
| Upload new version |✓ |✓ |✓ |✓ |  |
| Delete a version |✓ |✓ |✓ |✓ |  |
| Preview |✓ |✓ |✓ |✓ |✓ |
| Proof |✓ |✓ |✓ |✓ |  |
| Generate proof |✓ |✓ |  |  |  |
| Remove proof |✓ |✓ |✓ |✓ |  |
| Add/Remove&#42;&#42; |✓ |✓ |✓ |✓ |  |
| Rename&#42;&#42; |✓ |✓ |✓ |✓ |  |
| Link (with integration) |✓ |✓ |✓ |✓ |  |
| Unlink (with integration) |✓ |✓ |✓ |✓ |  |

{style="table-layout:auto"}

&#42; Using an access level, Workfront administrators can disable or enable this functionality. For more information, see [Configurable access to functionality for each object type](../../../administration-and-setup/add-users/access-levels-and-object-permissions/configurable-functionality-in-each-access-level-by-object-type.md).

&#42;&#42;Available only for document folders, not documents

## Users

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <col> 
 </col> 
 <col> 
 </col> 
 <col> 
 </col> 
 <col> 
 </col> 
 <thead> 
  <tr> 
   <th> <p>Action</p> </th> 
   <th> <p>Planner</p> </th> 
   <th>Worker</th> 
   <th> <p>Reviewer</p> </th> 
   <th> <p>Requestor</p> </th> 
   <th> <p>External user**</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Create</td> 
   <td>✓*</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Delete</td> 
   <td>✓*</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Edit, delete, deactivate, log in as, or reset the password for any user</td> 
   <td>✓*<p><b>NOTE</b>: You can not log in as any user that is a system administrator.</p></td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Edit, delete, deactivate, log in as, or reset the password for any user in a group they administer</td> 
   <td>✓*<p><b>NOTE</b>: You can not log in as any user that is a system administrator.</p></td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>View users</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>View contact info</td> 
   <td>✓</td> 
   <td> ✓</td> 
   <td>✓ </td> 
   <td> ✓</td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>

&#42; Using an access level, Workfront administrators can disable or enable this functionality. For more information, see [Configurable access to functionality for each object type](../../../administration-and-setup/add-users/access-levels-and-object-permissions/configurable-functionality-in-each-access-level-by-object-type.md).

&#42;&#42;External users can only search for other users

## Teams

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p>Action</p> </th> 
   <th> <p>Planner</p> </th> 
   <th>Worker</th> 
   <th> <p>Reviewer</p> </th> 
   <th> <p>Requestor</p> </th> 
   <th> <p>External user*</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Create</td> 
   <td>✓*</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Delete</td> 
   <td>✓*</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Edit teams they're on</td> 
   <td>✓*</td> 
   <td>✓*</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Edit teams in groups they manage</td> 
   <td>✓*</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>View all teams</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>View teams associated with their groups</td> 
   <td>✓</td> 
   <td> ✓</td> 
   <td>✓ </td> 
   <td> ✓</td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>

&#42; Using an access level, Workfront administrators can disable or enable this functionality. For more information, see [Configurable access to functionality for each object type](../../../administration-and-setup/add-users/access-levels-and-object-permissions/configurable-functionality-in-each-access-level-by-object-type.md).

## Templates

| Action |Planner |Worker |Reviewer |Requestor |External user |
|---|---|---|---|---|---|
| Create |✓&#42; |  |  |  |  |
| Delete |✓&#42; |  |  |  |  |
| Share |✓&#42; |  |  |  |  |
| Share system-wide |✓&#42; |  |  |  |  |
| View |✓&#42; |  |  |  |  |
| Copy |✓ |  |  |  |  |
| Edit template details |✓ |  |  |  |  |

{style="table-layout:auto"}

&#42; Using an access level, Workfront administrators can disable or enable this functionality. For more information, see [Configurable access to functionality for each object type](../../../administration-and-setup/add-users/access-levels-and-object-permissions/configurable-functionality-in-each-access-level-by-object-type.md).

## Financial data

Only users with a Plan license can have full access to financial data.

The Request and External User license types are not included here because they don't have access to these objects and areas.

| Action |Planner |Worker |Reviewer |
|---|---|---|---|
| Edit role billing and cost rates |✓&#42; |  |  |
| Edit user billing and cost rates |✓&#42; |  |  |
| View role billing and cost rates |✓&#42; |  |  |
| View user billing and cost rates |✓&#42; |  |  |
| Manage billing records |✓ |  |  |
| Manage expenses |✓ |✓ |  |
| View financial data |✓&#42; |✓&#42; |✓&#42; |
| <span class="preview">Manage rate cards</span>  |✓ |  |  |
| View information by Cost in the Resource Planning tools  |✓ |  |  |
| Budget Resources in the Resource Planning tools&#42;&#42; |✓ |  |  |
| View resource allocation in the Resource Planning tools&#42; |✓ |✓ |✓ |
| Create risks on projects |✓ |  |  |
| View risks on projects |✓ |✓ |✓ |

{style="table-layout:auto"}

&#42; Using an access level, Workfront administrators can disable or enable this functionality. For more information, see [Configurable access to functionality for each object type](../../../administration-and-setup/add-users/access-levels-and-object-permissions/configurable-functionality-in-each-access-level-by-object-type.md).

&#42;&#42;Requires additional access to Resource Management.

## Resource Management

Only users with a Plan license can have full access to [select object or area]. Other license types can have limited or no access to Resource Management in Workfront.

| Action |Planner |Worker |Reviewer |Requestor |External user |
|---|---|---|---|---|---|
| Edit priorities and budget hours in the Planner |✓&#42; |  |  |  |  |
| Create, edit, delete Resource Pools&#42;&#42; |✓&#42; |  |  |  |  |
| Update Planned Hours in the Workload Balancer&#42;&#42;&#42; | ✓*  |  |  |  |  |
| View project priorities in the Resource Planner | ✓&#42; |  |  |  |  |
| View resource allocation in the Resource Planning tools | ✓&#42; |✓&#42; |✓&#42; |  |  |
| View Resource Pools | ✓&#42; |✓&#42; |✓&#42; |  |  |
| Budget resources in the Resource Planning tools&#42;&#42; |✓ |  |  |  |  |
| Attach Resource Pools to projects, templates, and users |✓ |  |  |  |  |

{style="table-layout:auto"}

&#42; Using an access level, Workfront administrators can disable or enable this functionality. For more information, see [Configurable access to functionality for each object type](../../../administration-and-setup/add-users/access-levels-and-object-permissions/configurable-functionality-in-each-access-level-by-object-type.md).

&#42;&#42;Requires additional access to Financial Data and permissions to project finances. If you grant Resource Management access to a Planner user who doesn't have access to Financial Data, the user can still see the hourly allocations in the Resource Planner, but can't switch to Cost view or view the Business Case. For more information, see [Grant access to financial data](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md) and [Share financial permissions on an object](../../../workfront-basics/grant-and-request-access-to-objects/share-financial-permissions-object.md).

&#42;&#42;&#42;Requires permission to Contribute to the object, with Make Assignments enabled under Advanced Settings. For information, see the section [Understand inherited permissions and the hierarchy of objects](../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md#sharing-an-object) in the article [Overview of sharing permissions on objects](../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

## Scenario Planner area

| Action |Planner |Worker |Reviewer |Requestor |External user |
|---|---|---|---|---|---|
| Create/edit existing plans and initiatives | ✓ |✓ |✓ |  |  |
| Add or edit job role information on plans and initiatives&#42; |✓ |✓ |✓ |  |  |
| Add or edit cost information on plans and initiatives&#42; |✓ |✓ |✓ |  |  |
| Delete plans and initiatives | ✓ |✓ |✓ |  |  |
| View Scenarios in the Main Menu ![Scenario planner icon](assets/esp-icon-in-main-menu.png)| ✓ |✓ |✓ | |  |
| View plans and initiatives that the user created&#42; |✓ |✓ |✓ |  |  |

{style="table-layout:auto"}

>[!NOTE]
>
>Users can view a plan that another user created only if a link to the plan is shared with them.

&#42; In order for users to view financial data in a plan or initiative, they need access to Financial Data. For more information, see [Grant access to financial data](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).

## Workfront Goals area

| Actions |View |Edit |
|---|---|---|
| Create |  |✓ |
| Edit / delete all goals |  |✓ |
| View Goals in the Main menu |✓ |✓ |
| View the Goals area from a shared link |✓ |✓ |
| View all goals in the system |✓ |✓  |
| Activate/ deactivate/ close all goals |  |✓ |
| Create/ edit/ delete activities |  |✓ |
| Create/ edit/ delete results |  |✓ |
| Add an aligned goal |  |✓ |
| Update progress on a result or activity |  |✓ |
| Own a goal, result, or activity |✓ |✓ |
| Comment on a goal |✓ |✓ |
| Copy goals |  |✓ |
| View the Goal List section in the left panel |✓ |✓ |
| View the Graphs section in the left panel |✓ |✓ |
| View the Goal Alignment section in the left panel |✓ |✓ |


