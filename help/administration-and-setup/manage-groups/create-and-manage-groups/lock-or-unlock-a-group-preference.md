---
filename: lock-or-unlock-a-group-preference
user-type: administrator
product-area: system-administration;user-management;setup
navigation-topic: create-and-manage-groups
title: Lock or unlock a project, task, or issue preference for subgroups
description: As a group administrator, you can configure and then lock a project, task, or issue preference if a Workfront administrator has unlocked it at the system level.
---

# Lock or unlock a project, task, or issue preference for subgroups

As a *group administrator*, you can configure and then lock a project, task, or issue preference if a *Workfront administrator* has unlocked it at the system level.

Locking a project, task, or issue preference that you have configured at the

<!--
<MadCap:conditionalText data-mc-conditions="SnippetConditions-wf-groups.groups">
group
</MadCap:conditionalText>
-->

`<MadCap:conditionalText data-mc-conditions="SnippetConditions-wf-groups.groups">  group</MadCap:conditionalText>` level ensures that everyone

<!--
<MadCap:conditionalText data-mc-conditions="SnippetConditions-wf-groups.groups">
in your group and in its subgroups
</MadCap:conditionalText>
-->

`<MadCap:conditionalText data-mc-conditions="SnippetConditions-wf-groups.groups">  in your group and in its subgroups</MadCap:conditionalText>` is using the same setting for that preference. Though you can still reconfigure a preference that you lock

<!--
<MadCap:conditionalText data-mc-conditions="SnippetConditions-wf-groups.groups">
for your group
</MadCap:conditionalText>
-->

`<MadCap:conditionalText data-mc-conditions="SnippetConditions-wf-groups.groups">  for your group</MadCap:conditionalText>`, *group administrators* can’t reconfigure it for 

<!--
<MadCap:conditionalText data-mc-conditions="SnippetConditions-wf-groups.groups">
sub
</MadCap:conditionalText>
-->

`<MadCap:conditionalText data-mc-conditions="SnippetConditions-wf-groups.groups"> sub</MadCap:conditionalText>`groups

<!--
<MadCap:conditionalText data-mc-conditions="SnippetConditions-wf-groups.groups">
on lower levels
</MadCap:conditionalText>
-->

`<MadCap:conditionalText data-mc-conditions="SnippetConditions-wf-groups.groups">  on lower levels</MadCap:conditionalText>`.

Conversely, unlocking a 

<!--
<MadCap:conditionalText data-mc-conditions="SnippetConditions-wf-groups.groups">
group’s
</MadCap:conditionalText>
-->

`<MadCap:conditionalText data-mc-conditions="SnippetConditions-wf-groups.groups"> group’s </MadCap:conditionalText>`project, task, or issue preference allows 

<!--
<MadCap:conditionalText data-mc-conditions="SnippetConditions-wf-groups.groups">
sub
</MadCap:conditionalText>
-->

`<MadCap:conditionalText data-mc-conditions="SnippetConditions-wf-groups.groups"> sub</MadCap:conditionalText>`*group administrators* more flexibility to manage the way their groups work with those items. When a 

<!--
<MadCap:conditionalText data-mc-conditions="SnippetConditions-wf-groups.groups">
group
</MadCap:conditionalText>
-->

`<MadCap:conditionalText data-mc-conditions="SnippetConditions-wf-groups.groups"> group </MadCap:conditionalText>`preference is unlocked, *group administrators*

<!--
<MadCap:conditionalText data-mc-conditions="SnippetConditions-wf-groups.groups">
of lower subgroups
</MadCap:conditionalText>
-->

`<MadCap:conditionalText data-mc-conditions="SnippetConditions-wf-groups.groups">  of lower subgroups</MadCap:conditionalText>` can reconfigure it for 

<!--
<MadCap:conditionalText data-mc-conditions="SnippetConditions-wf-groups.groups">
those subgroups
</MadCap:conditionalText>
-->

`<MadCap:conditionalText data-mc-conditions="SnippetConditions-wf-groups.groups"> those subgroups</MadCap:conditionalText>`.

This is parallel to the ability that a *Workfront administrator* has to lock or unlock a preference for everyone in the system.

For information about how a *Workfront administrator* can lock or unlock a preference for all groups in the system, see [Lock or unlock project preferences for all groups in the system](../../../administration-and-setup/set-up-workfront/configure-system-defaults/lock-or-unlock-project-preferences-for-groups-system.md).

>[!NOTE]
>
>* Configuring an unlocked preference for a group doesn’t affect that preference for any subgroups below the group.
>
>  However, when a new subgroup is created, it inherits the preference settings and locked or unlocked state of the group immediately above it.
>
>* If you move a group under a group that has a locked preference, the moved group inherits that preference and it is locked for the moved group. 
>* If you move a group under a group that has an unlocked preference, the moved group is not affected by that preference.
>
>  If the preference in the moved group is locked at the time of the move, it remains locked, but the *group administrator* can unlock it now because it is unlocked for the parent group.
>

## Access requirements

You must have the following to perform the steps in this article:

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><em>Workfront</em> plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><em>Adobe Workfront</em> license*</td> 
   <td> <p><em>Plan</em> </p> <p>You must be a <em>group administrator</em> of the group or a <em>Workfront administrator</em>. For more information, see <a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">Group administrators</a> and <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Grant a user full administrative access</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;If you need to find out what plan or license type you have, contact your *Workfront administrator*.

## Lock or unlock a group project, task, or issue preference

<ol> 
 <li value="1">Click the <span class="bold">Main Menu</span> icon <img src="assets/main-menu-icon.png"> in the upper-right corner of <em>Adobe Workfront</em>, then click <span class="bold">Setup</span> <img src="assets/gear-icon-settings.png">.</li> 
 <li value="2">In the left panel, click <span class="bold">Groups</span>.</li> 
 <li value="3">Click the name of the group where you want to lock or unlock a project preference.</li> 
 <li value="4">In the left panel, click <span class="bold">Project Preferences</span> or <span class="bold">Tasks & Issues Preferences</span>.</li> 
 <li value="5"> <p>On the page that appears, do any of the following for a preference that is unlocked at the system level or for a group above your group:</p> 
  <ul> 
   <li> <p>If you want administrators of groups below your group to be able to configure a preference for their groups, unlock it <img src="assets/unlock-toggle-button.png">.</p> </li> 
   <li> <p>If you want all groups below yours to use your configuration for a preference, make sure that it is locked <img src="assets/lock-toggle-button.png">.</p> <note type="important">
     It's important to communicate with the administrators and users in groups below yours to ensure that all needs are accounted for in the way you configure a locked preference. When you lock it, your configuration for it is inherited by any subgroups below. And if the preference has been unlocked for any period of time, your configuration replaces those that 
     <em>group administrators</em> in lower subgroups might have made.
    </note> </li> 
  </ul> </li> 
 <li value="6">Click <span class="bold">Save</span>.</li> 
</ol>

