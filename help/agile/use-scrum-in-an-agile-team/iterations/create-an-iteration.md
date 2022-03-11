---
filename: create-an-iteration
product-area: agile-and-teams
navigation-topic: iterations
title: Create an iteration
description: Iterations are a key component for Scrum agile teams in planning out work capacity. Adobe Workfront allows Scrum agile teams to manage their work by creating multiple iterations to accommodate team needs.
---

# Create an iteration

Iterations are a key component for Scrum agile teams in planning out work capacity. `Adobe Workfront` allows Scrum agile teams to manage their work by creating multiple&nbsp;iterations to accommodate team needs.

## Access requirements

You must have the following access to perform the steps in this article:

<table cellspacing="0"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><span>Adobe Workfront</span> plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><span>Adobe Workfront</span> license*</td> 
   <td> <p><span>Review</span> or higher</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan or license type you have, contact your `Workfront administrator`.
Add an iteration Use the Add Iteration feature to quickly create an iteration and add tasks and issues later. Click the Main Menu icon in the upper-right corner of Adobe Workfront, then click Teams. (Optional) Click the Switch team icon , then either select a new Scrum team from the drop-down menu or search for a team in the search bar. On the Iterations tab, click Add Iteration. Specify the following: Iteration Name Enter the name of the iteration. Goal Add any goals you have for the iteration. Start Date Enter the date the iteration should start. End Date Enter the date the iteration should end. Workfront recommends setting an end date no longer than 4 weeks from the start date. Tip: Make sure to choose a working day as the end date. The burndown chart uses only working days in its calculations. By default, the burndown chart uses the default schedule to define working days (as described in Create a schedule). Or, to incorporate team-specific non-working days, agile teams can choose to use an alternate schedule (as described in"Defining an Alternate Team Schedule for Burndown Charts" in Create an agile team). Capacity Specify the capacity for the iteration. This is the number of points or hours your team is able to accomplish in the iteration. The number you enter must be equal to or greater than the number of points or hours from the sum of all the stories in the iteration. Workfront pre-populates this field with 50 capacity by default. Focus Specify the focus percentage of the team. If all members of the team will be focused completely on this iteration, the focus would be 100%. Workfront pre-populates this field with 100% by default. Click Submit. Now that you've created an iteration, you need to add stories. For more information, see Add stories to an existing iteration. 

## Plan an iteration on the Backlog tab

Use the Plan Iteration feature to create an iteration using tasks on your backlog.

<ol> Click the Main Menu icon in the upper-right corner of Adobe Workfront, then click Teams. (Optional) Click the Switch team icon , then either select a new Scrum team from the drop-down menu or search for a team in the search bar. Select Backlog on the left panel. Then, click Plan Iteration. 
 <li value="4">Specify the following information:<br> 
  <table cellspacing="0"> 
   <col> 
   <col> 
   <tbody> 
    <tr> 
     <td role="rowheader"><span class="bold">Iteration Name:</span></td> 
     <td>Specify a name for the iteration.</td> 
    </tr> 
    <tr> 
     <td role="rowheader"><span class="bold">Start Date:</span></td> 
     <td> Specify the date the iteration should start.</td> 
    </tr> 
    <tr> 
     <td role="rowheader"><span class="bold">End Date:</span>&nbsp;</td> 
     <td><p>Specify the date the iteration should end. Workfront recommends setting an end date no longer than 4 weeks from the start date.</p><note type="tip">
       Make sure to choose a working day as the end date. The burndown chart uses only working days in its calculations.
       <br>By default, the burndown chart uses the&nbsp;default schedule to define working days (as described in&nbsp;
       <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref">Create a schedule</a>). Or, to incorporate team-specific non-working days,&nbsp;agile teams can choose to use an alternate schedule (as described in 
       <a href="../../../agile/use-scrum-in-an-agile-team/burndown/use-alt--team-schedule-burndown-charts.md" class="MCXref xref">Use an alternate team schedule for burndown charts</a>).
      </note></td> 
    </tr> 
    <tr> 
     <td role="rowheader"><span class="bold">Focus:</span></td> 
     <td>Specify the focus percentage of the team. If all members of the team will be focused completely on this iteration, the focus would be 100%.<br><span>Workfront</span> pre-populates this field with the average value from your team's past iterations. If this is your team's first iteration, this field value is 0 by default.</td> 
    </tr> 
    <tr> 
     <td role="rowheader"><br><span class="bold">Capacity:</span></td> 
     <td> Specify the capacity for the iteration. This is the number of points or hours your team is able to accomplish in the iteration. The number you enter must be equal to or greater than the number of points or hours from the sum of all the stories in the iteration.<br><span>Workfront</span> pre-populates this field with the average value from your team's past iterations. If this is your team's first iteration, this field value is 0 by default.</td> 
    </tr> 
    <tr> 
     <td role="rowheader"><br><span class="bold">Goal:</span></td> 
     <td> Specify a goal for the iteration.&nbsp;This field is not required.</td> 
    </tr> 
   </tbody> 
  </table></li> 
 <li value="5">(Optional) Select stories to add them to&nbsp;the iteration now, or you can skip this step and add stories to an iteration at a later time. The stories at the top of the backlog are higher priority. Stories&nbsp;are highlighted in green when they fit in the capacity; they are highlighted in red if they do not.<br>You can add both tasks and issues to a single iteration: 
  <ul> 
   <li><span class="bold">To add tasks to the iteration:</span> On the <span class="bold">Backlog</span> tab, ensure that the <span class="bold">Stories</span> tab is selected (this tab is selected by default when viewing the backlog). Select the stories you want to add to the iteration.<br>When you add tasks to an iteration, the start date of the task is calculated as described in&nbsp;<a href="#understanding-how-task-start-dates-are-calculated-when-added-to-an-iteration" class="MCXref xref">Understand how task start dates are calculated when added to an iteration</a>.</li> 
   <li><span class="bold">To add issues to the iteration:</span> On the <span class="bold">Backlog</span> tab, click the <span class="bold">Issues</span> tab. Select the issues you want to add to the iteration.</li> 
  </ul></li> 
 <li value="6">Click <span class="bold">Save.</span><br>The iteration is created.</li> 
 <li value="7">(Optional) To add stories to an existing iteration, see <a href="../../../agile/use-scrum-in-an-agile-team/iterations/add-stories-to-existing-iteration.md" class="MCXref xref">Add stories to an existing iteration</a>.</li> 
</ol>

## Understand how task start dates are calculated when added to an iteration

When you add a task as a story to an iteration, the Must Finish On task constraint is used for&nbsp;each story. In most cases, the planned start date of the task is calculated based on the following formula:

Iteration End Date minus (-) Task Duration equals (=) Task Planned Start Date

The Project End Date is used instead of the Iteration End Date if&nbsp;the&nbsp;project start date is after the iteration start date, and the project end date is after the iteration end date.
You can configure individual Scrum teams to use the project dates by default, rather than the iteration dates. For information, see the section Configure how dates are applied when adding work items to an iteration in the article Configure Scrum.  