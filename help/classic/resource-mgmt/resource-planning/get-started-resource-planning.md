---
filename: get-started-resource-planning
content-type: overview
product-area: resource-management
navigation-topic: resource-planning
title: Get started with Resource Planning
description: You can use the Adobe Workfront Resource Management tools to forecast the allocation of your resources so that you know with accuracy whether your projects are delivered on time and on budget. For an overview of Resource Management in Workfront, see Get started with Resource Management .
---

# Get started with Resource Planning

You can use the Adobe Workfront Resource Management tools to forecast the allocation of your resources so that you know with accuracy whether your projects are delivered on time and on budget. For an overview of Resource Management in Workfront, see [Get started with Resource Management](../../resource-mgmt/resource-mgmt-overview/get-started-resource-management.md).

You can use resource planning tools to manage your job roles, their availability, and general allocation to projects based on this availability.

Budgeting users' general allocation to projects does not assign them to actual work (tasks and issues). You must assign your resources to work by using the Resource Scheduling tools.

For more information about scheduling resources in Workfront, see [Resource Scheduling](../../resource-mgmt/resource-scheduling/resource-scheduling-overview.md) .

## Resource planning tools in&nbsp;Workfront

To budget time for your resources for the projects you plan to assign them to, you can use the following tools:

* For budgeting allocations for and prioritize multiple projects at the system-level: use the system-level Resource Planner.

  You can access the Resource Planner by going to the Resource Planner subtab in the Peoplearea.

  For information about the Resource Planner, see [Resource Planner overview](../../resource-mgmt/resource-planning/get-started-resource-planner.md).

* For budgeting allocations for a single project: use the&nbsp;project-level Resource Planner in the Resource Budgeting area of the Business Case of a the project. For information about budgeting resources for one project, see the article [Budget resources in the Business Case](../../manage-work/projects/define-a-business-case/budget-resources-in-business-case.md).

  To manage users and organize them in pools based on common skills or departmental structure and then manage their allocations for the projects they are assigned to, you must create resource pools.&nbsp;For more information about creating resource pools, see [Create resource pools in Adobe Workfront](../../resource-mgmt/resource-planning/resource-pools/create-resource-pools.md).

  >[!TIP]
  >
  >The Resource Budgeting area of a project is the Resource Planner at the project level. When you budget resources in the Business Case of a project, the information is also reflected in the system-level Resource Planner.

## The purpose of the resource planning tools

* Using the Resource Planner you can do the following:

  * Prioritize your projects to decide which projects should receive resources first. (Only in the Resource Planner)
  * Understand the availability of your resources based on the schedule of your users.
  * Budget hour, FTE, or cost allocations for your resources (users and job roles) for the projects to which they are assigned.

  For information about working in the Resource Planner, see the article [Resource Planner overview](../../resource-mgmt/resource-planning/get-started-resource-planner.md).

<!--
Prerequisites for resource planning
-->

<!--
To successfully use the Resource Planner for budgeting your resources, you must first ensure that you, your projects, and your tasks meet a set of prerequisites. These prerequisites are mandatory to display the correct information in the Resource Planner and to accurately manage your resources.
-->

<!--
Important: If any of the following prerequisites are missing, you might find that some of the information about the allocation or the availability of the resources is missing or has a zero value. For more information understanding why fields are missing data or have zero values, hover over the fields.
-->

<!--

-->

<!--
Note: The following prerequisites are required only when viewing the Resource Planner by project or by job role or when budgeting resources in the Business Case of a project. For more information about the views in the Resource Planner, see the "Project/ Role/ User view" selection section in the article Resource Planner overview.
-->

<!--
The following types of prerequisites are required for the correct functionality of the Resource Planner:
-->

  <!--
  User prerequisites
  -->

  <!--
  Project prerequisites
  -->

  <!--
  Tasks and issues prerequisites
  -->

<!--
User prerequisites
-->

<!--
Ensure the following user setup exists before starting using the Resource Planner:
-->

`<li>  <ul>   <li> <!--    You have the correct access to budget resources.   --> <!--    For information about the access needed to budget resources, see the article Access needed to budget resources.   --> </li>  </ul> </li>`

