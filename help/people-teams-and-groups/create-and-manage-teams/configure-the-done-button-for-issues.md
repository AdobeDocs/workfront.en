---
filename: configure-the-done-button-for-issues
product-area: agile-and-teams;setup
navigation-topic: create-and-manage-teams
title: Configure the Done button for issues
description: The Done button can automatically set the status of a task or an issue. By default, Adobe Workfront marks an issue as Resolved when an assignee clicks Done on their work item.
---

# Configure the Done button for issues

The Done button can automatically set the status of a task or an issue. By default, *Adobe Workfront*&nbsp;marks an issue as Resolved when an assignee clicks Done on their work item.

## Overview

&nbsp;Users with certain permissions can configure the Done button to reflect certain statuses in the system. There are 3 different ways the Done button works for issues in Workfront:

* If the user has an assigned Home Team, a *Workfront administrator* or a user with a Plan license can configure the Done button to reflect certain statuses for team members. See [Configure the Done button for a Team](#configur) in this article.

* If the user does not have a Home Team assigned, the Done button for issues is tied to a system-generated Resolved status that has the three-letter code RLV. There are no configuration options available in this scenario. The Done button automatically defaults to this status.
* If the Resolved (RLV) status is deleted and the user marking the issue as Done has no Home Team, the default issue status is tied to whatever is set as the default for Closed for the group assigned to the project the issue belongs to. The *Workfront administrator* can configure a system-wide default setting for the group. See [Configure the Done button when the Resolved status has been deleted](#configur2) in this article.

## Access requirements

You must have the following access to perform the steps in this article:

<table cellspacing="0"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><em>Adobe Workfront</em> plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><em>Adobe Workfront</em> license*</td> 
   <td> <p><em>Plan</em> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td>System administrator access is required to configure the Done button when the Resolved status is deleted</td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your *Workfront administrator*.

## Configure the Done button for a Team

You can change which status is applied to the work item with the Done button. You can also set multiple statuses and allow the user to choose which status is appropriate.

<ol> <draft-comment>
  <li value="1" data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click the <span class="bold">Main Menu</span> icon <img src="assets/main-menu-icon.png"> in the upper-right corner of <em>Adobe Workfront</em>, then click <span class="bold">Teams</span>.</li>
 </draft-comment>
 <li value="1" data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click the <span class="bold">Main Menu</span> icon <img src="assets/main-menu-icon.png"> in the upper-right corner of <em>Adobe Workfront</em>, then click <span class="bold">Teams</span>.</li> <draft-comment>
  <li value="2" data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click the <span class="bold">Switch team</span> icon, then either select a new team from the drop-down menu or search for a team in the search bar.</li>
 </draft-comment>
 <li value="2" data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click the <span class="bold">Switch team</span> icon, then either select a new team from the drop-down menu or search for a team in the search bar.</li> 
 <li value="3"> <draft-comment>
   <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click the <span class="bold">More</span> menu, then click <span class="bold">Edit</span>.</p>
  </draft-comment><p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click the <span class="bold">More</span> menu, then click <span class="bold">Edit</span>.</p> </li> 
 <li value="4">Find the <span class="bold">Done Button</span> section at the bottom of the <span class="bold">Team Settings</span> page.</li> 
 <li value="5">Select one status or more than one status for each work item type.<br><br><br><note type="note">
   <p>Consider the following when selecting statuses:<br></p>
   <ul>
    <li>When you select one status for each type of work item, the task or issue status is set to that status when a user clicks Done on their&nbsp;item.&nbsp;If you set multiple statuses for each type of work item, a drop-down menu is added to the Done button and the user must pick a status to change the status on the work item.<br></li>
    <li><p>You can associate only system-level statuses with the Done button. You cannot associate Group-specific statuses with work item statuses.</p></li>
    <li>Issue types are customizable and they might have different names than listed below in your environment.<br>Following&nbsp;are the default tasks and issue types:
     <ul>
      <li>Tasks</li>
      <li>Issue</li>
      <li>Request</li>
      <li>Change Order</li>
      <li>Bug Report</li>
     </ul></li>
   </ul>
  </note>If the task or issue is assigned to multiple users, you see a "Done with my part" option in the drop-down menu, in addition to the multiple statuses chosen for your team.<br></li> 
 <li value="6">Click <span class="bold">Save Changes</span>.</li> 
</ol>

## Associate users with a Home Team

To make the changes to the Done button functionality visible to users, you can make the team whose settings you changed the Home Team of the users.&nbsp;

To associate users with a Home Team:

<ol> <draft-comment>
  <li value="1" data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click the <span class="bold">Main Menu</span> icon <img src="assets/main-menu-icon.png"> in the upper-right corner of <em>Adobe Workfront</em>.</li>
 </draft-comment>
 <li value="1" data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click the <span class="bold">Main Menu</span> icon <img src="assets/main-menu-icon.png"> in the upper-right corner of <em>Adobe Workfront</em>.</li> <draft-comment>
  <li value="2" data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click <span class="bold">Users</span>, then select the user or users you want to associate with a Home Team.</li>
 </draft-comment>
 <li value="2" data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click <span class="bold">Users</span>, then select the user or users you want to associate with a Home Team.</li> <draft-comment>
  <li value="3" data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click the <span class="bold">More</span> menu, then select <span class="bold">Edit</span>.<br><img src="assets/user-settings-nwe-350x291.png" style="width: 350;height: 291;"></li>
 </draft-comment>
 <li value="3" data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click the <span class="bold">More</span> menu, then select <span class="bold">Edit</span>.<br><img src="assets/user-settings-nwe-350x291.png" style="width: 350;height: 291;"></li> 
 <li value="4">In the <span class="bold">Organization</span> section, select&nbsp;the <span class="bold">Home Team</span> field. Start typing the name of the team whose settings you want to associate with the&nbsp;users. Click the name of the team when you see it in the list.</li> 
 <li value="5">Click <span class="bold">Save Changes</span>.<br>The&nbsp;users you selected are now associated with a&nbsp;Home Team. &nbsp;<br>Any team settings, including the statuses associated with the Done button are now visible to these users.&nbsp;</li> 
</ol>

## Configure the Done button when the Resolved status has been deleted

If a user does not have a Home Team and the system-wide default for Resolved (RLV) has been deleted, a *Workfront administrator* can configure the Closed status for the group on to the project. Workfront selects this status for a closed issue when the user clicks the Done button.

### Find the group associated with the project

When a user creates a project, their Home Group is automatically assigned to the project. Users with Manage access to the project can change this group in the Project Details section at any time. To understand what status Workfront uses for a completed issue in this case, you must understand what group is associated with the project the issue is on and what the default status for Closed this group has for issues.

To find the group associated with the project:

1. Go to a Project.

   <!--
   <li value="2" data-mc-conditions="QuicksilverOrClassic.Quicksilver">On the left side of the page, click <span class="bold">Project Details</span>.</li>
   -->

1. On the left side of the page, click `Project Details`.

   <!--
   <li value="3" data-mc-conditions="QuicksilverOrClassic.Quicksilver">Locate the <span class="bold">Project association</span> section, then find <span class="bold">Group</span>.<br>This is the group name you need to use to check the status in the Setup area. See the following section for instructions on how to update the default status for a specific group.</li>
   -->

1. Locate the `Project association` section, then find `Group`.  
   This is the group name you need to use to check the status in the Setup area. See the following section for instructions on how to update the default status for a specific group.

### Update the default status for a specific group

As a *Workfront administrator*, you can update the status for a specific group:

<ol> <draft-comment>
  <li value="1" data-mc-conditions="QuicksilverOrClassic.Quicksilver"> <p>Click the <span class="bold">Main Menu</span> icon <img src="assets/main-menu-icon.png"> in the upper-right corner of <em>Adobe Workfront</em>, then click <span class="bold">Setup</span> <img src="assets/gear-icon-settings.png">.</p> </li>
 </draft-comment>
 <li value="1" data-mc-conditions="QuicksilverOrClassic.Quicksilver"> <p>Click the <span class="bold">Main Menu</span> icon <img src="assets/main-menu-icon.png"> in the upper-right corner of <em>Adobe Workfront</em>, then click <span class="bold">Setup</span> <img src="assets/gear-icon-settings.png">.</p> </li> 
 <li value="2">In the left panel, click <span class="bold">Project Preferences</span>, then <span class="bold">Statuses</span>.</li> 
 <li value="3">Click <span class="bold">Issues</span>, then type the name of the group in the <span class="bold">System Statuses</span> search box located on the right.</li> 
 <li value="4">Select the group.</li> 
 <li value="5"> <p>Click the <span class="bold">Set Default Statuses</span> drop-down menu, then choose a default status for Closed. Workfront uses this status for a closed issue when a user clicks the Done button.</p> <note type="important">
   This status is used only when the user has no assigned Home Team and the RLV status has been deleted.
  </note> </li> 
 <li value="6">Click <span class="bold">Save</span>.</li> 
</ol>

