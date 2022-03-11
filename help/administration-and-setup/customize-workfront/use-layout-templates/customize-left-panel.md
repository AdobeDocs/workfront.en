---
filename: customize-left-panel
title: Customize the left panel using a Layout Template
user-type: administrator
product-area: system-administration;templates;setup
navigation-topic: layout-templates
title: Customize the left panel using a layout template
description: In a layout template, you can customize what users see in the left panel area throughout Adobe Workfront.
---

# Customize the left panel using a layout template

In a layout template, you can customize what users see in the left panel area throughout Adobe Workfront.

For example, you can determine which of the following items users see in the left panel when viewing a task:

![](assets/left-panel-adobe-branding-350x233.png)

>[!IMPORTANT]
>
>Changes made to order and visibility are reflected in the mobile app.

For information about layout templates for groups, see [Create and modify a group’s layout templates](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-layout-templates.md).

## Access requirements

You must have the following to perform the steps in this article:

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>You must be a Workfront administrator. For more information, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Grant a user full administrative access</a>.</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Customize the left panel for an area in Workfront:

<ol> 
 <li value="1">Begin working on a layout template, as described in <a href="../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md" class="MCXref xref">Create and manage layout templates</a>.</li> 
 <li value="2"> <p>Click the down arrow <img src="assets/dropdown-arrow.png"> under <span class="bold">Customize what users see</span>, then click the left panel you want to customize.</p> <note type="note">
   For information about the Home option in this drop-down list, see 
   <a href="../../../administration-and-setup/customize-workfront/use-layout-templates/customize-home-summary-layout-template.md" class="MCXref xref">Customize Home and Summary using a layout template</a>. For information about the Lists option, see 
   <a href="../../../administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md" class="MCXref xref">Customize Filters, Views, and Groupings using a layout template</a>.
  </note> </li> 
 <li value="3"> <p>In the <span class="bold">Left panel</span> list, do any of the following to determine what will users see in the left panel for the option (Workfront area or object type) you have selected:</p> 
  <ul> 
   <li>Show <img src="assets/add-secondary-nav-item.png"> or hide <img src="assets/delete-secondary-nav-item.png"> items. Any item without <img src="assets/add-secondary-nav-item.png"> or <img src="assets/delete-secondary-nav-item.png"> cannot be hidden.</li> 
   <li>Drag items <img src="assets/move-icon---dots.png"> to change their order on the left panel.</li> 
  </ul> 
  <table cellspacing="15"> 
   <col>  
   <col> 
   <thead> 
    <tr> 
     <th>Option</th> 
     <th>When users click the following...</th> 
     <th>They see the left panel items you choose from the following:</th> 
    </tr> 
   </thead> 
   <tbody> 
    <tr> 
     <td>Project</td> 
     <td>The name of a project</td> 
     <td>Tasks, Project Details, Business Case, Updates, Documents, Issues, Risks, Approvals, Baselines, Billing Rates, Billing Records, Expenses, Hours, Scheduling, People, Utilization, Queue Details, Routing Rules, Queue Topic, Topic Group, Metrics</td> 
    </tr> 
    <tr> 
     <td>Task</td> 
     <td>The name of a task</td> 
     <td> Updates, Documents, Task Details, Subtask, Issues, Hours, Approvals, Expenses, Predecessors</td> 
    </tr> 
    <tr> 
     <td>Issue</td> 
     <td>The name of an issue</td> 
     <td> Updates, Documents, Issue Details, Hours, Approvals</td> 
    </tr> 
    <tr> 
     <td>Portfolio</td> 
     <td>The name of a portfolio</td> 
     <td>Projects, Programs, Portfolio Details, Portfolio Optimization, Documents, Updates</td> 
    </tr> 
    <tr> 
     <td>Program</td> 
     <td>The name of a program</td> 
     <td>Projects, Program Details, Updates, Documents</td> 
    </tr> Template The name of a project template Template Tasks, Template Details, Updates, Documents, Risks, Expenses, People, Approvals, Billing Rates, Queue Details, Routing Rules, Queue Topic, Topic Group Template Task The name of a template task Updates, Documents, Template Task Details, Subtasks, Expenses, Approvals, Predecessors <!--
     Document Document Details (for a document uploaded to Workfront) Updates, Approvals, All Versions, Custom Forms
    --> Billing Record The name of a billing record for a project Billing Record Details, Billable Hours, Billable Expenses, Fixed Revenues Projects Projects in the Main menu Projects Requests The name of a request New Request, Submitted requests, All Requests, Drafts Dashboards The name of a dashboard My Dashboards, Shared Dashboards, All Dashboards Note: If you created custom tabs for the Reports area using a layout template in Adobe Workfront Classic, they display at the bottom of this list. For users, they display at the bottom of the left panel in the Dashboards area. Scrum Team The name of a Scrum team Iterations, Current iteration, Backlog, Schedule, Updates, Team Settings Kanban Team The name of a Kanban team Schedule, Kanban board, Backlog, Updates, Team Settings Waterfall Team The name of a Waterfall team Schedule, Updates, Team Requests, Team Settings Iteration The name of an iteration Stories, Issues, Story Board, Overview, Custom Forms, Updates <!--
     Company The name of the company People (cannot be hidden), Billing Rates, Custom Forms
    --> <!--
     Timesheets The name of the timesheet My Timesheets, Timesheets I Approve, All Timesheets (cannot be hidden)
    --> <!--
     Resourcing The name of the resource Planner (cannot be hidden), Scheduling, Utilization, Resource Pools
    --> <!--
     User Details ____________ Details (cannot be hidden), Org Chart, Time Off, Custom Forms
    --> 
   </tbody> 
  </table> <note type="note"> 
   <p>The last 3 items in the <span class="bold">Customize what users see</span> drop-down list (Lists, Home and Summary, and Branding) are for configuring areas other than the left panel. For information about them, see these articles:</p> 
   <ul> 
    <li><a href="../../../administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md" class="MCXref xref">Customize Filters, Views, and Groupings using a layout template</a> </li> 
    <li><a href="../../../administration-and-setup/customize-workfront/use-layout-templates/customize-home-summary-layout-template.md" class="MCXref xref">Customize Home and Summary using a layout template</a> </li> 
    <li><a href="../../../administration-and-setup/customize-workfront/use-layout-templates/brand-wf-using-a-layout-template.md" class="MCXref xref">Brand Adobe Workfront using a layout template</a> </li> 
   </ul> 
  </note> </li> 
 <li value="4"> <p>(Optional) If you want to add a left panel item that links to one of your organization's dashboards, click <span class="bold">Add custom section</span>, type a <span class="bold">Custom section title</span> for the item, then add the dashboard.</p> <p>Dashboard items appear at the bottom of the left panel. Users see the Custom section title you type next to the dashboard item when they hover over the left panel.</p> <note type="note">
   Users can add custom dashboard items to their own left panel. When you add custom dashboard items in a layout template, your items merge with theirs, without overwriting or resetting them. This is also true if you assign users to a new layout template with custom dashboard items. For information about how users can customize the left panel, see 
   <a href="../../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/create-custom-tabs.md" class="MCXref xref">Create custom tabs or sections</a>.
  </note> <p>For information about dashboards, see <a href="../../../reports-and-dashboards/dashboards/dashboards-overview.md" class="MCXref xref">Dashboards</a>.</p> </li> 
 <li value="5"> <p>Continue customizing the layout template.</p> <p>Or</p> <p>If you are finished customizing, click <span class="bold">Save</span>.</p> <note type="tip">
   You can 
   <span class="bold">Save</span> your progress at any time, then continue to modify the template later.
  </note> </li> 
</ol>

