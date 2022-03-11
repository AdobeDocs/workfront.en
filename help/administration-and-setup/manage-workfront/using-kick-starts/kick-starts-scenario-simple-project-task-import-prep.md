---
filename: kick-starts-scenario-simple-project-task-import-prep
user-type: administrator
product-area: system-administration;projects
keywords: kickstart,kick-start,kickstarts,kick-starts
navigation-topic: use-kick-starts
title: Kick-Starts scenario: simple project and task import preparation
description: Describes in detail the available settings and controls for a basic Project and Task Import using the Kick Start method.
---

# Kick-Starts scenario: simple project and task import preparation

Describes in detail the available settings and controls for a &nbsp;basic Project and Task Import using the Kick Start method.&nbsp;

## `Scenario`

The implementation team would rather import project and task information for active projects as opposed to manually inputting this data into the system.

* [Projects](#projects) 
* [Task list](#task)

### Projects

The following table displays four Projects and their basic details that need to be mapped into the Kick Start file formats.

`<font color="#666666">This scenario assumes users are already imported into </font>`Adobe Workfront`<font color="#666666">. If users are not already in </font>`Workfront`<font color="#666666">, subsitute different names or complete the Kick Start Scenario with users prior to this scenario.&nbsp;</font>`

<ol> 
 <li value="1"> <p>Implement Workfront.</p> 
  <table cellspacing="0"> 
   <col width="50%"> 
   <col width="50%"> 
   <tbody> 
    <tr> 
     <td role="rowheader">Planned Start Date</td> 
     <td>Today</td> 
    </tr> 
    <tr> 
     <td role="rowheader">Project Manager</td> 
     <td>Jennifer Campbell</td> 
    </tr> 
    <tr> 
     <td role="rowheader">Project Sponsor</td> 
     <td>Marc Lewis</td> 
    </tr> 
    <tr> 
     <td role="rowheader">Group</td> 
     <td>Marketing</td> 
    </tr> 
    <tr> 
     <td role="rowheader">Company</td> 
     <td><i>YourCompany</i> </td> 
    </tr> 
   </tbody> 
  </table> </li> 
 <li value="2"> <p>Implement HR&nbsp;System.</p> 
  <table cellspacing="0"> 
   <col width="50%"> 
   <col width="50%"> 
   <tbody> 
    <tr> 
     <td role="rowheader">Planned Start Date</td> 
     <td>July 14, 20XX</td> 
    </tr> 
    <tr> 
     <td role="rowheader">Project Manager</td> 
     <td>Pam Reynolds</td> 
    </tr> 
    <tr> 
     <td role="rowheader">Project Sponsor</td> 
     <td>Marc Lewis</td> 
    </tr> 
    <tr> 
     <td role="rowheader">Group</td> 
     <td>Marketing</td> 
    </tr> 
    <tr> 
     <td role="rowheader">Company</td> 
     <td><i>YourCompany</i> </td> 
    </tr> 
   </tbody> 
  </table> </li> 
 <li value="3"> <p>Implement Document Management System.</p> 
  <table cellspacing="0"> 
   <col width="50%"> 
   <col width="50%"> 
   <tbody> 
    <tr> 
     <td role="rowheader">Planned Start Date</td> 
     <td>August 22, 20XX</td> 
    </tr> 
    <tr> 
     <td role="rowheader">Project Manager</td> 
     <td>Jennifer Campbell</td> 
    </tr> 
    <tr> 
     <td role="rowheader">Project Sponsor</td> 
     <td>Ray Andrews</td> 
    </tr> 
    <tr> 
     <td role="rowheader">Group</td> 
     <td>IT</td> 
    </tr> 
    <tr> 
     <td role="rowheader">Company</td> 
     <td><i>YourCompany</i> </td> 
    </tr> 
   </tbody> 
  </table> </li> 
 <li value="4"> <p>Implement New Calendar System.</p> 
  <table cellspacing="0"> 
   <col width="50%"> 
   <col width="50%"> 
   <tbody> 
    <tr> 
     <td role="rowheader">Planned Start Date</td> 
     <td>September 6, 20XX</td> 
    </tr> 
    <tr> 
     <td role="rowheader">Project Manager</td> 
     <td>Pam Reynolds</td> 
    </tr> 
    <tr> 
     <td role="rowheader">Project Sponsor</td> 
     <td>Ray Andrews</td> 
    </tr> 
    <tr> 
     <td role="rowheader">Group</td> 
     <td>IT</td> 
    </tr> 
    <tr> 
     <td role="rowheader">Company</td> 
     <td><i>YourCompany</i> </td> 
    </tr> 
   </tbody> 
  </table> </li> 
</ol>

### Task list

The following task list displays overly simplified task lists for the projects. The only difference between projects is the start dates and progress made on each project.&nbsp;

Parent tasks inherit the Duration, Work, and Percent Complete of children tasks. It is not necessary to set those values for that&nbsp;will become summary tasks.

>[!NOTE]
>
>The instructions provided in this scenario are not as explicit as the step-by-step directions provided in ` [Kick-Starts Scenario: Company, Group, Role, and User Kick-Starts Preparation](../../../administration-and-setup/manage-workfront/using-kick-starts/kick-starts-scenario-company-group-role-user-prep.md)`. The assumption is you have already learned how to look up and copy values from the Company and Group sheets, so these steps will be mentioned, but not specifically outlined.&nbsp;

<ol> 
 <li value="1">Configure.</li> 
 <li value="2"> <p>Import users.</p> 
  <table cellspacing="0"> 
   <col width="50%"> 
   <col width="50%"> 
   <tbody> 
    <tr> 
     <td role="rowheader">Assigned to</td> 
     <td>Ray Andrews</td> 
    </tr> 
    <tr> 
     <td role="rowheader">Parent task</td> 
     <td>1</td> 
    </tr> 
    <tr> 
     <td role="rowheader">Duration</td> 
     <td>1 hour</td> 
    </tr> 
    <tr> 
     <td role="rowheader">Work</td> 
     <td>1 hour</td> 
    </tr> 
    <tr> 
     <td role="rowheader">Percent complete</td> 
     <td> <p>Workfront: 0%</p> <p>HR: 100%</p> <p>Docs: 100%</p> <p>Calendar: 100%</p> </td> 
    </tr> 
   </tbody> 
  </table> </li> 
 <li value="3"> <p>Set permissions.</p> 
  <table cellspacing="0"> 
   <col width="50%"> 
   <col width="50%"> 
   <tbody> 
    <tr> 
     <td role="rowheader">Assigned to</td> 
     <td>Ray Andrews</td> 
    </tr> 
    <tr> 
     <td role="rowheader">Parent task</td> 
     <td>1</td> 
    </tr> 
    <tr> 
     <td role="rowheader">Pred</td> 
     <td>2</td> 
    </tr> 
    <tr> 
     <td role="rowheader">Duration</td> 
     <td>1 hour</td> 
    </tr> 
    <tr> 
     <td role="rowheader">Work</td> 
     <td>1 hour</td> 
    </tr> 
    <tr> 
     <td role="rowheader">Percent complete</td> 
     <td> <p>Workfront: 0%</p> <p>HR: 100%</p> <p>Docs: 100%</p> <p>Calendar: 100%</p> </td> 
    </tr> 
   </tbody> 
  </table> </li> 
 <li value="4"> <p>Build groups.</p> 
  <table cellspacing="0"> 
   <col width="50%"> 
   <col width="50%"> 
   <tbody> 
    <tr> 
     <td role="rowheader">Assigned to</td> 
     <td>Ray Andrews</td> 
    </tr> 
    <tr> 
     <td role="rowheader">Parent task</td> 
     <td>1</td> 
    </tr> 
    <tr> 
     <td role="rowheader">Pred</td> 
     <td>4</td> 
    </tr> 
    <tr> 
     <td role="rowheader">Duration</td> 
     <td>2 days</td> 
    </tr> 
    <tr> 
     <td role="rowheader">Work</td> 
     <td>4 hours</td> 
    </tr> 
    <tr> 
     <td role="rowheader">Percent complete</td> 
     <td> <p>Workfront: 0%</p> <p>HR: 100%</p> <p>Docs: 100%</p> <p>Calendar: 25%</p> </td> 
    </tr> 
   </tbody> 
  </table> </li> 
 <li value="5"> <p>Prepare training.</p> 
  <table cellspacing="0"> 
   <col width="50%"> 
   <col width="50%"> 
   <tbody> 
    <tr> 
     <td role="rowheader">Assigned to</td> 
     <td>Chris Manning</td> 
    </tr> 
    <tr> 
     <td role="rowheader">Duration</td> 
     <td>2 days</td> 
    </tr> 
    <tr> 
     <td role="rowheader">Work</td> 
     <td>4 hours</td> 
    </tr> 
    <tr> 
     <td role="rowheader">Percent complete</td> 
     <td> <p>Workfront: 0%</p> <p>HR: 100%</p> <p>Docs: 50%</p> <p>Calendar: 100%</p> </td> 
    </tr> 
   </tbody> 
  </table> </li> 
 <li value="6"> <p>Build ongoing support policies.</p> 
  <table cellspacing="0"> 
   <col width="50%"> 
   <col width="50%"> 
   <tbody> 
    <tr> 
     <td role="rowheader">Assigned to</td> 
     <td>Chris Manning</td> 
    </tr> 
    <tr> 
     <td role="rowheader">Duration</td> 
     <td>2 days</td> 
    </tr> 
    <tr> 
     <td role="rowheader">Work</td> 
     <td>4 hours</td> 
    </tr> 
    <tr> 
     <td role="rowheader">Percent complete</td> 
     <td> <p>Workfront: 0%</p> <p>HR: 100%</p> <p>Docs: 50%</p> <p>Calendar: 0%</p> </td> 
    </tr> 
   </tbody> 
  </table> </li> 
 <li value="7"> <p>Roll out.</p> 
  <table cellspacing="0"> 
   <col width="50%"> 
   <col width="50%"> 
   <tbody> 
    <tr> 
     <td role="rowheader">Pred</td> 
     <td>1, 6, 7</td> 
    </tr> 
   </tbody> 
  </table> </li> 
 <li value="8"> <p>Train users.</p> 
  <table cellspacing="0"> 
   <col width="50%"> 
   <col width="50%"> 
   <tbody> 
    <tr> 
     <td role="rowheader">Assigned to</td> 
     <td>Chris Manning</td> 
    </tr> 
    <tr> 
     <td role="rowheader">Parent task</td> 
     <td>8</td> 
    </tr> 
    <tr> 
     <td role="rowheader">Duration</td> 
     <td>1 day</td> 
    </tr> 
    <tr> 
     <td role="rowheader">Work</td> 
     <td>2 hours</td> 
    </tr> 
    <tr> 
     <td role="rowheader">Percent complete</td> 
     <td> <p>Workfront: 0%</p> <p>HR: 0%</p> <p>Docs: 0%</p> <p>Calendar: 0%</p> </td> 
    </tr> 
   </tbody> 
  </table> </li> 
</ol>

## `Download Template`

Go to the Kick-Starts page. Select the Company, Group, Project, Task, and User objects.&nbsp;Select the Include existing data checkbox &nbsp;(do this to quickly reference Company, Group and User IDs).&nbsp;Click the Download button.

## Input Project Details

Open the Workfront.xlsx file you just downloaded.&nbsp;Go to the PROJ Project sheet.

![](assets/im2-350x14.png)   
Unless you have already created projects in Workfront, it should be empty.  
![](assets/im3-350x37.png)

>[!NOTE]
>
>Consider using the spreadsheet's Freeze Panes tool and/ or hiding or removing unneeded columns to make the sheet easier to use. However, be careful not to remove any required columns or columns &nbsp;to use later.

![](assets/im10-350x42.png)

Set the values for the following project fields:&nbsp;

* `Set isNew column`   
  Input TRUE into rows 3 through 6 for the isNew column.
* `Set unique IDs`   
  Input a unique ID in each row for the ID column — Typically, integers starting at 1 work well when creating new records.
* `Set Project Names`   
  Input the names of each project into the setName column.
* `Set project schedule`

  Input the ID of the schedule that you want the project to use in the setScheduleID field

* `Set the project Planned Start Date`

  Input the date and the time in the setPlannedStartDate column with the time and the date when you want the project to start. If left empty, Workfront imports the project with the current day's date and a timestamp of that day's midnight according to the browser's timezone. 

* `Set Task numbers`   
  Input values into the setTaskNumber column to control the order the tasks will appear in the project plan.
* `Provide project dates.`   
  Input the Planned Start Date for each project in the setPlannedStartDate column.
* `Set other needed details.`   
  Fill in other details, such as a description or current status, as needed.&nbsp;Look up the Group IDs for each project on the GROUP Group sheet and input them into the setGroupID column for the respective projects.&nbsp;Look up the Company ID for the projects on the CMPY Company sheet and input it into the setCompanyID column.&nbsp;Look up the User ID for each project owner on the USER User sheet and input it into the setOwnerID column.&nbsp;Look up the User ID for each project sponsor on the USER User sheet and input it into the setSponsorID column.

![](assets/im9-350x24.png)

>[!NOTE]
>
>Acceptable values for Status and Priority fields can be located by reviewing the status and priority preferences for each object in the Workflow Setup area of Workfront.

## `Input Task Details`

You can add information about the tasks on the project, as you import the project using kick-starts.

Open the Workfront.xlsx file you just downloaded.  `Go to the TASK Task sheet.`

Unless you have already created tasks in&nbsp;Workfront, this sheet should be empty.

![](assets/im8-350x14.png)

![](assets/im7-350x43.png)

![](assets/im6-350x16.png)

The easiest way to map tasks is one project at a time (especially when the tasks are the same on each project). You can then copy the task plan for the first project and make small adjustments to the task plan for the subsequent projects. The remaining steps will assume you are creating tasks for just the Implement Workfront project. According to the scenario, you will be importing 9 tasks per project, so input TRUE into rows 3 through 11 for the isNew column.

Set the values for the following task fields:&nbsp;

<ul> 
 <li> <p><span class="bold">Set IDs</span> <br>Input a unique ID in each row for the ID column.</p> </li> 
 <li> <p><span class="bold">Set Names</span> <br>Input the task names into the setName column.</p> </li> 
 <li> <p><span class="bold">Confirm Project ID&nbsp;</span> <br>Input the ID you set for the Implement Workfront project; review the PROJ Project sheet to make sure it is the correct ID.</p> </li> 
 <li> <p><span class="bold">Set Users</span> <br>Go to the USER User sheet to look up the ID for the user assigned to each task and input these values in the respective cells in the setAssignedToID column.</p> </li> 
 <li> <p><span class="bold">Identify&nbsp;Task relationships</span> <br>For tasks 2 through 5, input a 1 in the setParentID column.&nbsp;For task 9, input a 8 in the setParentID column.&nbsp;In the &nbsp;setPredecessorString column, input the task number for each predecessor task.&nbsp;In cases where a task has multiple predecessors, like task 8 in this scenario, you will need to use a comma to separate each predecessor task ID. Predecessors &nbsp;can be defined with lags on non-Finish-Start relationships by using the shorthand described in the <span class="external">Creating Predecessor Relationships</span> article.</p> </li> 
 <li> <p><span class="bold">Set Duration</span> <br>Set the duration for each task by inputting number of hours, days, weeks, or months for the task in the setDuration field. Then input the duration unit in the setDurationUnit field.</p> 
  <table cellspacing="15"> 
   <col> 
   <col> 
   <thead> 
    <tr> 
     <th>&nbsp;</th> 
     <th>Acceptable value</th> 
    </tr> 
   </thead> 
   <tbody> 
    <tr> 
     <td>Minutes</td> 
     <td>M</td> 
    </tr> 
    <tr> 
     <td>Hours</td> 
     <td>H</td> 
    </tr> 
    <tr> 
     <td>Days</td> 
     <td>D</td> 
    </tr> 
    <tr> 
     <td>Weeks</td> 
     <td>W</td> 
    </tr> 
    <tr> 
     <td>Months</td> 
     <td>T</td> 
    </tr> 
   </tbody> 
  </table> <p>Minutes can also be represented &nbsp;as fraction of an hour (eg., minutets = 5 hours)</p> </li> 
 <li> <p>Set the amount of effort for each task in the setWorkRequired field. Then input the work unit in the setWorkUnit field. If the Work Required value is different from the duration, you will also need to input an A into the setDurationType field.</p> 
  <table border="1" cellspacing="15" cellpadding="1"> 
   <col> 
   <col> 
   <thead> 
    <tr> 
     <th scope="col">Duration Type</th> 
     <th scope="col">Acceptable Value</th> 
    </tr> 
   </thead> 
   <tbody> 
    <tr> 
     <td>Calculated Assignment</td> 
     <td>A</td> 
    </tr> 
    <tr> 
     <td>Calculated Work</td> 
     <td>W</td> 
    </tr> 
    <tr> 
     <td>Effort Driven</td> 
     <td>D</td> 
    </tr> 
    <tr> 
     <td>Simple</td> 
     <td>S</td> 
    </tr> 
   </tbody> 
  </table> </li> 
 <li> <p>Input the whole number representation of the percent complete in the setPercentComplete field for each task. This value should not include the percent symbol (%).</p> </li> 
 <li> <p>Include a description and other details for each Task you are creating, as needed.</p> <p> <img src="assets/im5-350x35.png" style="width: 350;height: 35;"> </p> </li> 
 <li> <p>The setPlannedStartDate and setTaskConstraint columns are not used to build out the timeline of this project because we are relying on predecessor relationships. You can input a date for each task instead. If you do this, be sure you also provide a valid task constraint in the setTaskConstraint column. Reveiw the <span class="external">Task Constraint</span>and related articles for details on valid values for this field.</p> <p>In the case of this scenario, the easiest way to build out the tasks for the other projects you are importing is to copy the tasks you just defined and paste them below, starting on row 12. Then you will:</p> 
  <ol> 
   <li value="1">Renumber the values in the ID column.</li> 
   <li value="2">Update the setProjectID column to the value you set for the next project.</li> 
   <li value="3">Update the setParentID and setPredecessorString values to reflect the new IDs assigned to this project's tasks.</li> 
   <li value="4">Update task assignments and percent complete.</li> 
   <li value="5">Repeat these steps for the next project's tasks.</li> 
  </ol> </li> 
 <li> <p><span class="bold">Import the Excel File</span> </p> <p>Follow the directions provided in <a href="../../../administration-and-setup/manage-workfront/using-kick-starts/import-data-via-kickstarts.md" class="MCXref xref">Import data into Adobe Workfront via a Kick-Start template</a>.</p> </li> 
</ul>

