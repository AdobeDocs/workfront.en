---
filename: _custom-view-filter-grouping-samples
content-type: reference
product-area: reporting
navigation-topic: reports
---




# Custom View, Filter, and Grouping samples {#custom-view-filter-and-grouping-samples}

This section provides examples of custom views, filters, and groupings that you can use in your `Workfront` account. These examples cannot be built just by using the standard mode interface and can only be built by using the text mode interface only. For more information about text mode, see [Understand Text Mode](understand-text-mode.md).


## Hour {#hour}

[View: combined task and issue details in an Hour list](view-combined-task-issue-details-hour-list.md) 


An Hour view which combines the Task and Issue name columns, as well as the Task and Issue work required (Planned Hours) using the 

```
sharecol=true
```

line. This allows you to display the Planned Hours for both Tasks and Issues in one column. Because each hour entry can only be associated with either a Task or an Issue, you always have just one value in the shared column. In the case of an hour entry on a task, the issue reference will be null, and vice versa.


[View: hours with parent task information](view-hours-parent-task-information.md) 


This Hour view displays the name of the task where the hours were logged as well as the name of the parent task.


[Grouping: Project Sponsor for hours](grouping-project-sponsor-hours.md) 


This Hour grouping organizes hours by the sponsor of the project where the hours reside. The standard interface for Hour groupings does not provide a mapping to the project sponsor; it must be done through the Text Mode interface.


## Issue {#issue}

[View: issues with approval information](view-issues-approval-information.md) 


This Issue view shows the approval process, step, names of the approvers, and the status of the Issue before the approval was granted. Some of these fields are not accessible through the standard interface builder.


[View: issues with the company name of the originator](view-issues-company-name-originator.md) 


This Issue view displays the company name associated with the user who submitted the issue.


[View: issues with resolving object details](view-issues-resolving-object-details.md) 


This Issue view displays the name and percentage complete of the resolving object of the Issue, allowing the issue originator to have insight into the progress of the issue even without access to the resolving task or project.


## Project {#project}

[View: project with all project team users and roles](view-project-all-project-team-users-roles.md) 


This Project view shows a list of users and roles assigned to the project team.


[Filter: current projects pending approval](filter-current-projects-pending-approval.md) 


This Project filter displays projects in the Current - Pending Approval status, where the logged in user is either the project sponsor or the portfolio manager.


[View: multi-row project View](view-multi-row-project-view.md) 


This Project view displays project information in a two row format. It employs the use of the 

```
sharecol=true
```

line to combine multiple fields under the same column header. Additionally, it utilizes place holder columns that hold an HTML line break tag (<br/>) that forces the description to reside below the project name, for example.


[Grouping: project percent breakdown 1](grouping-project-percent-breakdown-1.md) 


In this custom project grouping, you can display projects grouped by a range of their percent complete values. The breakdowns show percent complete value of 25 percent point increments: 0-25%, 25-50%, etc.


[Grouping: project percent breakdown 2](grouping-project-percent-breakdown-2.md) 


In this custom project grouping, you can display projects grouped by a range of their percent complete values. The breakdowns show percent complete value of 10 percent point increments: 0-10%, 11-20%, 21-30% etc.


## `Project User`  {#project-user}

[View: project user list](view-project-user-list.md) 


A project view that displays a list of all users associated with a project and the roles they fulfill on the project. 


## Report {#report}

[Filter: report delivery filter](filter-report-delivery-filter.md) 


This Report filter will show you all reports scheduled to be delivered automatically through the `Workfront` report delivery feature. It is best used with the standard Report List View.


[View: reporting elements used in reports](view-reporting-elements-used-reports.md) 


This Report view displays the View, Filter, and Grouping used to build each report in `Workfront` in a text mode format.


You can see the fields or valueexpressions used in every element of the report.


## Task {#task}

[View: display original issue information on task and project list](view-display-original-issue-info-task-project-list.md) 


This task view allows you to display information from the original issues on task lists, after the issues have been converted to the tasks. 


[View: Actual Hours over Planned Hours in task View](view-actual-hours-planned-hours-task-view.md) 


This Task view provides an example of using the 

```
sharecol=true
```

line for a column to display the immediately following column under the same column header. In this example the actual hours recorded are displayed over the planned hours for each task.


[View: task with All Dates variance](view-task-all-dates-variance.md) 


This Task view is similar to the "All Dates" view provided with your `Workfront` account. The additions in the "Task with All Date Variance" view are the "Variance" columns which calculate the difference in days between the Planned & Projected Start Dates, Planned & Actual Start Dates, Planned & Projected Completion Dates, and Planned & Actual Completion Dates.


