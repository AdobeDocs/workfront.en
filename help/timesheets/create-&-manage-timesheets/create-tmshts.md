---
filename: create-tmshts
product-area: timesheets
navigation-topic: create-and-manage-timesheets
---




# Create Timesheets {#create-timesheets}

The following sections describe how timesheets are created in `Workfront`.


## Understand when Tasks and Issues appear on your Timesheet {#understand-when-tasks-and-issues-appear-on-your-timesheet}

A task or issue assigned to a user automatically appears on the timesheet of a user if the task or issue meets any of the following criteria:



* The user&nbsp;has logged hours on the task or issue
* The planned dates of the task or issue fall within the dates of timesheet
* The task or issue has an Actual Start Date (The task or issue status is In Progress)
* The task or issue is pinned to the timesheet
* The Planned Completion date falls within the date range of the timesheet and the status is In Progress


If the "Pre-populate timesheets..." preferences (located in the Timesheets preferences, as described in [Timesheet and hour preferences](timesheet-and-hour-preferences.md)) are&nbsp;deselected, the timesheet shows issues and tasks which have a status of In Progress.


## Create a Timesheet {#create-a-timesheet}

You can create a single-use timesheet, or the system administrator can create recurring timesheets by creating a timesheet profile.&nbsp;



* [Create a Timesheet Profile (Recommended)](#creating-a-timesheet-profile) 
* [Create a single-use Timesheet](#creating-a-single-use-timesheet) 




### Create a Timesheet Profile (Recommended) {#create-a-timesheet-profile-recommended}

For consistency in your system, we recommend that the system administrator create timesheets for users in the system by creating Timesheet Profiles. This is an automatic way of creating timesheets for users. 


For more information about Timesheet Profiles, see [Create Timesheet Profiles](create-timesheet-profiles.md).


### Create a single-use Timesheet {#create-a-single-use-timesheet}

You can manually create a single-use&nbsp;timesheet if you want a timesheet that is not recurring.&nbsp;When the end date of the timesheet is reached and more timesheets are needed, you need to create a new timesheet.&nbsp;


>[!NOTE]
>
>&nbsp;When creating a single-use timesheet, you cannot specify&nbsp;specific general hour types to include in your timesheet. All general hour types that are activated in your system display in timesheets created manually. If you want to select only certain general hour types to display in your timesheets, use a timesheet profile.&nbsp;For more information about timesheet profiles, see [Create Timesheet Profiles](create-timesheet-profiles.md).


To create a single-use timesheet:



1. Click the **Main Menu** icon ![](assets/main-menu-icon.png) in the upper-right corner of `Workfront`.

1. Click Timesheets.
1. Click All Timesheets in the left panel.
1.  Click **New Timesheet**.  

1. Specify the following information:  
   **Create timesheet for**: Start entering the name of the user for whom you are creating the timesheet, and click it when it appears&nbsp;in the list.  
   **Start Date:** This is the start date of the timesheet.  
   **End Date:** This is the end date of the timesheet.  
   **Approvers:&nbsp;**Approvers are&nbsp;users who approve the timesheet for the users associated with the timesheet. Only users with timesheet administrative rights can be set as approvers. For more information about timesheet administrative rights, see [Assign users administrative access](assign-users-administrative-access.md).  
   Start entering the names of the timesheet approvers and click them when they appear&nbsp;in the list.  
   You can have multiple approvers on a timesheet. In this case, after&nbsp;one of the approvers approves the timesheet, the timesheet is marked as **Closed** and it disappears from the timesheet approvals list of all the remaining approvers.  
   **Can edit time:** Select this option if you want to allow approvers to edit hours on the timesheet.&nbsp;

1. Click **Create Timesheet**.


