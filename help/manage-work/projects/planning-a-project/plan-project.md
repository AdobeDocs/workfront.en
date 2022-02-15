---
filename: plan-project
product-area: projects
navigation-topic: plan-a-project
---



# Plan a project overview {#plan-a-project-overview}

A project is a large work item in *`Adobe Workfront`*. You can break down a project into tasks which are smaller work items. Tasks can be assigned to users or teams who can be responsible for their completion. When all users complete their tasks, the project also becomes complete.&nbsp;


In addition to planning your tasks in a project, a lot of other details go into planning projects. From determining the economic impacts to considering resource availability, there are many elements of projects that need attention.&nbsp;


## Establish a project scope {#establish-a-project-scope}

Project planning means determining exactly what major objectives you need to accomplish in order to complete the project.


In the initial phases of a project, you may not have yet determined if you should actually do the project. It may not be cost effective, or you may not have the resources. In this stage of planning, you can create a project in *`Workfront`* without adding any tasks and set the status to planning.&nbsp;


For more information about creating a project, see the article [Create a project](create-project.md).


Consider the following questions before you plan a project:&nbsp;



* Which objectives are mandatory and which are optional?
* Do you have sufficient time to achieve all of the objectives or only the core objectives?
* Do you have enough budget to accomplish all of the objectives now?&nbsp;


Using the Business Case of a project you can define your objectives and ensure that your project aligns with the strategy of your organization.&nbsp;


For more information about defining a Business Case for a project, see the article [Create a Business Case for a project in Adobe Workfront](create-business-case.md).


After you have defined the overall scope of the project, you may then determine whether you want to undertake the project at all and start planning it.&nbsp;


## Preliminary project planning {#preliminary-project-planning}




* [Define the Start and Completion Date of the project](#define-start-and-completion-dates) 
* [Define the project Schedule](#define-schedule) 
* [Manage additional information needed for planning the project](#manage-additional-information) 




### Define the Start and Completion Date of the project {#define-the-start-and-completion-date-of-the-project}

When you plan a project, one of the first things that you need to determine is the timeline: when can the project start and by what time it must complete. Determine whether there a set deadline for when the project must be finished, or whether you should set a starting point and work out from there.&nbsp;


You can schedule a project from a Start Date, or you can schedule it from the Completion Date. You can set this attribute when you initially create the project, and you can change it at any time by editing your project.


### Define the project Schedule {#define-the-project-schedule}

You must determine a schedule and associate it with the project, as well as with the users who are responsible for completing the tasks on the project.&nbsp;


Consider defining the following on a Schedule:



* Holidays
* Time off
* Number of hours available for work during a day, or week


Knowing when users are available to work is important in understanding the progress of your tasks on the project.&nbsp;


You can create multiple project schedules and apply a default schedule to the project. Additional custom schedules may be applied to different individuals.


For more information about Schedules, see the article [Create a schedule](create-schedules.md).


### Manage additional information needed for planning the project {#manage-additional-information-needed-for-planning-the-project}

When planning a project, there is additional information that must be set up before you can start working on the project.&nbsp;


Consider asking the following questions:



* Is there a regulation that mandates that you keep a record of events and processes? If so, what are you required to track?  
  *`Workfront`* lets you record edits, scope changes, status changes, and actions so you can comply with the regulations specific to your industry.  
  For more information about defining what updates to track in *`Workfront`*, see the article [System-tracked updates](system-tracked-update-feeds.md).

* Is there any information that you are required to track that does not have a field in *`Workfront`* to store it in?! If yes, create Custom Forms for projects or tasks where you can store this information.  
  For more information about creating custom forms, see the article [Create or edit a custom form](create-or-edit-a-custom-form.md).

* Are there any approval check points that must be granted before the work on a project can continue?&nbsp;If yes, create Approval Processes for projects or tasks that you can use as you're building your project.  
  For more information about Approval Processes, see the article [Create an approval process](create-approval-processes.md).





## Build the project timeline {#build-the-project-timeline}

After you determine the major objectives of a project, and you have decided that the project is worth pursuing, you should calculate the timeline for each objective. Each objective can become one of your tasks on the project.


This helps prioritize your objectives and plan your Work Breakdown Structure accordingly. The Work Breakdown Structure defines the timeline of the project.  
For more information about creating tasks on a project, see the article [Define tasks](#define-tasks).


Consider the following when building the timeline of the project:



* Break down larger objectives into children tasks and define their Start and their Completion dates.
*  Determine whether your objectives have dependencies on other objectives. 


  You can set up those dependencies as predecessors.


  For example, you might have a project to build an apartment building. One of your objectives includes the plumbing and another is laying the foundation. One of your plumbing tasks is to hook up to the main city water line and this must be done prior to laying the foundation. However, most of your other plumbing tasks cannot be done until after the foundation is laid. In this case, you should consider using predecessors to understand when one objective can start after its prerequisite has finished.


  When you use parent tasks to organize objectives, you can create one task for each major objective, and add sub-tasks when you get to the stage of breaking major objectives into individual tasks. This keeps the tasks that are part of the objective organized within the project.&nbsp;


  For more information about task predecessors, see [Overview of task predecessors](predecessors-overview.md).

*  Consider the most important objectives for your project, and flag them as milestone tasks.


  We recommend using parent tasks as milestones. 


  For more information about using milestone tasks, see [Create a milestone path](create-milestone-path.md).

* Define a timeline for each objective. If you work with parent tasks, each child task must have a defined Start and Completion Date. The time between the earliest Start Date of a task and the latest Completion Date of a task on the same project results in the project timeline.&nbsp;




## Define tasks {#define-tasks}

As you are defining the objectives of your project and the tasks associated with them you are creating the project timeline.&nbsp;


You can create tasks on a project in the following ways:



* Add tasks to a project in inline edit.
*  Use a Template with defined Template Tasks and add it to your project.&nbsp;


  The Template Tasks become the Tasks of the Project.&nbsp;


  For more information about creating tasks, see the article [Create tasks in a project](create-tasks-in-project.md).



When defining tasks, consider the following:



*  Define the timeline of each task. This is captured in the Duration field of each task. 


  For information about task Duration, see the article [Overview of Task Duration and Duration Type](task-duration-and-duration-type.md). 

* Define the parent-child relationship between the tasks.
* Define the predecessor relationship between the tasks.
*  Associate a Milestone Path with the project and associate a Milestone with its respective task.&nbsp;


  For more information about using milestone tasks, see the article [Create a milestone path](create-milestone-path.md).

*  Define the amount of work needed to complete each task. This is captured in the Planned Hours field of each task.


  For more information about Planned Hours, see the article [Planned Hours overview](planned-hours.md).

* Assign each task to a user or team who is responsible for completing it.&nbsp;
* Check the availability of the users you are assigning to the tasks. Ensure they are free to work and not overallocated so they can complete their assigned tasks. If users are overallocated or they have time off in their schedules, consider one of the following: 
    
    
    * Reduce the Planned Hours of each task.
    * Add more users to a task to ensure it can be completed during the time allocated for it.
    * Reassign the tasks to users who are available with no other constraints.  
      For more information about planning your project resources, see the article [Resource Planning in Adobe Workfront](_resource-planning-overview.md).  
      For more information about scheduling your resources to accomplish the work on a project, see the article [Resource Scheduling](_resource-scheduling-overview.md).
    
    


