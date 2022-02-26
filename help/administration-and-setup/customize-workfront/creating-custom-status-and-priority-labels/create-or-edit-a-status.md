---
filename: create-or-edit-a-status
title: Create and customize statuses
user-type: administrator
product-area: system-administration
navigation-topic: create-custom-status-and-priority-labels
title: Create or edit a status
description: As an Adobe Workfront administrator, you can create custom statuses for projects, tasks, and issues. These can be for users throughout the entire Workfront system or for specific groups or subgroups. For more information about statuses, see Statuses overview.
---

# Create or edit a status

As an *Adobe Workfront administrator*, you can create custom statuses for projects, tasks, and issues. These can be for users throughout the entire *Workfront* system or for specific groups or subgroups. For more information about statuses, see [Statuses overview](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/statuses-overview.md).

>[!NOTE]
>
>*Group administrators* can also create their own group statuses, for use only by their groups. For more information, see [Create or edit a group status](../../../administration-and-setup/manage-groups/manage-group-statuses/create-or-edit-a-group-status.md).

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

## Create a custom status

You can add a custom status for use by your entire organization or by a single group.

When you create a custom status for the entire organization, you can configure it so that all groups in the system can use it without editing it. Or you can configure it so that *group administrators* can modify it for their groups, as explained in [Create or edit a group status](../../../administration-and-setup/manage-groups/manage-group-statuses/create-or-edit-a-group-status.md).

