---
filename: prioritize-projects-resource-planner
product-area: resource-management;projects
navigation-topic: resource-planning
title: Prioritize projects in the Resource Planner
description: Projects are listed in order of priority in the Resource Planner with the most important project at the top.
---

# Prioritize projects in the *Resource Planner*

Projects are listed in order of priority in the *Resource Planner* with the most important project at the top.

## Access requirements

You must have the following:

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><em>Adobe Workfront</em> plan*</td> 
   <td> <p><em>Pro</em> and higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><em>Adobe Workfront</em> license*</td> 
   <td> <p><em>Plan</em> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to&nbsp;Resource Management that includes access to&nbsp;Edit priorities and budget hours in the <em>Resource Planner</em></p> <p>Edit access to Financial Data, Projects, and Users</p> <p>Note: If you still don't have access, ask your <em>Workfront administrator</em> if they set additional restrictions in your access level. For information on how a <em>Workfront administrator</em> can change your access level, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to the projects you want to budget information for with ability to Manage Finances</p> <p>For information on requesting additional access, see <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects in Adobe Workfront</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your *Workfront administrator*.

## Default order of projects in the *Resource Planner*

By default, the projects are listed in the Project View of the *Resource Planner* by taking into consideration the criteria below.

>[!IMPORTANT]
>
>Projects are listed according to the three criteria below only the first time you open the *Resource Planner*. However, this default priority automatically becomes your custom priority and cannot be reverted to the original priority any time you do one of the following:
>
>* When you click Save at any time.
>* When you manually change the project planning priority. For information about changing the project planning priority manually, see the section [Manually change the Project Planning Priority](#project-planning-priority-subsection) in this article.
>
>After the project priority becomes your custom priority, any changes in the project information no longer affect the ordering of the projects using these criteria. After this, you can prioritize projects only manually.

The original default criteria for listing the projects in the Project View are as follows, in this order:

1. By the Alignment Score on the project.   
   For more information about the Alignment Score of the project, see [Apply a scorecard to a project and generate an Alignment Score](../../manage-work/projects/define-a-business-case/apply-scorecard-to-project-to-generate-alignment-score.md) .

1. By the Planned Start Date of the project (if the Alignment field is null or is the same for several projects). 
1. Alphabetically (if the Alignment field is null or is the same, and the Planned Start date is the same for several projects).

Consider the following when working with project priorities in the *Resource Planner*:

* You can manually customize the project priority only when you apply the Project View. This also changes the order of the projects in the *Resource Planner*.
* When you apply the Role or User Views in the *Resource Planner*, the projects appear in the same order of priority established in the Project View.
* The order of the projects in the *Resource Planner* is unique to you. Other users can view the same projects in the *Resource Planner*, but in a different order. You cannot report on the Project Planning Priority field. This is visible just in the *Resource Planner* and it serves as a flag for prioritizing your projects.

Projects associated with a portfolio might have a portfolio-level priority. You can enable viewing the portfolio priority of a project in the *Resource Planner*, in addition to the *Resource Planner* priority. You can also order the projects according to their portfolio priority. 

## Manually change the Project Planning Priority

You must have Edit access to Resource Management and Manage permissions to projects, to reorder projects in the *Resource Planner*.

By giving projects a new priority, you can rank them in order of importance.

To edit the Project Planning Priority:

<ol>
 <li value="1"> Go to the <span class="bold"><em>Resource Planner</em></span>.<br></li>
 <li value="2"><p> Click inside the field to the left of the project name which contains a number, and enter a number to change Planning Priority, then press Enter.<br><img src="assets/mceclip4.png"><br>Or<br>Hover over the name of the project and click the indicator to the left of the project name, and drag it and drop it in the correct spot, to change the priority. </p><p><img src="assets/drag-and-drop-projects-rp--1--350x184.png" alt="drag_and_drop_projects_RP__1_.png" style="width: 350;height: 184;"></p><p>When you select numbers to prioritize projects, select lower numbers for higher (more important) priorities, and higher numbers for lower (less important) priorities. When you change the priority number of a project to a lower number (higher priority), all other projects in the <em>Resource Planner</em> shift down on the list (become less important).<br>When you change the priority number of a project to a higher number (lower priority), all other projects in the <em>Resource Planner</em> shift up on the list (become more important).</p></li>
 <li value="3">Click <span class="bold">Save</span>.<br>The order of the projects changes according to your selections and this becomes your custom project priority in the <em>Resource Planner</em>. Other users cannot see your order of priority for the projects in the <em>Resource Planner</em>, although they might be able to view the same projects in their <em>Resource Planner</em>s. </li>
</ol>

## Order projects according to their Portfolio Priority in the *Resource Planner*

>[!IMPORTANT]
>
>Your company must have a *Business* or higher *Workfront* plan to prioritize projects in the Portfolio Optimizer. 
>
>For more information on the *Workfront* plans, see [Our Plans](https://www.workfront.com/plans). 
>
>For information about prioritizing projects in the Portfolio Optimizer, see [Prioritize projects in the Portfolio Optimizer](../../manage-work/portfolios/portfolio-optimizer/prioritize-projects-in-portfolio-optimizer.md).

<ol>
 <li value="1"><p>Open the <span class="bold"><em>Resource Planner</em></span> in the <span class="bold">Project View</span>.</p></li>
 <li value="2">Click the <span class="bold">Settings</span> icon.</li>
 <li value="3"><p>Enable the <span class="bold">Display Portfolio Priorities</span> setting to display the project priorities according to the Portfolio they are assigned to. The priority of the projects according to their portfolios displays next to the <em>Resource Planner</em> priority. This setting is disabled by default.</p><p><img src="assets/rp-portfolio-priority-unordered-(1)-350x203.png" style="width: 350;height: 203;"></p><p>The portfolio priorities of the projects display only in the Project view of the <em>Resource Planner</em>.</p></li>
 <li value="4"><p>Click <span class="bold">Order</span> to order the projects according to the portfolio priorities. </p><p>If you have projects that belong to more than one portfolio, you could see multiple projects with the same portfolio priority in the <em>Resource Planner</em>. In this case, the projects with the same portfolio priority are listed by the following criteria, in this order:</p>
  <ol>
   <li value="1"><p>Alignment Score</p></li>
   <li value="2"><p>Planned Start Date</p></li>
   <li value="3"><p>Project Name</p></li>
  </ol><p><img src="assets/rp-portfolio-priority-ordered-350x225.png" style="width: 350;height: 225;"></p></li>
 <li value="5">Click <span class="bold">Save</span>.</li>
</ol>

## The effect of changing the Project Planning Priority on User Available Hours

The Project Planning Priority affects the Available Hours of users. The users associated with the project with the highest priority show their fullest availability for the Available Hours (AVL) column for this project, according to their schedules.

The same users associated with the second project in order of priority will show an Available Hours value which is the difference between their full amount of Available Hours and what has already been budgeted for the first project in the Budgeted Hours column, and so on. For information about budgeting resources in the *Resource Planner*, see [Budget resources in the Resource Planner using the Project and Role views](../../resource-mgmt/resource-planning/budget-resources-project-role-views-resource-planner.md).

If no hours have been budgeted for the first project (in order of priority) for a user, but hours have been budgeted for the second project for the same user, the user will show the full amount of available hours for both projects.

We recommend updating the Budgeted Hours column for your users in the order of the projects in the *Resource Planner*, to ensure that you can accurately see the Available Hours for the user at all times.

>[!NOTE]
>
>Because the Project Planning Priority is unique to every resource manager, your second priority project might be a first priority project for another user viewing the same projects in their *Resource Planner*. If another resource manager budgets a resource for their first project, the Available Hours will decrease for that resource for your first project based on that change.
>
>The user who budgets the hours first allocates that resource and reduces the number of Available Hours for that resource across the system. The amount of Available Hours should update for all the users as soon as the Budgeted Hours are saved for a resource in the *Resource Planner*.
>
>For more information about Available Hours, see [Availability and allocation of resources](../../resource-mgmt/resource-planning/resource-availability-allocation-resource-planner.md#availability-and-allocation-of-resources).

