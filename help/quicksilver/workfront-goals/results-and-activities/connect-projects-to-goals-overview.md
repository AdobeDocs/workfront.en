---
filename: connect-projects-to-goals-overview
content-type: overview
product: workfront-goals
product-area: projects
navigation-topic: results-and-activities
title: Overview of connecting projects to goals in Adobe Workfront Goals
description: (NOTE: THIS MIGHT NEED TO BE RENAMED BECAUSE THERE WILL BE OTHER OBJECTS CONNECTED TO GOALS IN THE FUTURE)
---

# Overview of connecting projects to goals in Adobe Workfront Goals

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: THIS MIGHT NEED TO BE RENAMED BECAUSE THERE WILL BE OTHER OBJECTS CONNECTED TO GOALS IN THE FUTURE) </p>
-->

Your organization must have the following to use the functionality described in this article:

* A Pro or higher [Adobe Workfront plan](https://www.workfront.com/plans). 
* An Adobe Workfront Goals license in addition to a Workfront license.

  Contact your Workfront account manager to learn about a Workfront Goals license.

  Workfront Goals is available only in the new Adobe Workfront experience.

For additional information about access to Workfront Goals, see [Requirements to use Workfront Goals](../../workfront-goals/goal-management/access-needed-for-wf-goals.md).

>[!IMPORTANT]
>
>Project-level goals created in the Business Case area of a project are not connected to strategic goals created in Workfront Goals.&nbsp;For information about Business Case project goals, see [Create Business Case goals](../../manage-work/projects/define-a-business-case/create-business-case-goals.md).

## Connect projects to goals

To move your organization forward, you must create alignment between your outputs (executed work) and your outcomes (strategic goals). You can show how the work your groups, teams, and individual contributors are performing contributes to the progress of your organization’s goals.

To this purpose, you can connect projects as activities (outputs or executed work) to your goals (outcomes).

## Considerations about connecting projects to goals

* ```You must have access to create goals before you can add projects to goals. For information about creating goals, see [Create goals in Adobe Workfront Goals](../../workfront-goals/goal-management/create-goals.md).``` 
* Adding a project to a goal is identical to adding activities to a goal.

  For information about adding activities to goals, see [Add activities to goals in Adobe Workfront Goals](../../workfront-goals/results-and-activities/add-activities-to-goals.md). For information about disconnecting projects from goals, see the "Disconnect projects from goals" section in the article [Remove results, activities, and projects from goals in Adobe Workfront Goals](../../workfront-goals/results-and-activities/remove-results-activities-from-goals.md). 

* You can add a project that meets the following criteria to a goal:

   * You must have at least permissions to&nbsp;View it.

     >[!NOTE]
     >
     >If you lose your permissions to view the project after you have attached the project to the goal, you can still see project information on the goal, but you can no longer access the project.

   * The project must not be in a status of Dead.

* You can associate multiple projects with a goal.
* You can associate the same project with multiple goals. 
* Although the project is connected to the goal as a type of activity, you cannot manually update the progress of a project when you check in on your goal. Instead, Workfront calculates the percent complete of the project and Workfront Goals calculates the goal progress using this percent complete. ```This updates the goal in real time after the project percent updates.``` 
* The owner of the project becomes the owner of this activity.
* The project duration can be outside the time period of a goal. If a project lasts longer than the goal’s deadline, you can still close your goal and consider it completed, but the goal percent complete will not be 100%. The percent complete of the project no longer updates on the goal. There is an indication on the goal list that the project no longer updates progress for the goal.

  ![](assets/goal-closed-project-active-warning-goal-list-350x94.png)

* When you delete a project attached to a goal, the project is also deleted from the goal.

  >[!CAUTION]
  >
  >If the goal was active and there are no other progress indicators on the goal, the goal becomes Inactive.

## Locate project information on goals

The following project information is visible at the goal level: 

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Project Name</td> 
   <td>Any changes in the project name also reflect in the connected project. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Project Owner</td> 
   <td> If the project has no owner, then the activity has no owner. Any changes in the project owner also reflect in the connected project. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Project Percent Complete</td> 
   <td>Any change in the percent complete of the project automatically updates the goal progress unless the goal is closed. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Due Date</td> 
   <td> <p>This is the project's Planned Completion Date. A project's due date can be earlier than the goal's start date, or later than the goal's end date. The Due Date of the project is visible at the goal level.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Locate goal information on projects

The following goal information is visible in a project list or report:

| Goals  |A list of all goals that have a project as one of their activities.  |
|---|---|
| Goal Hierarchy |The hierarchy that a goal belongs to. Only the parents of the goal and the goal display in this field. Children goals do not display.  |
| Number of Linked Goals |The number of goals linked to one project. |

