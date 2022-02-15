---
filename: create-timesheet-profiles
product-area: timesheets;system-administration
navigation-topic: create-and-manage-timesheets
---




# Create Timesheet Profiles {#create-timesheet-profiles}



## Understand Timesheet Profiles {#understand-timesheet-profiles}

As&nbsp;a system administrator, you can define recurring timesheet profiles and associate them with users.  
As a group administrator, you can define recurring timesheet profiles for the groups you administer and associate them with users in your groups.&nbsp;


For more information about Group Administrators, see the "Understanding Group Administrators" section in [Create and manage groups](create-manage-groups.md).


Although you can manually create individual timesheets for users, we recommend that you use recurring timesheet profiles associated with users to generate timesheets automatically. For more information about creating a timesheet manually, see [Create Timesheets](create-tmshts.md).


Recurring timesheets allow you to program `Workfront` to automatically create a weekly, bi-weekly, or monthly&nbsp;timesheet for your users, without any further intervention from you.


`Workfront` automatically creates two timesheets&nbsp;based on the specifications of the recurring timesheet profile. The first timesheet always includes the current date in the timeframe of the timesheet.&nbsp;


By using a timesheet profile, you can ensure the following are consistent between users:&nbsp;



* Timesheet timeframe
* Approvers
* General hour types




## Access needed to create a Timesheet Profile {#access-needed-to-create-a-timesheet-profile}

To be able to create a Timesheet Profile, assign it to users, and generate timesheets manually, you must have the following access:



* System Administrator.
* Group Administrator with administrative access to Timesheet & Hours.  
  For more information about granting administrative access in a user's Access Level, see [Assign users administrative access](assign-users-administrative-access.md).  
  For more information about Group Administrators, see the "Understanding Group Administrators" section in&nbsp; [Create and manage groups](create-manage-groups.md).





## Create or Edit a Timesheet Profile {#create-or-edit-a-timesheet-profile}

You can create a new timesheet profile, or edit an existing one. You might want to edit an existing timesheet profile when a change occurs, such as the user designated as an approver on a timesheet changes and you need to reflect that change `.`


To create or edit a timesheet profile:



1. Click the **Main Menu** icon ![](assets/main-menu-icon.png) in the upper-right corner of `Workfront`, then click **Setup** ![](assets/setup-gear-icon.png).

1. Expand **Timesheet & Hours**,&nbsp;then click **Timesheet&nbsp;Profiles**.  

1.  To create a new timesheet profile, click **New Profile**.


   Or


   To edit an existing timesheet profile, select the timesheet profile you want to edit, then click **Edit**.  
   The new or existing timesheet profile is displayed.

1.  Specify the following information in the** Set Details** tab:



