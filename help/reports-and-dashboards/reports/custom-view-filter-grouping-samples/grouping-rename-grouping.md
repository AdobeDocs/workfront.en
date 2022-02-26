---
filename: grouping-rename-grouping
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: Grouping: edit the display name in a grouping
description: You can rename groupings to something more familiar to your users.
---

# Grouping: edit the display name in a grouping

You can rename groupings to something more familiar to your users.

For example, when you apply the standard Portfolio Name grouping to a list of projects, the name of the grouping appears as *Portfolio: Name: <name of portfolio>*.

![](assets/grouping-unedited-name-350x167.png)

You can modify this grouping using text mode to display a name that is easier to read.

![](assets/grouping-edited-name-350x160.png)

## Access requirements

You must have the following access to perform the steps in this article:

<table cellspacing="0"> 
 <col> 
 <col> 
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
   <td> <p>Edit access to&nbsp;Reports,&nbsp;Dashboards,&nbsp;Calendars</p> <p>Edit access to Filters, Views, Groupings</p> <p>Note: If you still don't have access, ask your <em>Workfront administrator</em> if they set additional restrictions in your access level. For information on how a <em>Workfront administrator</em> can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to a report</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects in Adobe Workfront</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your *Workfront administrator*.

## Edit the display name in a grouping

To change the display name in a project grouping:

<ol> 
 <li value="1">Go to a list of projects.</li> 
 <li value="2">From the <span class="bold">Grouping</span>drop-down menu, select <span class="bold">New Grouping</span>.</li> 
 <li value="3">Click&nbsp;<span class="bold">Add Grouping</span>, and start typing "Portfolio Name" in the <span class="bold">First by:</span> field, then select it when it displays in the list.</li> 
 <li value="4">Click <span class="bold">Switch to Text Mode</span>.</li> 
 <li value="5"> <p>Done one of following:</p> 
  <ul> 
   <li> <p> Add the following code to the existing text available in the <span class="bold">Group your Report</span> box:</p> <p><code>group.0.displayname=Your </code><code data-mc-edit-date="2019-01-07T12:27:43.3787530-05:00" data-mc-editor="alinawilson" data-mc-comment="Alina: maybe add a screen shot here?" data-mc-initials="AL" data-mc-creator="alinawilson" data-mc-create-date="2019-01-07T12:27:30.8346347-05:00">Value</code> </p> <p>Or, in this case:</p> <p><code>group.0.displayname=Portfolio</code> </p> </li> 
   <li> <p>Remove all the lines in the text mode interface of the grouping that have the word "name" in them, then add the line:</p> <p><code>group.0.name=Your Value</code> </p> <p>Or, in this case:</p> <p><code>group.0.name=Portfolio</code> </p> <p>You can also leave the <code>group.0.name</code> line blank, in which case the grouping shows the name of the value you are grouping by.</p> <p> <img src="assets/grouping-edited-name-no-name-350x162.png" style="width: 350;height: 162;"> </p> </li> 
  </ul> </li> 
 <li value="6">Click <span class="bold">Done</span>, then <span class="bold">Save Grouping</span>.</li> 
</ol>

