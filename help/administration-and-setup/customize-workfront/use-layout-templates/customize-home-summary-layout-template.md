---
filename: customize-home-summary-layout-template
title: Customize Home using a Layout Template
user-type: administrator
product-area: system-administration;templates;setup
navigation-topic: layout-templates
title: Customize Home and Summary using a layout template
description: You can use a Layout Template to configure what users see when they click a task or issue in Home and in the Summary. Each configuration you make using the steps below affects the Home area and the Summary panel in the same way. These customizations don't apply to the Document Summary panel.
---

# Customize Home and Summary using a layout template

You can use a Layout Template to configure what users see when they click a task or issue in Home and in the Summary. Each configuration you make using the steps below affects the Home area and the Summary panel in the same way. These customizations don't apply to the Document Summary panel.

You can configure:

* What fields display for a task or issue in the Details area, and in what order
* Whether updates, logged time, attached documents, and timestamps display for a selected task or issue

You can also customize the fields that users see in the Home area when users click a project approval, document approval, or document version approval that is assigned to them.

For information about the Home area, see [Use the Home area](../../../workfront-basics/using-home/using-the-home-area/use-the-home-area.md).For information about the Summary panel, see Summary overview in the new Adobe Workfront experience.

For information about layout templates for groups, see [Create and modify a group’s layout templates](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-layout-templates.md).

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

## Customize Home and Summary using a layout template

<ol> 
 <li value="1">Begin working on a layout template, as described in <a href="../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md" class="MCXref xref">Create and manage layout templates</a>.</li> 
 <li value="2">Click the down arrow <img src="assets/dropdown-arrow.png"> under <span class="bold">Customize what users see</span>, then click <span class="bold">Home</span><span class="bold"> and Summary</span>.</li> 
 <li value="3"> <p>In the list that appears on the left, click the object type (<span class="bold">Tasks</span>, <span class="bold">Issues</span>,<span class="bold">Projects</span>, <span class="bold">Documents</span>, or <span class="bold">Document Versions</span>) that you want to customize in Home and Summary.</p> 
  <table cellspacing="0"> 
   <col> 
   <col> 
   <tbody> 
    <tr> 
     <td role="rowheader">Tasks</td> 
     <td> <p>In Home, your configuration for this setting affects the area to the right of a task when a user clicks the task. And, in a list of tasks, it affects the Summary panel that displays on the right side of the page when a user selects a task, then clicks the Open Summary icon <img src="assets/summary-panel-icon.png">.</p> <p>For example, you can determine which fields users see in the Details area when users select tasks in Home:</p> <p> <img src="assets/home-details-adobe-branding-350x192.jpg" style="width: 350;height: 192;"> </p> <p>And when they select tasks in the Summary:</p> <p> <img src="assets/summary-details-350x219.jpg" style="width: 350;height: 219;"> </p> </td> 
    </tr> 
    <tr> 
     <td role="rowheader">Issues</td> 
     <td> <p>In Home, your configuration for this setting affects the area to the right of an issue when a user clicks the issue.</p> <p>In a list of issues, this setting affects the Summary panel that displays on the right side of the page when a user selects an issue, then clicks the Open Summary icon <img src="assets/summary-panel-icon.png">.</p> </td> 
    </tr> 
    <tr> 
     <td role="rowheader">Projects</td> 
     <td>In Home, when a user clicks a project approval assigned to them, your configuration for this setting affects the area to the right of the approval.</td> 
    </tr> 
    <tr> 
     <td role="rowheader">Documents</td> 
     <td>In Home, when a user clicks a document approval assigned to them, your configuration for this setting affects the area to the right of the approval.</td> 
    </tr> 
    <tr> 
     <td role="rowheader">Document Versions</td> 
     <td>In Home, when a user clicks an approval assigned to them for a particular version of a document, your configuration for this setting affects the area to the right of the approval.</td> 
    </tr> 
   </tbody> 
  </table> <note type="important">
   If a task is unassigned, the user assigned to the layout template will not see the field customizations in the Summary.
  </note> </li> 
 <li value="4"> <p>(Conditional) If you clicked Tasks or Issues in the previous step, click the category of task or issue that you want to customize.</p> <p> <img src="assets/choose-cat-cstmz-nwe-adobe-branding-350x254.png" style="width: 350;height: 254;"> </p> </li> 
 <li value="5"> <p>(Conditional) If the <span class="bold">Set primary action button</span> drop-down menu appears (if you select <span class="bold">Tasks</span> or <span class="bold">Issues</span> in the list on the left), click the primary action (<span class="bold">Done</span> or <span class="bold">Status</span>) that you want available for users in the Home area and in the Summary panel when they view a task or an issue.</p> <p> <img src="assets/set-primary-action-button-dropdown-pdf-adobe-branding-350x223.png" style="width: 350;height: 223;"> </p> </li> 
 <li value="6"> <p>Add <img src="assets/add-item-plus-in-circle-blue.png"> or hide <img src="assets/close-or-hide---x.png"> fields for the selected object type.</p> <p> <img src="assets/lt-home-add-hide-fields-adobe-branding-350x302.png" style="width: 350;height: 302;"> </p> </li> 
 <li value="7">Repeat steps 3-6 to customize Home area and the Summary panel for any other object types.</li> 
 <li value="8"> <p>Click <span class="bold">Global settings</span>, near the lower left corner, then enable or disable any of the following options related to <span>Adobe Workfront</span> objects in Home and Summary:</p> 
  <table cellspacing="0"> 
   <col> 
   <col> 
   <tbody> 
    <tr> 
     <td role="rowheader">Show updates for work</td> 
     <td>Displays any updates made on a selected task or issue in Home or Summary. This includes both system updates and updates made by a user. Users can still filter out system updates, as described in <a href="../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md#enable" class="MCXref xref">Enable or disable system updates</a> in <a href="../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md" class="MCXref xref">Update work</a>.</td> 
    </tr> 
    <tr> 
     <td role="rowheader">Log time against work</td> 
     <td>Displays the Log time against work option when a task or issue is selected, allowing users to log time on work items directly from the Home and Summary areas.</td> 
    </tr> 
    <tr> 
     <td role="rowheader">View documents associated with work</td> 
     <td>Displays a Documents area in Home and Summary when a task or issue is selected, listing any documents attached to the task or issue. Users can click documents to view them in a preview window.</td> 
    </tr> 
    <tr> 
     <td role="rowheader">Hide timestamp</td> 
     <td>Hides timestamps for the following date fields in Home and Summary:
      <ul>
       <li>Planned Completion Date</li>
       <li>Commit Date</li>
       <li><p>Submitted Date</p></li>
      </ul><note type="note">
        When this option is enabled, work items that become past due are moved to the Late grouping in the Home Work List based on date only, not time.
      </note></td> 
    </tr> 
   </tbody> 
  </table> </li> 
 <li value="9"> <p>Continue customizing the layout template.</p> <p>Or</p> <p>If you are finished customizing, click <span class="bold">Save</span>.</p> </li> 
</ol>

For more information about layout templates, see [Create and manage layout templates](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).
