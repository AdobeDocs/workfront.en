---
filename: issue-status
content-type: tips-tricks-troubleshooting
product-area: projects
navigation-topic: tips-tricks-and-troubleshooting-groups
title: Configure the Done button for issues if no team is assigned
description: Clicking the Done button on an issue updates the status for the issue. By default, the Done button marks an issue as Resolved. Users with certain permissions can configure the Done button to reflect certain statuses in the system. The primary way to configure statuses for the Done button is through the Home Team. For more information, see Configure the Done button for issues.
---

# Configure the Done button for issues if no team is assigned

Clicking the Done button on an issue updates the status for the issue. By default, the Done button marks an issue as Resolved. Users with certain permissions can configure the Done button to reflect certain statuses in the system. The primary way to configure statuses for the Done button is through the Home Team. For more information, see [Configure the Done button for issues](../../people-teams-and-groups/create-and-manage-teams/configure-the-done-button-for-issues.md).

If the user does not have a Home Team assigned, the Done button for issues is tied to a system-generated Resolved status that has the three-letter code RLV. System administrators can delete the Resolved (RLV) status if they wish, though this is not recommended.

If the Resolved (RLV) status is deleted and the user marking the issue as Done has no Home Team, the default issue status is tied to whatever is set as the default for Closed for the group assigned to the project. This article explains how to find the group associated with a project, then update that status if needed.

## Access requirements

You must have the following access to perform the steps in this article:

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><span>Adobe Workfront</span> plan</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><span>Adobe Workfront</span> license</td> 
   <td> <p>Plan</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>System administrator</p> </td> 
  </tr> 
 </tbody> 
</table>

## Find the group associated with the project

When a user creates a project, their Home group is automatically assigned to the project. Users can change this group in the Project Details section at any time. You need to know what group is on a specific project to modify the default status for the issue Done button. To find the group associated with the project

1. Go to a project.

## Update the default status for a specific group

<ol> Click the Main Menu icon in the upper-right corner of Adobe Workfront, then click Setup . 
 <li value="2">In the left panel, click <span class="bold">Project Preferences</span>, then <span class="bold">Statuses</span>.</li> 
 <li value="3">Click <span class="bold">Requests</span>, then type the name of the group in the <span class="bold">System Statuses</span> search box located on the right.</li> 
 <li value="4">Select the group.</li> 
 <li value="5"> <p>Click the Set Default Statuses drop-down menu, then choose the status you want the Done button to use. </p> <note type="important">
   This status is used only when they user has no assigned Home Team and the RLV status has been deleted.
  </note> </li> 
 <li value="6">Click <span class="bold">Save</span>.</li> 
</ol>