<table style="width: 100%;mc-table-style: url('../../Resources/TableStyles/TableStyle-List-options-in-steps.css');" class="TableStyle-TableStyle-List-options-in-steps" cellspacing="0"> 
 <col style="width: 456px;" class="TableStyle-TableStyle-List-options-in-steps-Column-Column1"> 
 <col style="width: 50%;" class="TableStyle-TableStyle-List-options-in-steps-Column-Column2"> 
 <thead> 
  <tr> 
   <th class="TableStyle-TableStyle-List-options-in-steps-HeadH-Column1-">&nbsp;</th> 
   <th class="TableStyle-TableStyle-List-options-in-steps-HeadG-Column2-">&nbsp;</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray"><b>Name</b> </td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p> Specify a name for the timesheet profile.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray"><b>Description</b> </td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray"> <p> Provide a description for the timesheet profile.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray"><b>Group with Administration Access</b> </td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p> <p>Indicate the group whose Group Administrator has the permission to edit this Timesheet Profile. The Group Administrator of the group specified here can&nbsp;modify the Timesheet Profile.&nbsp;</p> <p>Important:  <p>When a group administrator creates a Timesheet Profile, this field is mandatory. A group administrator can create a Timesheet Profile only designated for a specific administrative group for which they are designated as the administrator. The Timesheet Profile created for a specific group is not visible to users that do not belong to the Group specified here when they attach a Timesheet Profile to a user they have access to edit.&nbsp;</p> <p>For more information about editing users, see&nbsp;<a href="edit-a-users-profile.md" class="MCXref xref">Edit a user's profile</a>.</p> <p> This field is optional when System Administrators create a Timesheet Profile. They can create a system-level Timesheet Profile when they do not associate it with a specific administrative group. The system-level Timesheet Profiles are visible to select to all users who can edit user accounts. Only the System Administrator can edit system-level Timesheet Profiles.&nbsp;</p> </p> <p>Specifying a&nbsp;<b>Group with Administration Access</b>&nbsp;for a Timesheet Profile does not assign the profile to the users in the group. Specifying a <b>Group with Administration Access</b> only allows the Group Administrator of the group to modify the Timesheet Profile.</p> <p>For more information about Group Administrators, see the "Understanding Group Administrators" section in&nbsp;<a href="create-manage-groups.md" class="MCXref xref">Create and manage groups</a>.</p> </p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray"><b>Create timesheets</b> </td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray"> <p> <p>&nbsp;Specify when the timesheet profile should generate the timesheets. A timesheet can be set to automatically generate on a weekly, bi-weekly, semi-monthly, or monthly basis. Select the day of the week when you want the timesheet to be produced.</p> <p>Note: &nbsp;If you configure a timesheet profile to create timesheets on a Friday, users are not able to record hours on Friday, Saturday, and Sunday, for the current week.</p> <p><span class="WFVariablesProdNameWF">Workfront</span> always creates two timesheets at a time: the first timesheet always includes the current date, and the second timesheet&nbsp;starts when the timeframe of the first one ends.</p> </p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray"><b>Approvers</b> </td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p> <p>&nbsp;Approvers are&nbsp;users who approve the timesheet for the users associated with the timesheet. You can identify up to 7 users as approvers on a timesheet. Identifying multiple users is useful to ensure an approver is available when someone is out of the office. All approvers are notified when a user submits the timesheet for approval. Only one user is required to approve the timesheet in order for it to be approved.</p> <p>Only users with timesheet administrative rights can be set as approvers. For more information about timesheet administrative rights, see <a href="assign-users-administrative-access.md" class="MCXref xref">Assign users administrative access</a>.</p> <p>Use the drop-down menu&nbsp;to select&nbsp;the approver&nbsp;for the timesheet (if an approver is required). You can select from the following options:</p> 
     <ul> 
      <li value="1"><b>None</b>: The timesheet does not need to&nbsp;be approved.</li> 
      <li value="2"><b>Their Manager</b>: This is the default approver, set by the system. In this case, the user designated as their manager approves the timesheet when it is submitted for approval.</li> 
      <li value="3"><b>Specific People:</b>&nbsp;You can designate specific users, by name, as timesheet approvers. You can have multiple approvers on a timesheet. In this case, after&nbsp;one of the approvers approves the timesheet, the timesheet is marked as <b>Closed</b> and it disappears from the timesheet approvals list of all the remaining approvers.</li> 
     </ul> </p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray"><b>Can edit hours</b> </td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray"> <p> <p>Select this option to allow the approvers to edit hours on the timesheet.</p> <p>Note: Once you submit a timesheet for approval, you can no longer edit the hours. To return a submitted timesheet to an editable state, recall the timesheet or have the approver reject the timesheet. For more information, see <a href="timesheet-approvals.md" class="MCXref xref">Timesheet Approvals</a>.</p> </p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-LightGray"><b>Available Hour Types</b> </td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-LightGray">By default, users see all general hours on a timesheet. However, if your organization wants only specific general hours to be shown for a particular set of users, you can select the general hours that they need to see in their timesheets by&nbsp;selecting them in their timesheet profile in this field. If you want to disable all general hours, deselect&nbsp;all hour types to generate the timesheet without a section for general hours.</td> 
  </tr> 
 </tbody> 
</table>



1.  Click the **Assign People** tab to associate the timesheet with specific users, groups, or teams. Begin typing the name of the person, team, or group, then click it when it appears in the drop-down list.


   >[!NOTE]
   >
   >Group Administrators can only assign Timesheet Profiles to groups they manage, or users they can edit. Group Administrators cannot assign Timesheet Profiles to teams. If **Timesheets & hours** is not enabled in their Access Level, Group Administrators cannot assign Timesheet Profiles, although they can create them.  

   >
   >
   >For more information about enabling Timesheets & hours administrative access in a user's Access Level, see [Assign users administrative access](assign-users-administrative-access.md).
   >
   >
   >If the User Admin (All Users) setting is not enabled in their Access Level, Group Administrators cannot assign groups to Timesheet Profiles, they can only assign them to users they can edit.&nbsp;
   >
   >
   >For more information about the access needed to edit users, see [Grant access to users](grant-access-other-users.md).




1. Click`<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">  <b>Save</b>.</MadCap:conditionalText>`




## Associate a Timesheet Profile with an existing user {#associate-a-timesheet-profile-with-an-existing-user}

You can assign a timesheet profile to users or groups as part of creating the timesheet profile.  



