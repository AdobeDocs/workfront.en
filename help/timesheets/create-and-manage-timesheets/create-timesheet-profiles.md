---
filename: create-timesheet-profiles
product-area: timesheets;system-administration
navigation-topic: create-and-manage-timesheets
---



# Create, edit, and assign timesheet profiles {#create-edit-and-assign-timesheet-profiles}

You can create, edit, and assign timesheet profiles that generate recurring timesheets for your users without any further intervention from you. This saves you time and ensures that the following are consistent between users:



* Timesheet time frame
* Approvers
* General hour types


For more information about creating a timesheet manually, see [Create a single-use timesheet](create-tmshts.md).


##  

## Access requirements {#access-requirements}

You must have the following to perform the steps in this article:

<table style="width: 100%;margin-left: 0;margin-right: auto;mc-table-style: url('../../Resources/TableStyles/TableStyle-List-options-in-steps.css');" class="TableStyle-TableStyle-List-options-in-steps" cellspacing="0"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2"> 
 <tbody> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader"><span class="mc-variable WFVariables.FullProdNameWF variable varname">Adobe Workfront</span> plan</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p>Any</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader"><span class="mc-variable WFVariables.FullProdNameWF variable varname">Adobe Workfront</span> license</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray"> <p><span class="mc-variable WFVariables.WFLicense-Plan variable varname">Plan</span> </p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-LightGray" role="rowheader">Access level configurations*</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-LightGray"> <p>You must have administrative access to timesheets. For more information, see <a href="grant-users-admin-access-certain-areas.md" class="MCXref xref" data-mc-variable-override="">Grant users administrative access to certain areas</a>.</p> <p data-mc-conditions="SnippetConditions.HIDE">Or, in order to work on <span class="mc-variable Snippet_Variables.Object variable varname">timesheet profiles</span> for a group, you must be an administrator of the group or a <span class="mc-variable WFVariables.AdminWF variable varname">Workfront administrator</span>. For more information, see <a href="group-administrators.md" class="MCXref xref" data-mc-variable-override="">Group administrators</a> and <a href="grant-a-user-full-administrative-access.md" class="MCXref xref" data-mc-variable-override="">Grant a user full administrative access</a>.</p> <p>Note: If you still don't have access, ask your <span class="mc-variable WFVariables.AdminWF variable varname">Workfront administrator</span> if they set additional restrictions in your access level. For information on how a <span class="mc-variable WFVariables.AdminWF variable varname">Workfront administrator</span> can modify your access level, see <a href="create-modify-access-levels.md" class="MCXref xref" data-mc-variable-override="">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your *`Workfront administrator`*.
{#access-requirements-you-must-have-the-following-to-perform-the-steps-in-this-article-adobe-workfront-plan-any-adobe-workfront-license-plan-access-level-configurations-you-must-have-administrative-access-to-timesheets-for-more-information-see-grant-users-administrative-access-to-certain-areas-or-in-order-to-work-on-timesheet-profiles-for-a-group-you-must-be-an-administrator-of-the-group-or-a-workfront-administrator-for-more-information-see-group-administrators-and-grant-a-user-full-administrative-access-note-if-you-still-dont-have-access-ask-your-workfront-administrator-if-they-set-additional-restrictions-in-your-access-level-for-information-on-how-a-workfront-administrator-can-modify-your-access-level-see-create-or-modify-custom-access-levels-to-find-out-what-plan-license-type-or-access-you-have-contact-your-workfront-administrator}



## Create or edit a timesheet profile {#create-or-edit-a-timesheet-profile}



>[!IMPORTANT] {type="important"}
>
>To enable timesheet profile changes in current timesheets, you have to delete the existing timesheets and then generate new ones. For instructions, see [Delete generated timesheets](delete-timesheets.md) and [Manually generate timesheets](manually-generate-timesheets.md).






1. Click the `Main Menu` icon ![](assets/main-menu-icon.png) in the upper-right corner of *`Adobe Workfront`*, then click `Setup` ![](assets/gear-icon-settings.png).

1.  If you are creating or editing a timesheet profile for use throughout the system, click `Timesheet & Hours`.


   Or


   If you creating or editing a timesheet profile for a group, click **Groups**, then click the group's name.

1.  Click **Timesheet Profiles**.
1.  To create a new timesheet profile, click `New Profile`.


   Or


   To edit an existing timesheet profile, select the timesheet profile you want to edit, then click `Edit`.  



   The new or existing timesheet profile displays.

1.  On the `Set Details` tab, type a `Name`and `Description`for the timesheet profile and supply the following information:



<table style="width: 100%;mc-table-style: url('../../Resources/TableStyles/TableStyle-List-options-in-steps.css');margin-left: 0;margin-right: auto;" class="TableStyle-TableStyle-List-options-in-steps" cellspacing="0"> 
 <col style="width: 456px;" class="TableStyle-TableStyle-List-options-in-steps-Column-Column1"> 
 <col style="width: 50%;" class="TableStyle-TableStyle-List-options-in-steps-Column-Column2"> 
 <tbody> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader"><span class="bold">Group with Administration Access</span> </td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p> 
     <ul> 
      <li> <p>If you are creating a system-level timesheet profile, leave this field blank.</p> <p>Any user who can edit user accounts can attach a system-level timesheet to other users.</p> <p>Only a <span class="mc-variable WFVariables.AdminWF variable varname">Workfront administrator</span> can edit a system-level timesheet profile.</p> </li> 
     </ul> 
     <ul> 
      <li> <p>If you are creating a timesheet profile for a group you administer, identify the group here.</p> <p>This does not assign the timesheet profile to the users in the group; it only allows the group’s administrators to modify the timesheet profile. You will assign the profile to users in Step 6.</p> <p>Note: When users outside the group are attaching timesheet profiles to other user, they won’t be able to see or attach this timesheet profile.</p> </li> 
     </ul> </p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader"><span class="bold">Create timesheets</span> </td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray"> <p> <p>Specify when the timesheet profile should generate the timesheets. A timesheet can be set to automatically generate on a weekly, bi-weekly, semi-monthly, or monthly basis. Select the day of the week when you want the timesheet to be produced.</p> <p>Note:  If you configure a timesheet profile to create timesheets on a Friday, users are not able to record hours on Friday, Saturday, and Sunday, for the current week.</p> <p><span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span> always creates two timesheets at a time: the first timesheet always includes the current date, and the second timesheet&nbsp;starts when the time frame of the first one ends.</p> </p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader"><span class="bold">Approvers</span> </td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p> <p>Approvers are&nbsp;users who approve the timesheet for the users associated with the timesheet. You can identify up to 7 users as approvers on a timesheet. Identifying multiple users is useful to ensure an approver is available when someone is out of the office. All approvers are notified when a user submits the timesheet for approval. Only one user is required to approve the timesheet in order for it to be approved.</p> <p>Only users with timesheet administrative rights can be set as approvers. For more information about timesheet administrative rights, see <a href="grant-users-admin-access-certain-areas.md" class="MCXref xref">Grant users administrative access to certain areas</a>.</p> <p>Use the drop-down menu&nbsp;to select&nbsp;the approver&nbsp;for the timesheet (if an approver is required). You can select from the following options:</p> 
     <ul> 
      <li><span class="bold">None</span>: The timesheet does not need to&nbsp;be approved.</li> 
      <li><span class="bold">Their Manager</span>: This is the default approver, set by the system. In this case, the user designated as their manager approves the timesheet when it is submitted for approval.</li> 
      <li><span class="bold">Specific People:</span>&nbsp;You can designate specific users, by name, as timesheet approvers. You can have multiple approvers on a timesheet. In this case, after&nbsp;one of the approvers approves the timesheet, the timesheet is marked as <span class="bold">Closed</span> and it disappears from the timesheet approvals list of all the remaining approvers.</li> 
     </ul> </p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader"><span class="bold">Can edit hours</span> </td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray"> <p> <p>Select this option to allow the approvers to edit hours on the timesheet. If Restrict timesheet editing to owners and admins is enabled in Timesheet &amp; Hours &gt; Preferences, you can't enable this setting. </p> <p>Note: Once you submit a timesheet for approval, you can no longer edit the hours. To return a submitted timesheet to an editable state, recall the timesheet or have the approver reject the timesheet. For more information, see <a href="submit-timesheet-for-approval.md" class="MCXref xref">Submit a timesheet for approval</a> and<a href="timesheet-approvals.md" class="MCXref xref">Approve a timesheet</a>.</p> </p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader"><span class="bold">Available Hour Types</span> </td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray">By default, users see all general hours on a timesheet. However, if your organization wants only specific general hours to be shown for a particular set of users, you can select the general hours that they need to see in their timesheets by&nbsp;selecting them in their timesheet profile in this field. If you want to disable all general hours, deselect&nbsp;all hour types to generate the timesheet without a section for general hours.</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray" data-mc-conditions=""> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-MediumGray" role="rowheader"><span style="font-weight: bold;">Overtime</span> </td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-MediumGray">You can choose to hide the Overtime box in timesheets. This option is disabled by default.</td> 
  </tr> 
 </tbody> 
</table>



1.  Click the `Assign People` tab to associate the timesheet profile with specific users, groups, or (if you are a *`Workfront administrator`*) teams. Begin typing the name of the user, group, or team, then click it when it appears in the drop-down list.


   If you are a *`group administrator`*, you can assign the timesheet profile to groups you administer, but not to teams. For more information, see [Limitations for a group administrator assigning a timesheet profile](#possible) in this article.


   >[!NOTE]
   >
   >
   >    
   >    
   >    *  You can also associate a user with a timesheet profile by editing the user profile. For more information, see [Edit a user's profile](edit-a-users-profile.md).
   >    * When you add a group, only the group name appears on the Assign People tab, not the list of group members. If you want to see the group members listed here, click Save Changes, then click the name of the timesheet profile you just created.
   >    * When you finish these steps, the timesheet profile generates timesheets only for the assigned users or group members who don’t have existing timesheets for the current period.
   >    
   >    




1.  Click`<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">  <span class="bold">Save Changes</span></MadCap:conditionalText>`.


   The first time the timesheet profile generates timesheets, 2 timesheets are created for each user. After that, each time it generates new timesheets, onhe timesheet is created per user. 





## Limitations for a *`group administrator`* assigning a timesheet profile {#limitations-for-a-group-administrator-assigning-a-timesheet-profile}

If you are a *`group administrator`* and the administrative access option Timesheets & hours is disabled in your access level, you can create timesheet profiles, but you can assign them only to:



* Groups you administer 
*  Individual users you have access to edit who are in a group you administer 


For these groups and users, you won’t have access to the timesheets that the timesheet profile generates.


Further, if the option User Admin (Group Users) is also disabled in your access level, you can assign the timesheet profile to a group you administer, but it affects only the users in the group that you have access to edit. If the group contains users that you don’t have access to edit, they are not assigned the timesheet profile along with the rest of the group.


For information about the option Timesheets & hours in your access level, see [Grant users administrative access to certain areas](grant-users-admin-access-certain-areas.md).


For information about the option User Admin (Group Users) in your access level, see [Grant access to users](grant-access-other-users.md).


## Multiple recurring timesheet profiles {#multiple-recurring-timesheet-profiles}

You can have more than one timesheet profile for your organization if there are:



* Unique pay periods for different sets of users
* Unique approvers for different sets of users
* Unique general hours requirements for different sets of users


One user cannot be associated with more than one timesheet profile at a time.&nbsp;
