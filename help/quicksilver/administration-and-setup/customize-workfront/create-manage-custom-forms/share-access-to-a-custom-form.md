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
 <tbody> Adobe Workfront plan* Any 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Plan </p> </td> 
  </tr> Access level configurations* Administrative access to custom forms For information about how Workfront administrators grants this access, see Grant users administrative access to certain areas. 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access level configurations you have, contact your Workfront administrator.

## Access to custom forms

By default, when you create a new custom form and someone attaches it to an object, any user assigned to the object can view and fill out the form. This includes users with Request licenses and external users.

However, on an object where the custom form is not already attached, a user (even if they have a Planner access level) cannot attach it from the Custom Forms drop-down menu unless one of the following is true:

* Someone shared the custom form with the user or with their team, job role, group, or company, granting at least View permission with the Attach to Custom Data selected
* The user has a Plan license and their access level allows administrative access to custom forms

## Share a custom form

Rather than leaving a custom form in the default sharing state (described in [Access to custom forms](#access) in this article), you can configure specific levels of access to the form for certain users, job roles, groups, teams, and companies.

1. Click the `Main Menu` icon ![](assets/main-menu-icon.png) in the upper-right corner of Adobe Workfront, then click `Setup` ![](assets/gear-icon-settings.png).

1. In the left panel, click `Custom Forms`.
1. Select the custom form, then click `Share`.
1. In the box that displays, under `Give custom form access to`, start typing the name of the user, team, job role, group, or company you want to share the custom form with, then press `Enter` when the name displays.
1. To adjust access for the user, team, job role, group, or company you just added, click the drop-down menu to the right of the name, then configure one of the following available options and any of its advanced settings:

   <table cellspacing="0"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">View it</td> 
      <td> <p>Ability to view and fill out the custom form on objects.</p> <p>Note: For users with Work, Review, and Request licenses, this is the highest available option.</p> <p>Click <span class="bold">Advanced Settings</span> to specify whether you want to allow the following:</p> 
       <ul> 
        <li><span class="bold">Attach to custom data</span>: Ability to attach the custom form to projects, tasks, and issues for which they have Manage access</li> 
        <li> <p><span class="bold">Share</span>: Ability to share the custom form with others in the system</p> <p>Users with a Work, Review, or Request license can share a custom form only through the API or a custom forms report. For more information, see .</p> </li> 
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
   </table>

1. (Optional) Repeat Steps 4-5 to add other names to the list and configure their options.
1. (Optional) If you want to limit access to the custom form (on objects where it's attached) to those you have specified in the previous steps, click the gear icon ![](assets/gear-icon-settings-with-dn-arrow.jpg) in the upper right corner of the sharing box, then click `Remove system-wide access`.

   If you change your mind, you can click `Make this visible system-wide` (the default option).

   >[!NOTE]
   >
   >
   >  
   >  
   >  * When you make a custom form visible system-wide, you allow users only to see and fill it out on objects they are assigned to, not to attach it to other objects. You can grant the ability to attach the custom form to objects using the option "Attach to custom data" explained under step 5.
   >  * Most organizations want to ensure that everyone in the system can fill out a custom form when it's attached to objects they work on and view its data in reports. If this is true for your organization, we recommend that you use " `Make this visible system-wide`." When the option is configured this way, "Visible System-Wide" displays in the dialog box:
   >  
   >  
   >    ![](assets/visible-system-wide-350x480.png)   >  
   >  

   >  
   >  
   >    If you are concerned about a custom form where users might enter sensitive data when it is attached to certain objects, limiting sharing for those *objects* might be better rather than limiting access to the form itself.
   >  
   >  
   >

1. Click `Save`.

## Remove access to a custom form

1. Click the `Main Menu` icon ![](assets/main-menu-icon.png) in the upper-right corner of Adobe Workfront, then click `Setup` ![](assets/gear-icon-settings.png).

1. In the left panel, click `Custom Forms`.
1. Select the custom form, then click `Share`.
1. In the box that displays, click the X to the right of the name of the user, team, role, group, or company whom you no longer want to have special access to the form.
1. (Optional) Repeat the previous step to for other names you want to remove.
1. Click `Save`.

