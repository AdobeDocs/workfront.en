---
filename: manage-task-details-forms-finances
product-area: projects
navigation-topic: manage-tasks
title: Manage task details, custom forms, and finances
description: You can manage the information about a task by referring to the Task Details tab.
---

# Manage task details, custom forms, and finances

You can manage the information about a task by referring to the Task Details tab.

You must have view or contribute permissions to the task to see information on the Task Details tab. You must have manage permissions to the task to edit information on the Task Details tab.

To access the Task Details tab:

1. Go to the `Projects` area of the Global Navigation Bar.
1. Click `Projects`.
1. Click the name of the project where you want to view a task.
1. Click the `Tasks` tab.
1. Click the name of a task that you want to view.
1. Click `Task` Details.
1. Choose any of the three sub-tabs to view more information about the task:

>[!TIP]
>
>You can also search for a task, and click the name to access the task. For more information on searching for objects in *Adobe Workfront*, see [Search Adobe Workfront](../../../workfront-basics/navigate-workfront/search/search-workfront.md).

## Manage task information on the Overview subtab

If you have manage permissions to the task, you can edit the information on the `Overview` sub-tab.  If you have view or contribute permissions to a task, you can only view the information on the `Overview` sub-tab.

For more information about task permissions, see [Share a task in Adobe Workfront](../../../workfront-basics/grant-and-request-access-to-objects/share-a-task.md).

You can see the following information on the `Overview` sub-tab:

`Name`:&nbsp;Name of the task.

`Description`:&nbsp;Description&nbsp;of the task.&nbsp;

`URL`: Users with contribute or manage permissions to a task can specify&nbsp;any links to internal or external&nbsp;pages that&nbsp;reference the task in this field.

`Priority`:&nbsp;The designated​&nbsp;priority or importance of the task.

`Duration Type`:&nbsp;Identifies the relationship between the number of resources assigned to a task and the total effort or total duration of the task. For more information about duration types, see [Overview of Task Duration and Duration Type](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md).

`Duration`: The difference in days between the planned start date and the planned completion date, provided the duration type is simple. This is the planned length of time the task will take. Depending on the duration type of the task, and the number of resources assigned to the task, this value can be manually editable, or a calculation. For more information about duration types, see [Overview of Task Duration and Duration Type](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md).

`Projected Duration`: The difference in days between the projected start date and the projected completion date.&nbsp;

`Actual Duration`:​&nbsp;The difference in days between the actual start date and the actual completion date. This is how long the task actually took to complete.&nbsp;

`Planned Hours`:&nbsp;Hours planned for the task. Depending on the duration type of the task and the number of resources assigned to the task, this value can be manually editable, or a calculation. For more information about duration types, see [Overview of Task Duration and Duration Type](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md).

`Actual` `Hours`: Hours actually recorded on the task.

`Task Constraint`:&nbsp;Sets the scheduling constraint for the task. For more information about task constraints, see [Task Constraint overview](../../../manage-work/tasks/task-constraints/task-constraint-overview.md).

`Planned Start Date`: When the task&nbsp;is planned to start.&nbsp;The planned start date of a task is set and influenced by a number of factors:

* Depending on the system-wide preference&nbsp;for the task planned start date, the start date of a new task on a project can either be today, or the start date of the project. For more information about the system-wide task preferences, see [Configure system-wide task and issue preferences](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).
* Depending on the predecessors of the task, the planned start date is picked by *Workfront*&nbsp;to be the next available date after the predecessors finish, or start, depending on the predecessor relationship. For more information about predecessor relationships, see [Overview of task predecessors](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md).

* The project manager or the task owner can manually set the planned start date when the task constraint is either Fixed Dates or Must Start On. For more information about task constraints, see [Task Constraint overview](../../../manage-work/tasks/task-constraints/task-constraint-overview.md).

`Projected Start Date`: ``The&nbsp;‘real life’ date&nbsp;of when the task is going to start based on the progress and completion of prior tasks.&nbsp;The projected start&nbsp;date and the planned start&nbsp;date start out by being the same, when a project is first planned. The projected start&nbsp;date can move away from the planned start, if the project evolves and the task is not started yet. For more information about projected start&nbsp;dates, see [Overview of the project Projected Start Date](../../../manage-work/projects/planning-a-project/project-projected-start-date.md).

`Actual Start Date`:&nbsp;The date and time the work was initiated. The default is always the actual time when the task status changed to In Progress, for the first time. The actual start date can also be manually modified by the project manager, or the task owner.&nbsp;

`Planned Completion Date`: The anticipated completion date as shown when the task is planned. The planned completion date can be set by a number of factors:

