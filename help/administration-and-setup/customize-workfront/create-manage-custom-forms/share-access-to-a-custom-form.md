---
filename: share-access-to-a-custom-form
title: Share a Custom Form
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
title: Share a custom form
description: You can configure access for a custom form to control who—person, role, group, team, company—can view, share, and edit it.
---

# Share a custom form

You can configure access for a custom form to control who—person, role, group, team, company—can view, share, and edit it.

## Access requirements

You must have the following to perform the steps in this article:

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> <draft-comment>
   <tr data-mc-conditions=""> 
    <td role="rowheader"> <p><em>Adobe Workfront</em> plan*</p> </td> 
    <td>Any</td> 
   </tr>
  </draft-comment>
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p><em>Adobe Workfront</em> plan*</p> </td> 
   <td>Any</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><em>Adobe Workfront</em> license*</td> 
   <td> <p><em>Plan</em> </p> </td> 
  </tr> <draft-comment>
   <tr data-mc-conditions=""> 
    <td role="rowheader">Access level configurations*</td> 
    <td> <p>Administrative access to custom forms</p> <p>For information about how <em>Workfront administrators</em> grants this access, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref" data-mc-variable-override="">Grant users administrative access to certain areas</a>.</p> </td> 
   </tr>
  </draft-comment>
  <tr data-mc-conditions=""> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Administrative access to custom forms</p> <p>For information about how <em>Workfront administrators</em> grants this access, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref" data-mc-variable-override="">Grant users administrative access to certain areas</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access level configurations you have, contact your *Workfront administrator*.

## Access to custom forms

By default, when you create a new custom form and someone attaches it to an object, any user assigned to the object can view and fill out the form. This includes users with *Request* licenses and external users.

However, on an object where the custom form is not already attached, a user (even if they have a Planner access level) cannot attach it from the Custom Forms drop-down menu unless one of the following is true:

* Someone shared the custom form with the user or with their team, job role, group, or company, granting at least View permission with the Attach to Custom Data selected
* The user has a *Plan* license and their access level allows administrative access to custom forms

## Share a custom form

Rather than leaving a custom form in the default sharing state (described in [Access to custom forms](#access) in this article), you can configure specific levels of access to the form for certain users, job roles, groups, teams, and companies.

<ol> 
 <li value="1">Click the <span class="bold">Main Menu</span> icon <img src="assets/main-menu-icon.png"> in the upper-right corner of <em>Adobe Workfront</em>, then click <span class="bold">Setup</span> <img src="assets/gear-icon-settings.png">.</li> 
 <li value="2">In the left panel, click <span class="bold">Custom Forms</span>.</li> 
 <li value="3"> <p>Select the custom form, then click <span class="bold">Share</span>.</p> </li> 
 <li value="4"> <p>In the box that displays, under <span class="bold">Give <em>custom form</em> access to</span>, start typing the name of the user, team, job role, group, or company you want to share the <em>custom form</em> with, then press <span class="bold">Enter</span> when the name displays.</p> </li> 
 <li value="5"> <p>To adjust access for the user, team, job role, group, or company you just added, click the drop-down menu to the right of the name, then configure one of the following available options and any of its advanced settings:</p> 
  <table cellspacing="0"> 
   <col> 
   <col> 
   <tbody> 
    <tr> 
     <td role="rowheader">View it</td> 
     <td> <p>Ability to view and fill out the custom form on objects.</p> <note type="note">
       For users with 
       <em>Work</em>, 
       <em>Review</em>, and 
       <em>Request</em> licenses, this is the highest available option.
      </note> <p>Click <span class="bold">Advanced Settings</span> to specify whether you want to allow the following:</p> 
      <ul> 
       <li><span class="bold">Attach to custom data</span>: Ability to attach the custom form to projects, tasks, and issues for which they have Manage access</li> 
       <li> <p><span class="bold">Share</span>: Ability to share the custom form with others in the system</p> <p>Users with a <em>Work</em>, <em>Review</em>, or <em>Request</em> license can share a custom form only through the API or a custom forms report. For more information, see .</p> </li> 
      </ul> </td> 
    </tr> 
    <tr> 
     <td role="rowheader">Manage it</td> 
     <td> <p>Available only for users with a Plan license. </p> <p>In addition to being able to add the form to objects they have access to edit, users can also fully edit the custom form, including adding, editing, and deleting fields.</p> <p>Click <span class="bold">Advanced Settings</span> to specify whether you want to allow following:</p> 
      <ul> 
       <li> <p><span class="bold">Attach to custom data</span>: Ability to attach the custom form to projects, tasks, and issues for which they have Manage access</p> </li> 
       <li><span class="bold">Delete</span>: Delete the custom form from the system</li> 
       <li><span class="bold">Share</span>: Share the custom form with others in the system</li> 
      </ul> </td> 
    </tr> 
   </tbody> 
  </table> </li> 
 <li value="6">(Optional) Repeat Steps 4-5 to add other names to the list and configure their options.</li> 
 <li value="7"> <p>(Optional) If you want to limit access to the custom form (on objects where it's attached) to those you have specified in the previous steps, click the gear icon <img src="assets/gear-icon-settings-with-dn-arrow.jpg"> in the upper right corner of the sharing box, then click <span class="bold">Remove system-wide access</span>.</p> <p>If you change your mind, you can click <span class="bold">Make this visible system-wide</span> (the default option).</p> <note type="note"> 
   <ul> 
    <li> <p>When you make a custom form visible system-wide, you allow users only to see and fill it out on objects they are assigned to, not to attach it to other objects. You can grant the ability to attach the custom form to objects using the option "Attach to custom data" explained under step 5.</p> </li> 
    <li> <p>Most organizations want to ensure that everyone in the system can fill out a custom form when it's attached to objects they work on and view its data in reports. If this is true for your organization, we recommend that you use "<span class="bold" style="font-weight: normal;">Make this visible system-wide</span>." When the option is configured this way, "Visible System-Wide" displays in the dialog box:</p> <p> <img src="assets/visible-system-wide-350x480.png" style="width: 350;height: 480;"> </p> <p>If you are concerned about a custom form where users might enter sensitive data when it is attached to certain objects, limiting sharing for those <i>objects</i> might be better rather than limiting access to the form itself.</p> </li> 
   </ul> 
  </note> </li> 
 <li value="8">Click <span class="bold">Save</span>.</li> 
</ol>

## Remove access to a custom form

<ol> 
 <li value="1">Click the <span class="bold">Main Menu</span> icon <img src="assets/main-menu-icon.png"> in the upper-right corner of <em>Adobe Workfront</em>, then click <span class="bold">Setup</span> <img src="assets/gear-icon-settings.png">.</li> 
 <li value="2">In the left panel, click <span class="bold">Custom Forms</span>.</li> 
 <li value="3"> <p>Select the custom form, then click <span class="bold">Share</span>.</p> </li> 
 <li value="4"> <p>In the box that displays, click the X to the right of the name of the user, team, role, group, or company whom you no longer want to have special access to the form.</p> </li> 
 <li value="5">(Optional) Repeat the previous step to for other names you want to remove.</li> 
 <li value="6">Click <span class="bold">Save</span>.</li> 
</ol>

