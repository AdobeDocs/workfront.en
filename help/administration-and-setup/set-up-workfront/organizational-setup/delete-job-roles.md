---
filename: delete-job-roles
user-type: administrator
product-area: system-administration;user-management
navigation-topic: organization-setup
title: Delete job roles
description: You can delete job roles that your organization no longer uses. We recommend that you do not delete job roles if they have been associated with work items in the past. To keep all your historical information about work assignments, we recommend that you deactivate roles, rather than delete them when they become obsolete. For information about deactivating roles, see Deactivate job roles.
---

# Delete job roles

You can delete job roles that your organization no longer uses. We recommend that you do not delete job roles if they have been associated with work items in the past. `To keep all your historical information about work assignments, we recommend that you deactivate roles, rather than delete them when they become obsolete. For information about deactivating roles, see [Deactivate job roles](../../../administration-and-setup/set-up-workfront/organizational-setup/deactivate-job-roles.md).`

## Access requirements

You must have the following:

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
   <td> <p><em>Plan</em> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Administrative access to Job roles</p> <p>Note: If you still don't have access, ask your <em>Workfront administrator</em> if they set additional restrictions in your access level. For information on how a <em>Workfront administrator</em> can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your *Workfront administrator*.

## Delete a job role

<ol data-mc-continue="false"> <draft-comment>
  <li value="1" data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click the <span class="bold">Main Menu</span> icon <img src="assets/main-menu-icon.png"> in the upper-right corner of <em>Adobe Workfront</em>, then click <span class="bold">Setup</span> <img src="assets/gear-icon-settings.png">.</li>
 </draft-comment>
 <li value="1" data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click the <span class="bold">Main Menu</span> icon <img src="assets/main-menu-icon.png"> in the upper-right corner of <em>Adobe Workfront</em>, then click <span class="bold">Setup</span> <img src="assets/gear-icon-settings.png">.</li> 
 <li value="2">Click<span class="bold"> Job Roles.</span></li> 
 <li value="3">Select the job role that you want to delete, then click <span class="bold">Delete.</span></li> 
 <li value="4">If there are any objects (users, tasks, issues) that&nbsp;are assigned to the job role, do one of the following:<br> 
  <ul> 
   <li><p><span class="bold">Replace&nbsp;the job role with a different job role:</span> Select the new job role from the drop-down list.</p><p>Any current and past resource allocations that are&nbsp;associated with the deleted job role are transferred to the job role that you select.</p><p>Users who have only one job role assigned to&nbsp;them are reassigned to the job role that you select; users who have a secondary job role assigned to them are not reassigned to the job role that you select.</p></li> 
   <li><p><span class="bold">Delete&nbsp;the job role and its resource allocation:</span> Select<span class="bold"> None</span>&nbsp;from the drop-down list.</p><note type="important">
      Deleting a job role deletes all current and past resource allocation related to that job role for all projects.
    </note><p>​For example, if a task or issue is assigned to only that job role, the task or issue is unassigned after the job role is deleted.</p></li> 
  </ul></li> 
 <li value="5">Click <draft-comment>
   <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
    <span class="bold">Yes, Delete It</span>. 
   </MadCap:conditionalText>
  </draft-comment><MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
   <span class="bold">Yes, Delete It</span>. 
  </MadCap:conditionalText></li> 
</ol>