* The planned completion date is calculated from the planned start date by adding the Duration of the task to the planned start date. When the&nbsp;project manager or *Workfront* specifies&nbsp;the Duration of the task, this triggers an update to the planned completion date. If the planned date changes, it will often be because the Duration of the has been updated.
* The project manager or the task owner can manually set the planned completion&nbsp;date when the task constraint is either Fixed Dates or Must Finish&nbsp;On. For more information about task constraints, see [Task Constraint overview](../../../manage-work/tasks/task-constraints/task-constraint-overview.md).
* If the Duration Type of the task changes, and&nbsp;the number of resources&nbsp;on the tasks changes at the same time, the planned completion date will change, as well.&nbsp;For more information about duration types, see [Overview of Task Duration and Duration Type](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md).

`Projected Completion Date:`&nbsp;The&nbsp;‘real life’ date&nbsp;of when the task is going to be completed based on the progress of prior tasks&nbsp;and on the progress updates made on the task by the assignee. The projected completion date and the planned completion date start out by being the same, when a project is first planned. The projected completion date can move away from the planned completion, if the project evolves and the task is not started yet. For more information about projected completion dates, see [Overview of the Projected Completion Date for projects, tasks, and issues](../../../manage-work/projects/planning-a-project/project-projected-completion-date.md).

`Actual Completion Date:`&nbsp;The actual date and time the task is marked Completed. The default date and time when a task is completed will always coincide with the actual time when the task status becomes Completed. The actual completion&nbsp;date can also be manually modified by the project manager, or the task owner.&nbsp;

`Entered By`: Person who created task.&nbsp;

`Last Updated By`: Person who last updated the task.

## Manage task information on the Custom Forms subtab

If your *Workfront administrator* created custom forms for tasks, you can attach a custom form to a task in this tab.

You can attach up to 10 forms to the same task. Only active custom forms can be associated with tasks. <![CDATA[    ]]>

For more information about creating custom forms, see [Create or edit a custom form](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md). For more information about applying custom form to objects, see [Add a custom form to an object](../../../workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md).

## Manage task finances on the Finance subtab

If you have manage permissions to the task, and you have finance access in your access level, you can&nbsp;view and edit the Finance tab of the task.

For more information on financial access, see [Grant access to financial data](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).&nbsp;

For more information about task permissions, see [Share a task in Adobe Workfront](../../../workfront-basics/grant-and-request-access-to-objects/share-a-task.md).

You can see the following information on the `Finance` sub-tab:

`Cost Type`: Defines how&nbsp;the cost of the task is tracked. For more information about cost types, see [Track costs](../../../manage-work/projects/project-finances/track-costs.md).

`Revenue Type`:&nbsp;Defines how&nbsp;revenue&nbsp;of the task is tracked. For more information about revenue types, see [Overview of Billing and Revenue](../../../manage-work/projects/project-finances/billing-and-revenue-overview.md).

`Planned Cost`: A calculation that shows the cost of the task based on the planned hours and the cost type. For more information about tracking costs, see [Track costs](../../../manage-work/projects/project-finances/track-costs.md).

`Actual Cost`: A calculation that shows the cost of the task based on the actual&nbsp;hours and the cost type. For more information about tracking costs, see [Track costs](../../../manage-work/projects/project-finances/track-costs.md).

`Planned Revenue`: A calculation that shows the revenue associated with the task based on the planned&nbsp;hours and the revenue&nbsp;type. For more information about tracking costs, see [Track costs](../../../manage-work/projects/project-finances/track-costs.md).

`Planned Revenue`: A calculation that shows the revenue associated with the task based on the planned&nbsp;hours and the revenue&nbsp;type. For more information about tracking costs, see [Track costs](../../../manage-work/projects/project-finances/track-costs.md).

`CPI/SPI/CSI`: Calculations of cost and schedule performance metrics for the task.&nbsp;

For more information about  `CPI` (Cost Performance Index), see [Calculate Cost Performance Index (CPI)](../../../manage-work/projects/project-finances/calculate-cpi.md).

For more information about `SPI` (Schedule Performance Index), see [Calculate Schedule Performance Index (SPI)](../../../manage-work/projects/project-finances/calculate-spi.md).

For more information about `CSI` (Cost Schedule Performance Index), see [Calculate Cost Schedule Performance Index (CSI)](../../../manage-work/projects/project-finances/calculate-csi.md).

`Estimate at Completion`: A calculation that shows the total cost of your task, at completion. For more information about estimate at completion, see [Calculate Estimate At Completion (EAC)](../../../manage-work/projects/project-finances/calculate-eac.md).