* 

  <!--
  Users who are assigned to tasks are added to the Resource Pools associated with the project.
  -->

  <!--
  For information about adding users to Resource Pools, see Associate resource pools with users in Adobe Workfront and Create resource pools in Adobe Workfront.
  -->

  >[!NOTE]
  >
  >
  >
  ><!--  >
  >When users are not added to Resource Pools, the following scenarios may exist:  >
  >-->  >
  >
  >
  >  
  >  
  >  
  >  
  >    <!--  >  
  >    The users do not appear in the Resource Planner although they might be assigned to tasks on the projects.  >  
  >    -->  >  
  >  
  >  
  >  
  >    <!--  >  
  >    If the tasks they are associated with have Planned Hours, those hours do not appear for the project in the Resource Planner, unless the user is also associated with a job role on those tasks.  >  
  >    -->  >  
  >  
  >  
  >  
  >    <!--  >  
  >    If the users are associated with a job role on a task on the project, the Planned Hours display in the Resource Planner for the job role, but the job role cannot be budgeted.  >  
  >    -->  >  
  >  
  >  
  >

* 

  <!--
  Users who are assigned to work and Resource Pools must have Schedules and Job Roles associated with their profile.
  -->

  <!--
  For information about associating Schedules and Job Roles with users, see the article Add users
  -->

  <!--
  Note: Users who are not associated with a Schedule but are in the Resource Pool of the project cannot be budgeted in the Resource Planner.
  -->

* 

  <!--
  For accurate Available Hours information, ensure that the schedules associated with your users have the schedule exceptions and time off updated.
  -->

  <!--
  Note: If a user is not associated with a Schedule, the Default Schedule of your Workfront system is associated with the user by default, for the purposes of the Resource Planner.
  -->

  <!--
  For information about creating schedules, see the article Create a schedule.
  -->

  <!--
  If you want to budget your resources by Cost, you must associate Job Roles with Cost/Hr. rates. The cost associated with Job Roles assigned to users in your Resource Pools is used to calculate the Budgeted Labor Cost and the Budgeted Cost of the project. For information about associating job roles with rates, see the article Create and manage job roles. For information about calculating Budgeted Labor Cost, see the article Understand Budgeted Labor Cost and Budgeted Hours for projects. For information about calculating Budgeted Cost, see the article Calculate Budgeted Cost.
  -->

<!--
Project prerequisites
-->

<!--
Ensure the following project setup exists before starting using the Resource Planner:
-->

  <!--
  Your projects are associated with Resource Pools. For more information about adding Resource Pools to projects, see Associate resource pools with projects and templates in Adobe Workfront. Important: Projects without Resource Pools do not display Planned Hour or assignments information in the Resource Planner.
  -->

* 

  <!--
  You have the correct access to budget resources.
  -->

  <!--
  For information about the access needed to budget resources, see the article Access needed to budget resources.
  -->

<!--
Tasks and issues prerequisites
-->

<!--
Ensure the following tasks and issues setup exists before starting budgeting resources in the Resource Planner:
-->

  <!--
  The tasks or issues on the projects for which you are budgeting resources are assigned to one of these entities: Users in the Resource Pools of the project who are also associated with Job Roles Job Roles Note: Teams assigned to tasks or issues do not display in the Resource Planner. The Planned Hours of tasks and issues assigned to job roles display in the Resource Planner, but these hours cannot be budgeted unless a user who is associated with the job role is listed in a Resource Pool associated with the project.
  -->

* 

  <!--
  Parent tasks should not be assigned to users or roles.
  -->

  <!--
  This will impact the value of Planned Hours for the project.
  -->

  <!--
  Tasks and issues have a value for Planned Hours which is greater than zero.
  -->

  <!--
  Tasks and issues have a value for their Duration which is greater than zero.
  -->

  <!--
  The Planned Dates of the issues are within the timeline of the project.
  -->

<!--
Access resource planning tools in Workfront
-->

<!--
You can access the Planner from the Resource Planner subtab of the Resourcing area.
-->

<!--
For information about accessing the Planner, see Resource Planner overview.
-->

<!--
Create Resource Pools You can manage your user resources by adding users to Resource Pools. Having users organized in Resource Pools and associating the pools with your projects are prerequisites to Resource Planning. For information about adding users to Resource Pools and associating them with projects, see Create resource pools in Adobe Workfront and Associate resource pools with users in Adobe Workfront.
-->

