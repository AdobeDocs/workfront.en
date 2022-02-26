---
filename: configure-system-updates
user-type: administrator
product-area: system-administration;setup
navigation-topic: system-tracked-update-feeds
title: Configure system updates
description: Adobe Workfront generates automatic system updates in an object's Updates area to record the following events:
---

# Configure system updates

*Adobe Workfront* generates automatic system updates in an object's Updates area to record the following events:

* Changes users make in an object field
* Actions users perform on an object

These system updates include the change that was made, the name of the user who made the change, and the time and date of the change.

As a *Workfront administrator*, you can configure which object fields and actions *Workfront* tracks to record system updates.

For example, you could have *Workfront* track all changes users make to the names of issues throughout the system. Any issue name change then appears as a system update on the issue's Updates area.

## Access requirements

You must have the following to perform the steps in this article:

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><em>Adobe Workfront</em> plan</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><em>Adobe Workfront</em> license</td> 
   <td> <p><em>Plan</em> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>You must be a <em>Workfront administrator</em>. For more information, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Grant a user full administrative access</a>.</p> <p>Note: If you still don't have access, ask your <em>Workfront administrator</em> if they set additional restrictions in your access level. For information on how a <em>Workfront administrator</em> can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Determine which fields *Workfront* tracks for an object type

You can determine what information *Workfront* tracks when users change information associated with a certain object type throughout the entire *Workfront* interface. You do this by adding or removing the fields you want *Workfront* to track for that object type.

>[!NOTE]
>
>* *Workfront* cannot track and record updates about calculated custom fields.
>* You can customize the system update for projects, tasks, issues, portfolios, programs, and users. You cannot customize the system update for templates, documents or timesheets, but *Workfront* does record system updates for these objects.
>

