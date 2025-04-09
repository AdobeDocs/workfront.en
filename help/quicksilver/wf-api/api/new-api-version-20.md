---
content-type: api
navigation-topic: api-navigation-topic
title: What's new in API version 20
description: Adobe Workfront released API version 20 on April 6, 2022. API version 20 features the following changes from version 19.
author: Becky
feature: Workfront API
role: Developer
---
# What's new in API version 20

Adobe Workfront released API version 20 on April 8, 2024. API version 20 features the following changes from version 19.

## Added resources

### AssignmentBillingRole (ASBLRL)



### StaffingPlan (STAFFP)



### StaffingPlanResource (STAFFR)




## Removed resources

No resources were removed for API version 20

## Modified resources

### AccessLevelPermissions (ALVPER)

An AccessLevelPermissions object represents a specific permission to access, create, or modify a Workfront object. These permissions can then be associated with an Access Level.



### AccessRequest (ACSREQ)

If a User does not have access to an object in Workfront that they need, they can request access to that object. The AccessRequest object represents this request.



### AccessRule (ACSRUL)

An AccessRule object represents a rule set in custom access levels that determines how users can share projects they create.



### AnnouncementAttachment



### Approval (APPROVAL)

A given work item, such as a task, document, or timesheet, may require that a supervisor or other user sign off on the work item. An Approval object represents the action of signing off on a work item.



### Assignment (ASSGN)

An Assignment object represents the connection between a work item and the user, team, or group that is assigned to work on it.



### Avatar



### Baseline (BLIN)

Baselines are snapshots of what the performance of a project looked like at a given moment in time. They store key pieces of information about the project, like key dates, progress, cost and revenue values. 



### BaselineTask (BSTSK)

Baselines are snapshots of what the performance of a project looked like at a given moment in time. They store key pieces of information about the project, like key dates, progress, cost and revenue values. When you create a baseline, the task information is also captured on the baseline tasks of that baseline.



### BillingRecord (BILL)

A BillingRecord object records the revenue, hours, or expenses that can be billed. This information can be used to create invoices in an external accounting system.



### Category (CTGY)

A Category object is a custom form.



### CategoryParameter (CTGYPA)



### Company (CMPY)

A Company object represents an organization consisting of a collection of people.




### CustomerPreferences (CUSTPR)

A CustomerPreferences object represents the set of preferences that a customer has set for their instance of Workfront.



### ExchangeRate (EXRATE)

An ExchangeRate object represents a currency exchange rate set up in Workfront. ExchangeRate objects are not dynamic.



### FinancialData (FINDAT)



### Group (GROUP)

A Group object represents a set of users and teams. Groups often represent departmental structure.



### Hour (HOUR)

An Hour object represents an hour logged by a user on a timesheet.



### OpTask (OPTASK)

An OpTask object is commonly known as an Issue. An issue is a work item that usually indicates that there is a problem preventing the completion of a task or project. An Issue can also be a Help Desk request. Change Orders, Requests, and Bugs are also Issues.



### Parameter (PARAM)

A Parameter object is a custom field.



### Portfolio (PORT)

A Portfolio object is a collection of projects that compete for the same resources, typically money or people to complete them.


### Program (PRGM)

A Program object is a subset of projects within a portfolio, where similar projects can be grouped together.



### Project (PROJ)

Projects are work items within Workfront, and are a main building block in the way Workfront helps people to do work. A Project object represents a group of tasks with a common, specific goal.



### QueueDef (QUED)

A QueueDef object represents a Queue, which is a project that has been published to the Help Desk area to allow users to submit issues to it.



### Rate (RATE)

A Rate object represents a billing rate in Workfront.



### Role (ROLE)

A Role object (job role) represents a functional capacity or a skill set a user might fill, such as Designer or Product Manager.



### ScheduledReport

A ScheduledReport object represents a report that has been configured to be scheduled for delivery.



### ScoreCardQuestion

A ScoreCardQuestion object represents a question that has been added to a Scorecard. These questions are usually determined by the Portfolio manager, and their answers allow the manager to understand how well a project aligns with the goals of the portfolio.



### Task (TASK)

A Task object represents a work item that must be performed as a step toward achieving a final goal (completing a Project).



### Template (TMPL)

A Template object represents a pattern for a project. Projects can be created from templates to save time. A template contains a team and tasks, which will be copied to any project created from the template.



### TemplateTask (TTSK)

A TemplateTask object represents a Task that is part of a Template. Template Tasks become Tasks in the Project where the Template is used.



### Timesheet (TSHET)

A Timesheet object represents a virtual timecard that allows Users to enter actual hours worked for Tasks, Projects, and overhead Hour Types.



### Update (UPDATE)

Work Items in Workfront can be updated to keep users informed of the current status. An Update object represents one of these updates. Updates can be entered by users or created by the Workfront system.



### User (USER)

A User object represents a person with an account in Workfront that can log in and interact with the system.



### Work (WORK)

A Work object is a common interface that both Task and OpTask inherit, and shares common code between the two.



