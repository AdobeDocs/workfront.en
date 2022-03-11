---
filename: customize-default-issue-types
user-type: administrator
product-area: system-administration;projects
navigation-topic: configure-system-defaults
title: Customize default issue types
description: Issue types are useful in the following circumstances:
---

# Customize default issue types

Issue types are useful in the following circumstances:

* When customizing issue statuses, as described in [Create or edit a status](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).
* When creating a request queue, as described in [Create a Request Queue](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

You can customize the labels for each default issue type to better match the terminology used in your organization.

## Access requirements

You must have the following to perform the steps in this article:

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
   <td> <p><span>Plan</span> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>You must be a <span>Workfront administrator</span>. For more information, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Grant a user full administrative access</a>.</p> <p>Note: If you still don't have access, ask your <span>Workfront administrator</span> if they set additional restrictions in your access level. For information on how a <span>Workfront administrator</span> can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Default issue types

If you have `Adobe Workfront administrator` access, there are four default issue types that you can configure and rename:

* `Bug Report` Used to track reported bugs in the system.
* `Change Order` Used to track issues&nbsp;that need to&nbsp;be updated or revised.
* `Issue` An object in `Workfront` that communicates unplanned work, a problem that arises, or something that must be resolved in order to continue a task.

* `Request` An issue type that applies to a request queue where users make requests in `Workfront`.

![](assets/screenshot-2016-05-10-16.56.24-350x202.png) 

## Customize an issue type

Consider the following about customizing issue types:

* You can modify the label for an issue type, but you can't change its function.
* You can't create additional issue types.
* You can't change the filter values for the name of an issue type. So, if you create a filter on an issue report, the value of the filter (key) does not reflect the issue type's custom name. 
* Three default statuses are associated with each issue type: New, In Progress, and Closed. You can't delete these statuses or remove them from an issue type, but you can rename them.
* You can re-order the options that appear on the drop-down menu for each issue type.

To customize an issue type:

<ol> 
 <li value="1">Click the <span class="bold">Main Menu</span> icon <img src="assets/main-menu-icon.png"> in the upper-right corner of <span>Adobe Workfront</span>, then click <span class="bold">Setup</span> <img src="assets/gear-icon-settings.png">.</li> 
 <li value="2">Click <span class="bold">Project Preferences</span> > <span class="bold">Statuses</span>.</li> 
 <li value="3">Click the <span class="bold">Issues</span> tab.</li> 
 <li value="4">Do any of the following:
  <ul>
   <li><p>Hover over the issue type you want to customize, click the Edit icon <img src="assets/edit-icon.png"> that appears to the far right, then type a new name for the issue type.</p><p><img src="assets/customize-issue-type-350x187.png" style="width: 350;height: 187;"></p></li>
   <li>Click an issue type to list its associated statuses, then drag the handles that appear when you hover over them and and drop them in the order you want them to appear in your users' issue <span class="bold">Status</span> drop-down menu.</li>
  </ul></li> 
</ol>