* [Add fields you want Workfront to track](#adding-fields-to-the-update-feeds) 
* [Remove fields that you don't want tracked](#removing-fields-from-the-update-feeds)

### Add fields you want *Workfront* to track

You can add fields you want *Workfront* to track for a particular type of object throughout the *Workfront* interface. When users change information in that field, *Workfront* records information about the change as a system update in the Updates area for the object.

>[!NOTE]
>
>You can track up to 300 built-in and custom fields in the update feeds. If you are tracking the maximum number of fields and want to track additional fields that are not displayed in the All Fields Sub-tab, you must first remove some of the tracked fields in order to track new fields. For more information about removing fields from the update fields, see see [Remove fields that you don't want tracked](#removing-fields-from-the-update-feeds).

<ol data-mc-continue="false"> <draft-comment>
  <li value="1" data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click the <span class="bold">Main Menu</span> icon <img src="assets/main-menu-icon.png"> in the upper-right corner of <em>Adobe Workfront</em>, then click <span class="bold">Setup</span> <img src="assets/gear-icon-settings.png">.</li>
 </draft-comment>
 <li value="1" data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click the <span class="bold">Main Menu</span> icon <img src="assets/main-menu-icon.png"> in the upper-right corner of <em>Adobe Workfront</em>, then click <span class="bold">Setup</span> <img src="assets/gear-icon-settings.png">.</li> 
 <li value="2">In the panel on the left, click <span class="bold">Interface</span> > <span class="bold">Update Feeds</span>.<br></li> 
 <li value="3">​Click <span class="bold">Add Fields</span>, then click the object that you want to be tracked.<br></li> 
 <li value="4"> <p>In the<draft-comment>
    <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
     <span class="bold">Update Feeds</span>
    </MadCap:conditionalText>
   </draft-comment><MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
    <span class="bold">Update Feeds</span>
   </MadCap:conditionalText> box that appears, start typing either a built-in (standard) field or a custom field for the object, then click to select it when it appears in the list.<br></p> <p>If <em>Workfront</em> is already tracking the field, you cannot add it a second time from the list.</p> <draft-comment>
   <p data-mc-conditions="QuicksilverOrClassic.Quicksilver"> <img src="assets/updates-feeds-box-qs-350x219.png" style="width: 350;height: 219;"> <br> </p>
  </draft-comment><p data-mc-conditions="QuicksilverOrClassic.Quicksilver"> <img src="assets/updates-feeds-box-qs-350x219.png" style="width: 350;height: 219;"> <br> </p> </li> 
 <li value="5"> <p>After adding all the fields you want <em>Workfront</em> to track, click <span class="bold">Add Fields</span>.<br></p> <p>The built-in fields that you added show under the <span class="bold">Built-in Fields</span> sub-tab.</p> <p>The custom fields you added show under the <span class="bold">Custom Fields</span> sub-tab.<br></p> <p>The <span class="bold">All Fields</span> sub-tab shows both the built-in and the custom fields that are being tracked.</p> </li> 
</ol>

### Remove fields that you don't want tracked

You can remove fields you do not want the system to track for a particular type of object throughout the *Workfront* interface.

<ol data-mc-continue="false"> <draft-comment>
  <li value="1" data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click the <span class="bold">Main Menu</span> icon <img src="assets/main-menu-icon.png"> in the upper-right corner of <em>Adobe Workfront</em>, then click <span class="bold">Setup</span> <img src="assets/gear-icon-settings.png">.</li>
 </draft-comment>
 <li value="1" data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click the <span class="bold">Main Menu</span> icon <img src="assets/main-menu-icon.png"> in the upper-right corner of <em>Adobe Workfront</em>, then click <span class="bold">Setup</span> <img src="assets/gear-icon-settings.png">.</li> 
 <li value="2">Click <span class="bold">Interface</span> > <span class="bold">Update Feeds</span>.<br></li> 
 <li value="3"> <p>On the <span class="bold">Tracked Fields</span> tab, select the <span class="bold">All Fields</span> sub-tab.<br></p> <p>This shows both the built-in and the custom fields that are currently being tracked.</p> </li> 
 <li value="4"> <p>Select the field you want to stop tracking, then click <span class="bold">Remove</span>.<br></p> </li> 
 <li value="5"> <p>In the <span class="bold">Remove Field</span> box that appears, click <span class="bold">Yes, Remove It</span> to confirm.</p> </li> 
</ol>

Any updates about the previously-tracked fields are preserved in the Updates area where they were recorded.

## Determine which actions *Workfront* tracks for an object type

You can have *Workfront* track the following actions that users can perform on objects throughout the *Workfront* interface.

For example, you can have *Workfront* record an update every time a user changes an assignment to a task or issue. The change then appears as a system update in the Updates area for the task or issue.

<table cellspacing="15"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><span class="bold">Action</span> </th> 
   <th><span class="bold">Objects</span> </th> 
   <th><span class="bold">Default Status</span> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Assignment is changed</td> 
   <td>Tasks, Issues</td> 
   <td> <p>Enabled</p> </td> 
  </tr> 
  <tr> 
   <td>Baseline is deleted</td> 
   <td>Projects</td> 
   <td> <p>Disabled</p> </td> 
  </tr> 
  <tr> 
   <td>Billing record is created or deleted</td> 
   <td>Projects</td> 
   <td> <p>Enabled</p> </td> 
  </tr> 
  <tr> 
   <td>Document is created or deleted</td> 
   <td>Projects, Tasks, Issues, Portfolios, Programs</td> 
   <td> <p>Enabled</p> </td> 
  </tr> 
  <tr> 
   <td>Expense is created or deleted</td> 
   <td>Projects, Tasks</td> 
   <td> <p>Enabled</p> </td> 
  </tr> 
  <tr> 
   <td>Hour is logged or deleted</td> 
   <td>Projects, Tasks, Issues</td> 
   <td> <p>Enabled</p> </td> 
  </tr> 
  <tr> 
   <td>Issue is deleted</td> 
   <td>Projects</td> 
   <td> <p>Enabled</p> </td> 
  </tr> 
  <tr> 
   <td>Task is deleted</td> 
   <td>Projects</td> 
   <td> <p>Enabled</p> </td> 
  </tr> 
  <tr> 
   <td>Someone's Access is changed</td> 
   <td>Projects, Tasks, Issues, Documents, Portfolios, Programs</td> 
   <td> <p>Enabled</p> </td> 
  </tr> 
  <tr> 
   <td>Subscribe comment object</td> 
   <td>Projects, Tasks, Issues</td> 
   <td> <p>Enabled</p> </td> 
  </tr> 
 </tbody> 
</table>

To configure which actions you want *Workfront* to track:

<ol data-mc-continue="false"> <draft-comment>
  <li value="1" data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click the <span class="bold">Main Menu</span> icon <img src="assets/main-menu-icon.png"> in the upper-right corner of <em>Adobe Workfront</em>, then click <span class="bold">Setup</span> <img src="assets/gear-icon-settings.png">.</li>
 </draft-comment>
 <li value="1" data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click the <span class="bold">Main Menu</span> icon <img src="assets/main-menu-icon.png"> in the upper-right corner of <em>Adobe Workfront</em>, then click <span class="bold">Setup</span> <img src="assets/gear-icon-settings.png">.</li> 
 <li value="2">Click <span class="bold">Interface</span> > <span class="bold">Update Feeds</span>.<br></li> 
 <li value="3">Click the <span class="bold">Actions</span> tab.<br></li> 
 <li value="4">Select an action to enable it, or deselect an action to disable it.</li> 
 <li value="5">Click <span class="bold">Save</span>.</li> 
</ol>

When you disable an action, any previously-recorded update about that action is preserved in the Updates area where it was recorded.
