---
filename: add-activities-to-goals
product: workfront-goals
product-area: projects
navigation-topic: results-and-activities
title: Add activities to goals in Adobe Workfront Goals
description: Activities measure the progress of a goal. Without associated results, activities, or aligned goals, a goal cannot be activated and progress cannot be recorded on it.
---

# Add activities to goals in&nbsp;Adobe Workfront Goals

Activities measure the progress of a goal. Without associated results, activities, or aligned goals, a goal cannot be activated and progress cannot be recorded on it.

## Access requirements

You must have the following:

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Pro or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Request or higher</p> <p>For more information, see <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront licenses overview</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td> <p>You must purchase an additional license for the Adobe Workfront Goals to access functionality described in this article. </p> <p>For information, see <a href="../../workfront-goals/goal-management/access-needed-for-wf-goals.md" class="MCXref xref">Requirements to use Adobe Workfront Goals</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Goals or higher</p> <p>Note:   <p>If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see:</p> 
     <ul> 
      <li> <p><a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a> </p> </li> 
      <li> <p><span href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md"><a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md" class="MCXref xref">Grant access to Adobe Workfront Goals</a></span> </p> </li> 
     </ul> </p> </td> 
  </tr> Object permissions Manage permissions to the goal For information about sharing goals, see Share a goal in Adobe Workfront Goals. 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your Workfront administrator.

## Prerequisites

You must have the following before you can start:

* A Layout Template that includes the Goals area in the Main&nbsp;Menu.
* An existing goal.

  For information about creating goals, see [Create goals in Adobe Workfront Goals](../../workfront-goals/goal-management/create-goals.md).

>[!IMPORTANT]
>
>A goal cannot have more than a total of 50 activities, results, or aligned goals.

For more information about activities, see [Get started with results and activities in Adobe Workfront Goals](../../workfront-goals/results-and-activities/get-started-with-results-and-activities.md).

## Add an activity to a goal

<ol> 
 <li value="1">Go to the goal for which you want to add an activity and click the name to open the <span class="bold">Goal&nbsp;Details</span> panel.</li> 
 <li value="2"> <p>Click <span class="bold">Add activities</span>.</p> <p> <img src="assets/add-activity-inside-goal-details-highlighted-350x152.png" style="width: 350;height: 152;"> </p> </li> 
 <li value="3"> <p>From the <span class="bold">Activity Type</span> drop-down menu, select the type of activity you want to associate with your goal.&nbsp;Select <span class="bold">Manual progress bar</span> or <span class="bold">Project</span>. Manual progress bar is the default selection. </p> </li> 
 <li value="4">(Conditional) Depending on which activity type you selected, do the following: 
  <ol> 
   <li value="1">If you selected Manual progress bar: 
    <ol> 
     <li value="1">Start typing a name for your activity in the <span class="bold">Activity</span> field. </li> 
     <li value="2"><p>(Optional) If you want to set the activity owner as someone other than yourself, click your name in the <span class="bold">Owner</span> field and begin typing the name of the user that you want to assign as the activity owner, then click it when it appears in the drop-down list.</p><note type="note">
       You cannot assign a team or group as an activity owner.
      </note><p>When you update the progress of an activity, the progress of the goal automatically updates. </p></li> 
    </ol></li> 
   <li value="2">If you selected <span class="bold">Project</span>: 
    <ol> 
     <li value="1"><p>&nbsp;Click the <span class="bold">Connect projects</span> field.</p><p>Existing projects that you have access to View display in the Connect projects list. Projects that are in a status of Dead do not display in the list. </p></li> 
     <li value="2"><p>&nbsp;Click the name of a project to add it as an activity to the goal. You can select several projects at one time.</p><p>Workfront uses the project percent complete of all the attached projects to calculate the progress of the goal. </p><p>For more information about associating projects with goals, see <a href="../../workfront-goals/results-and-activities/connect-projects-to-goals-overview.md" class="MCXref xref">Overview of connecting projects to goals in Adobe Workfront Goals</a>.</p> 
      <div class="tips" data-mc-autonum="<b>Tips: </b>"> <span class="autonumber"><span><b>Tips: </b></span></span> 
       <ul> 
        <li><p>The owner of the project becomes the owner of this activity. If the project has no owner, then the activity has no owner. </p></li> 
        <li><p>You cannot manually update the progress of a project. Workfront calculates the progress of the project based on the project percent complete. When the project percent complete updates in&nbsp;Workfront this also updates the connected project in&nbsp;Workfront Goals including the percent complete of the goal. </p></li> 
       </ul> 
      </div></li> 
    </ol></li> 
  </ol></li> 
 <li value="5"> <p>Click <span class="bold">Save</span>.</p> <p>The activity is saved for the selected goal. After you activate the goal, the progress of the goal automatically updates when you update the progress of an activity or when the percent complete of a project updates. For information about activating a goal, see <a href="../../workfront-goals/goal-management/activate-goals.md" class="MCXref xref">Activate goals in Adobe Workfront Goals</a>.</p> </li> 
</ol>