If you are a system administrator, you can also assign a timesheet profile to teams.&nbsp;


For more information about assigning users, teams, or groups with a timesheet profile, see [Create or Edit a Timesheet Profile](#creating-a-timesheet-profile).


You can also associate a user with a timesheet profile by editing the user profile. 


For more information about editing the profile of a user and associating a timesheet profile with them, see [Edit a user's profile](edit-a-users-profile.md).


## Multiple recurring Timesheet Profiles {#multiple-recurring-timesheet-profiles}

You can have more than one timesheet profile for your organization if there are:



* Unique pay periods for different sets of users.&nbsp;
* Unique approvers for different sets of users.
* Unique general hours requirements for different sets of users.


One user cannot be associated with more than one timesheet profile at a time.&nbsp;


## Delete and manually generating Timesheets {#delete-and-manually-generating-timesheets}

Anyone with administrative access to Timesheets in their Access Level can create or delete them.  
Only a system or group administrator can manually generate timesheets.  




* [Delete Timesheets](#deleting-timesheets) 
* [Manually generating Timesheets](#manually-generating-timesheets) 




### Delete Timesheets {#delete-timesheets}

The changes you make to a timesheet profile are not effective right away for the currently existing timesheets. For more information about editing existing timesheet profiles, see [Create or Edit a Timesheet Profile](#creating-a-timesheet-profile).


To make the changes visible on existing timesheets, you must&nbsp;delete the timesheets that have been generated, and generate new timesheets. This applies only to timesheets that have been generated by associating timesheet profiles with users. For more information about manually generating timesheets, see [Manually generating Timesheets](#manually-generating-timesheets).


>[!NOTE]
>
>When you delete timesheets, the hours logged against tasks, issues, and projects are not deleted. Only the General Hours are deleted with the timesheet. In a separate text editor, write down&nbsp;what General Hours are associated with the timesheet. After the timesheet is deleted, you can then log them in the new timesheet. 




>[!IMPORTANT] {type="important"}
>
>We recommend that you do not delete past timesheets because they are not generated automatically based on timesheet profiles. You can delete the current and future timesheets and generate them manually if you want the changes to your timesheet profiles to be immediately visible in the new timesheets. 


To delete timesheets:



1. Click the **Main Menu** icon ![](assets/main-menu-icon.png) in the upper-right corner of `Workfront`.

1. Click Timesheets.
1. Click All Timesheets in the left panel.
1.  Using the filters on the left side, filter for the timesheets you want to delete.


   You can filter timesheets by the following criteria:

    
    
    * User name, their team or job role
    * Approver name
    * Timesheet Status
    * Time Period of the timesheet
    
    

1. Select all timesheets that you want to delete and click **Delete**.
1.  Click **Yes, Delete it**.


   This deletes the timesheet. You cannot recover a deleted timesheet.&nbsp;





### Manually generating Timesheets {#manually-generating-timesheets}

To enable changes that you made to the timesheet profiles to reflect&nbsp;in current timesheets, you have to first delete the existing timesheets and then generate new ones. 


For more information about deleting timesheets, see [Delete Timesheets](#deleting-timesheets).


>[!NOTE]
>
>Only a system or group administrator can manually generate timesheets.


When you manually generate timesheets, the timesheets are generated according to the Timesheet Profiles that are associated with your users. Users who do not have Timesheet Profiles associated with them will not receive timesheets when you manually generate timesheets.&nbsp;


When you manually generate timesheets, only the current timesheet and the one to follow are generated. `Workfront` does not generate two timesheets for the same period. If you already have a timesheet for a specific timeframe, another one will not generate when you are using the manual process to generate timesheets.&nbsp;


You can manually generate timesheets from either of the following areas:


#### **From the Diagnostics Area**  {#from-the-diagnostics-area}




1. Click the **Main Menu** icon ![](assets/main-menu-icon.png) in the upper-right corner of `Workfront`, then click **Setup** ![](assets/setup-gear-icon.png).

1. Expand **System**, then click **Diagnostics**.

1. Click **Conduct Diagnostics**.&nbsp;
1. Click **Generate Timesheets**.




#### **From the Timesheets area**  {#from-the-timesheets-area}




1. Click the **Main Menu** icon ![](assets/main-menu-icon.png) in the upper-right corner of `Workfront`, then click **Setup** ![](assets/setup-gear-icon.png).

1. Expand **Timesheets & Hours**, then click **Timesheet Profiles**.

1.  Click **More**, then **Generate Timesheets**.&nbsp;


   New timesheets are created for up to two periods of time for users associated with Timesheet Profiles.