<ol> 
 <li value="1">Click the <span class="bold">Main Menu</span> icon <img src="assets/main-menu-icon.png"> in the upper-right corner of <em>Adobe Workfront</em>, then click <span class="bold">Setup</span> <img src="assets/gear-icon-settings.png">.</li> 
 <li value="2">In the left panel, click <span class="bold">Project Preferences</span> > <span class="bold">Statuses</span>.</li> 
 <li value="3"> <p>(Conditional) If you are creating a status for use system wide, ensure that<span class="bold"> System Statuses</span> is selected in the box in the upper-right corner.</p> <draft-comment>
   <p data-mc-conditions="QuicksilverOrClassic.Quicksilver"> <img src="assets/system-statuses-in-upper-rt-corner-350x140.jpg" style="width: 350;height: 140;"> </p>
  </draft-comment><p data-mc-conditions="QuicksilverOrClassic.Quicksilver"> <img src="assets/system-statuses-in-upper-rt-corner-350x140.jpg" style="width: 350;height: 140;"> </p> <p>Or</p> <p>If you are creating a status for a group or subgroup, start typing the name of the group in the box in the upper-right corner, then select it when it appears.</p> <draft-comment>
   <p class="preview" data-mc-conditions="QuicksilverOrClassic.Quicksilver"> <img src="assets/system-statuses-in-upper-rt-corner-group-350x139.jpg" style="width: 350;height: 139;"> </p>
  </draft-comment><p class="preview" data-mc-conditions="QuicksilverOrClassic.Quicksilver"> <img src="assets/system-statuses-in-upper-rt-corner-group-350x139.jpg" style="width: 350;height: 139;"> </p> </li> 
 <li value="4">Select the tab of the object type (<span class="bold">Project</span>, <span class="bold">Tasks</span>, or <span class="bold">Issues</span>) that you want to associate with the status.</li> 
 <li value="5"> <p>If you are creating a new status, click <span class="bold">Add a New Status</span>.</p> <p>Or</p> <p>If you are editing an existing status, hover over it, then click the <span class="bold">Edit</span> icon that displays to the far-right.</p> <draft-comment>
   <p data-mc-conditions="QuicksilverOrClassic.Quicksilver"> <img src="assets/custom-status-edit-350x178.png" alt="" style="width: 350;height: 178;"> </p>
  </draft-comment><p data-mc-conditions="QuicksilverOrClassic.Quicksilver"> <img src="assets/custom-status-edit-350x178.png" alt="" style="width: 350;height: 178;"> </p> </li> 
 <li value="6"> <p>Configure the status using the following options:</p> 
  <table cellspacing="0"> 
   <col> 
   <col> 
   <tbody> 
    <tr> 
     <td role="rowheader">Status Name</td> 
     <td> <p>Type a name for the status. This is a required field.</p> <p>When you create a status name, be aware that others in the system can create a status with the same name. We recommend using a unique name to avoid confusion when selecting statuses in <em>Workfront</em>.</p> </td> 
    </tr> 
    <tr> 
     <td role="rowheader">Description</td> 
     <td>(Optional) Type a description of the status. This communicates its purpose to those who use it.</td> 
    </tr> 
    <tr> 
     <td role="rowheader">Color</td> 
     <td> <p>Customize the color of the status by clicking the color field and selecting a color from the swatch panel. You can also enter a hex number in the field.</p> <p>The status color displays in the upper-right corner of <em>Workfront</em> when a user views the object.</p> <draft-comment>
       <p data-mc-conditions="QuicksilverOrClassic.Quicksilver"> <img src="assets/status-color-350x211.png" style="width: 350;height: 211;"> </p>
      </draft-comment><p data-mc-conditions="QuicksilverOrClassic.Quicksilver"> <img src="assets/status-color-350x211.png" style="width: 350;height: 211;"> </p> </td> 
    </tr> 
    <tr> 
     <td role="rowheader">Equates With</td> 
     <td> <p>Select one of the options from the list that best describes the function of the status. For example, if the status name is Done, the option it equates with should be Complete.</p> <p>Every status must equate with one of these options because this determines how the status functions.</p> <p>This option cannot be modified after the status is created.</p> </td> 
    </tr> 
    <tr> 
     <td role="rowheader">Key</td> 
     <td> <p>If you are creating a new status, type a code or abbreviation for the status or use the one generated for you. This key must be unique in <em>Workfront</em> because it can be used for reporting purposes. If you attempt to specify a key that is already in use in the system, the field turns red.</p> <p>It might be useful to use an abbreviation that is recognizable to those who will use it.</p> <p>This option cannot be modified after the status is created.</p> <p>You cannot change the key code for Planning, Current, and Complete statuses. This is important if you are building a report in text mode.<br></p> </td> 
    </tr> 
    <tr> 
     <td role="rowheader">Hide Status</td> 
     <td> <p>(Project and Task statuses only)</p> <p>Enable this option if you want the status hidden from users. When it is disabled (the default setting), all <draft-comment>
        <MadCap:conditionalText data-mc-conditions="SnippetConditions-wf-groups.system-level">
         users in the system
        </MadCap:conditionalText>
       </draft-comment><MadCap:conditionalText data-mc-conditions="SnippetConditions-wf-groups.system-level">
        users in the system
       </MadCap:conditionalText> can use the status.</p> <note type="tip">
       You can hide an Issue status by disabling all 4 issue types (Bug Report, Change Order, Issue, Request).
      </note> </td> 
    </tr> 
    <tr> 
     <td role="rowheader">Lock for all groups</td> 
     <td> <draft-comment>
       <p data-mc-conditions="SnippetConditions-wf-groups.system-level">If you leave this enabled, users throughout the system can see and use the status and <em>group administrators</em> cannot customize it for their groups.</p>
      </draft-comment><p data-mc-conditions="SnippetConditions-wf-groups.system-level">If you leave this enabled, users throughout the system can see and use the status and <em>group administrators</em> cannot customize it for their groups.</p> <draft-comment>
       <p data-mc-conditions="SnippetConditions-wf-groups.system-level">When this option is disabled, <em>group administrators</em> can customize the status for their individual groups.</p>
      </draft-comment><p data-mc-conditions="SnippetConditions-wf-groups.system-level">When this option is disabled, <em>group administrators</em> can customize the status for their individual groups.</p> <draft-comment>
       <p data-mc-conditions="SnippetConditions-wf-groups.system-level">For more information about locking statuses, see <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/lock-or-unlock-a-custom-system-level-status.md" class="MCXref xref">Locking or unlocking a custom system-level status</a>.</p>
      </draft-comment><p data-mc-conditions="SnippetConditions-wf-groups.system-level">For more information about locking statuses, see <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/lock-or-unlock-a-custom-system-level-status.md" class="MCXref xref">Locking or unlocking a custom system-level status</a>.</p> </td> 
    </tr> <draft-comment>
     <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
      <td role="rowheader"><span class="preview">Users can select this status only if required fields on the object are completed</span> </td> 
      <td> <p><span class="preview">(Applies only if you selected Tasks in Step 3) Assures that users can select this status for an object only if all required fields on the object are completed.</span> </p> <draft-comment>
        <p style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">This story is on the back burner</p>
       </draft-comment><p style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">This story is on the back burner</p> </td> 
     </tr>
    </draft-comment>
    <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
     <td role="rowheader"><span class="preview">Users can select this status only if required fields on the object are completed</span> </td> 
     <td> <p><span class="preview">(Applies only if you selected Tasks in Step 3) Assures that users can select this status for an object only if all required fields on the object are completed.</span> </p> <p style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">This story is on the back burner</p> </td> 
    </tr> 
   </tbody> 
  </table> </li> 
 <li value="7"> <p>Click <span class="bold">Save</span>.</p> </li> 
</ol>

`<li>For instructions on making this status a default status, see <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/use-custom-statuses-as-default-statuses.md" class="MCXref xref">Use custom statuses as default statuses</a>.</li>`  