[View: assigned user's Company and Home Group](view-assigned-users-company-home-group.md) 


This Task view displays the primary assigned resource's company and home (or default) group association. These are values that are not available in the drop down when creating a task view, but they are accessible through the application relationships as referenced in the Table of Database Relationships.


[View: baseline variance for Duration and Planned Work in a task View](view-baseline-variance-duration-planned-work-task-view.md) 


This Task view not only displays task information with baseline task information, it also shows the difference between duration and the default baseline duration, and the difference between the planned work and the default baseline planned work.


[View (Column): list of successors](view-column-list-successors.md) 


You can add a column to a task view, to show a list of the successors of the tasks. The "Task Successors" column includes the number of the successor as well as the name.


[Filter: cross-project predecessors](filter-cross-project-predecessors.md) 


This Task filter returns incomplete Cross-Project Predecessors.


[Filter: cross-project successors](filter-cross-project-successors.md) 


This Task filter returns incomplete Cross-Project Successors.


[View: external URL using custom data field](view-url-using-custom-data-field.md) 


This view displays the text input into a custom data parameter on a task as a link to a page external to `Workfront`.


[View: originating issue details for tasks and projects](view-originating-issue-details-tasks-projects.md) 


When an issue is converted into a task a resolving object relationship is established between the task and the issue. This Task view displays some of the details of the issue that resolves when the task completes.


[Filter: parent task filter](filter-parent-task-filter.md) 


This Task filter will filter out all parent tasks in your list and only show working tasks.


[View: show parent tasks up to 4 levels deep](view-show-parent-tasks-4-levels.md) 


This Task view shows the task name and (if they exist) parent tasks up four levels deep on the project plan.


[Grouping: tasks by portfolio, program, and project](grouping-tasks-portfolio-program-project.md) 


This grouping organizes tasks by the Portfolio and Program where the projects are assigned.


[Grouping: 4-level task Grouping for Portfolio Owner, Program Owner, Project Owner, and Project Status](grouping-4-level-task-grouping.md) 


This Task grouping provides four levels of grouping. In this case, tasks are grouped by Portfolio Owner, Program Owner, Project Owner, and Project Status. You can only have up to three levels of grouping using the standard interface. To add a fourth level, you must use text mode.


[View: predecessor details](view-predecessor-details.md) 


This Task view shows details of the predecessors of the tasks using a collection view. In a collection view, you can display information about objects that are in a "one to many" relationship. In this case, each task can have multiple predecessors. The view displays the name of the tasks, as well as its Predecessors' Names, Predecessors' Project Names, Predecessors' Planned Completion Dates, and Predecessors' Statuses.


[Grouping: tasks by portfolio, program, and project](grouping-tasks-portfolio-program-project.md) 


Use this grouping in a task report, to group the tasks by the portfolio and then the program of the projects they belong to.


[Grouping: Project Sponsor for a task list](grouping-project-sponsor-task-list.md) 


This Task grouping allows you to group tasks by the Project Sponsor.


[View: Planned Hours vs. Actual Hours per assignment in task View](view-planned-hours-actual-hours-assignment-task-view.md) 


This Task view displays the total Planned Hours of a task, the number of Planned Hours allocated to each assignee, the total Actual Hours, and the number of Actual Hours logged by each assignee.


[Grouping: task percent breakdown 1](grouping-task-percent-breakdown-1.md) 


In this custom task grouping, you can display tasks grouped by a range of their percent complete values. The breakdowns show percent complete value of 25 percent point increments: 0-25%, 26-50%, etc.


[Grouping: task percent breakdown 2](grouping-task-percent-breakdown-2.md) 


In this custom task grouping, you can display tasks grouped by a range of their percent complete values. The breakdowns show percent complete value of 10 percent point increments: 0-10%, 11-20%, etc.


[View: tasks impacted by schedule exceptions](view-tasks-impacted-schedule-exceptions.md) 


This Task view identifies tasks that will have to complete late because of weekends, Personal Time Off, or other schedule exceptions.


[Column: show name of parent tasks as all caps](column-show-name-parent-tasks-all-caps.md) 


You can add this column to a task view to display the name of the parent tasks in all capital letters.


## User {#user}

[View: expanded user details](view-expanded-user-details.md) 


This User view displays information about your users. In addition to their name, access levels and Company, it also shows lists of their Groups, Teams, and Job Roles.


[View: user personal time off](view-user-personal-time-off.md) 


This User view shows a list of future days which have been marked for Time-Off by users. The view includes lists of the users' job roles, teams, and groups, in addition to their name, access level, and Company.


[View: user Job Role percentage of FTE availability](view-user-job-role-percentage-fte-availability.md) 


This User column displays a list of the Job Roles the user is associated with as well as the percentage of FTE availability for each job role, as defined in the user profile.


## Work Item {#work-item}

[Report: combined task and issue View and Grouping](report-combined-task-issue-view-grouping.md) 


This Work Item report shows both tasks and issues which users have accepted to work on in one report. It is best when combined with a custom grouping.
