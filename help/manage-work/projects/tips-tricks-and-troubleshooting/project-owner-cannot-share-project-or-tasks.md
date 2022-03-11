---
filename: project-owner-cannot-share-project-or-tasks
content-type: tips-tricks-troubleshooting
product-area: projects;user-management
navigation-topic: tips-tricks-and-troubleshooting-projects
title: Project Owner cannot share a project or any of its tasks with a team
description: A user who is designated as the Project Owner of a project and has Manage permissions on the project is unable to share their project or any of its tasks with a Team. When they are sharing the project, a certain Team is not available to share and cannot be found in the Give project access to or the Give task access to fields.
---

# Project Owner cannot share a project or any of its tasks with a team

## Problem

A user who is designated as the `Project Owner` of a project and has `Manage` permissions on the project is unable to share their project or any of its tasks with a Team. When they are sharing the project, a certain `Team` is not available to share and cannot be found in the `Give project access to` or the `Give task access to` fields.

## Cause

The `Adobe Workfront administrator` restricted the user to viewing only Companies, Groups & Teams they belong to in the Access Level of the user. The team that the user is looking for is not one of their own teams.

## Solution

As a `Workfront administrator`, do the following:

<ol> 
 <li value="1">Find the user and click to access it.</li> 
 <li value="2"> Click the More menu next to the name of the user, then click Edit. </li> 
 <li value="3">Click <span class="bold">Access</span> and make note of the name of the <span class="bold">Access Level</span> assigned to this user.</li> 
 <li value="4"> Click the Main Menu icon in the upper-right corner of Adobe Workfront. </li> 
 <li value="5">Go to <span class="bold">Setup > Access Levels.</span></li> 
 <li value="6">Click the name of the <span class="bold">Access Level</span> to edit it.&nbsp;</li> 
 <li value="7"> <p>Deselect the following field: <span class="bold">View only companies, groups & teams they belong to.</span></p> <p> <img src="assets/view-only-team-groups-companies-they-belong-to-350x141.png" style="width: 350;height: 141;"> </p> </li> 
 <li value="8">Click <span class="bold">Save</span> <span class="bold">.</span></li> 
 <li value="9">Ask the user to share the project or the tasks with the team, again.&nbsp;</li> 
</ol>

>[!NOTE]
>
>As an alternative solution, you can assign the team to the user. However, we recommend against this solution because the user might be exposed to information belonging to the team that would be confusing to them, or they might get work requests or notifications addressed to the team that might be confusing to them.

