---
content-type: api
navigation-topic: api-navigation-topic
title: Updates to API Version 8
description: The following existing resources have been updated with this release of the Adobe Workfront API. To view the resources that are new to versions 8, please see What's New in API Version 8. Changes made to a resource are indicated in the following manner - EDIT ME.
author: Becky
feature: Workfront API
role: Developer
exl-id: c6d7d2d2-cd21-4ca8-a5a0-afe3669dc959
---
# Updates to API Version 8

## Updated Resources

The following existing resources have been updated with this release of the Adobe Workfront API. To view the resources that are new to versions 8, please see [What's New in API Version 8](../../wf-api/api/new-api-version-8.md). Changes made to a resource are indicated in the following manner:

* Additions are simply listed
* Removals are indicated with strikethrough text
* Changes are noted in the note after the table

### AccessRequest

| Fields |References |Collections |Search |Actions |Queries |Operations |
|---|---|---|---|---|---|---|
| action<sup>1</sup>&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |

{style="table-layout:auto"}

<sup>1</sup> Changes to possible values

### AccessRule<sup>1</sup>&nbsp;

| Fields |References |Collections |Search |Actions |Queries |Operations |
|---|---|---|---|---|---|---|
| coreAction<sup>2</sup>&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |
| forbiddenActions<sup>2</sup> |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |
| secondaryActions<sup>2</sup> |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |

{style="table-layout:auto"}

<sup>1</sup> Flag removed: REPORTABLE   
<sup>2</sup> Changes to possible values

### Approval

| Fields |References |Collections |Search |Actions |Queries |Operations |
|---|---|---|---|---|---|---|
| auditTypes<sup>1</sup> |agileWork&nbsp; |resourcePools |&nbsp; |&nbsp; |&nbsp; |&nbsp; |
| backlogOrder<sup>2</sup> |kanbanBoard&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |
| backlogParent |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |
| kanbanBoardID |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |

{style="table-layout:auto"}

<sup>1</sup>Changes to possible values   
<sup>2</sup>Flags added: DYNAMIC, LAZY_READ, and NOT_GROUPABLE

### Assignment

| &nbsp; |&nbsp; |&nbsp; |&nbsp; |Fields |References |Collections |Search |Actions |Queries |Operations |
|---|---|---|---|---|---|---|---|---|---|---|
| &nbsp; |&nbsp; |&nbsp; |&nbsp; |assignUserToRoleOnTasks |getAssignAssignmentsForTasks&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |
| &nbsp; |&nbsp; |&nbsp; |&nbsp; |swapUsersOnTasks |getUnassignAssignmentsForTasks |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |
| &nbsp; |&nbsp; |&nbsp; |&nbsp; |unassignUserFromTasks |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |

{style="table-layout:auto"}

### Customer

| Fields |References |Collections |Search |Actions |Queries |Operations |
|---|---|---|---|---|---|---|
| bizRuleExclusions<sup>1</sup> |&nbsp; |&nbsp; |&nbsp; |getPackagingOptionValue |&nbsp; |&nbsp; |
| proofPlan<sup>1</sup> |&nbsp; |&nbsp; |&nbsp; |isPackagingOptionEnabled |&nbsp; |&nbsp; |

{style="table-layout:auto"}

<sup>1</sup>Changes to possible values

### CustomerPreferences

| Fields |References |Collections |Search |Actions |Queries |Operations |
|---|---|---|---|---|---|---|
| name<sup>1</sup> |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |

{style="table-layout:auto"}

<sup>1</sup>Changes to possible values

### DocumentApproval

| Fields |References |Collections |Search |Actions |Queries |Operations |
|---|---|---|---|---|---|---|
| ID<sup>1</sup> |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |

{style="table-layout:auto"}

<sup>1</sup>Flag added: NOT_FILTERABLE

### DocumentVersion

| Fields |References |Collections |Search |Actions |Queries |Operations |
|---|---|---|---|---|---|---|
| activeProofStages |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |

{style="table-layout:auto"}

### Group

| Fields |References |Collections |Search |Actions |Queries |Operations |
|---|---|---|---|---|---|---|
| &nbsp; |&nbsp; |owners |&nbsp; |&nbsp; |&nbsp; |&nbsp; |

{style="table-layout:auto"}

### HourType

| Fields |References |Collections |Search |Actions |Queries |Operations |
|---|---|---|---|---|---|---|
| appGlobalID<sup>1</sup> |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |

{style="table-layout:auto"}

<sup>1</sup>Flag added: NOT_FILTERABLE

### Iteration

| Fields |References |Collections |Search |Actions |Queries |Operations |
|---|---|---|---|---|---|---|
| &nbsp; |&nbsp; |&nbsp; |&nbsp; |moveStories |&nbsp; |&nbsp; |

{style="table-layout:auto"}

### Like

| Fields |References |Collections |Search |Actions |Queries |Operations |
|---|---|---|---|---|---|---|
| `endorsementID`  |`endorsement`  |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |

{style="table-layout:auto"}

### Note

| Fields |References |Collections |Search |Actions |Queries |Operations |
|---|---|---|---|---|---|---|
| auditType<sup>1</sup> |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |

{style="table-layout:auto"}

<sup>1</sup>Changes to possible values

### OpTask

| Fields |References |Collections |Search |Actions |Queries |Operations |
|---|---|---|---|---|---|---|
| auditTypes<sup>1</sup> |agileWork&nbsp; |&nbsp; |&nbsp; |&nbsp; |defaultShownTimesheetIssues&nbsp; |&nbsp; |
| backlogOrder |iteration |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |
| backlogParent |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |
| estimate |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |
| iterationID |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |

{style="table-layout:auto"}

<sup>1</sup>Changes to possible values

### Portfolio

| Fields |References |Collections |Search |Actions |Queries |Operations |
|---|---|---|---|---|---|---|
| auditTypes<sup>1</sup> |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |

{style="table-layout:auto"}

<sup>1</sup>Changes to possible values

### Program

| Fields |References |Collections |Search |Actions |Queries |Operations |
|---|---|---|---|---|---|---|
| auditTypes<sup>1</sup> |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |

{style="table-layout:auto"}

<sup>1</sup>Changes to possible values

### Project

| Fields |References |Collections |Search |Actions |Queries |Operations |
|---|---|---|---|---|---|---|
| auditTypes<sup>1</sup> |&nbsp; |resourcePools |&nbsp; |&nbsp; |defaultShownTimesheetProjects |&nbsp; |

{style="table-layout:auto"}

<sup>1</sup>Changes to possible values

### ProofApproval

| Fields |References |Collections |Search |Actions |Queries |Operations |
|---|---|---|---|---|---|---|
| approverID |approver |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |
| documentVersionID |documentVersion |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |
| ID<sup>1</sup> |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |
| proofCreationDate |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |

{style="table-layout:auto"}

<sup>1</sup>Flag added: NOT_FILTERABLE

### QueueDef

| Fields |References |Collections |Search |Actions |Queries |Operations |
|---|---|---|---|---|---|---|
| requestorCoreAction<sup>1</sup> |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |
| requestorForbiddenActions<sup>1</sup> |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |

{style="table-layout:auto"}

<sup>1</sup>Changes to possible values

### Rate

| Fields |References |Collections |Search |Actions |Queries |Operations |
|---|---|---|---|---|---|---|
| endDate |&nbsp; |&nbsp; |&nbsp; |setRatesForRole&nbsp; |&nbsp; |&nbsp; |
| name |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |
| startDate |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |

{style="table-layout:auto"}

### ReservedTime

| Fields |References |Collections |Search |Actions |Queries |Operations |
|---|---|---|---|---|---|---|
| extRefID |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |

{style="table-layout:auto"}

### ResourceManager

| Fields |References |Collections |Search |Actions |Queries |Operations |
|---|---|---|---|---|---|---|
| projectPriority |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |

{style="table-layout:auto"}

### Task

| Fields |References |Collections |Search |Actions |Queries |Operations |
|---|---|---|---|---|---|---|
| auditTypes<sup>1</sup> |agileWork&nbsp; |&nbsp; |&nbsp; |&nbsp; |allTasksOnIterations&nbsp; |&nbsp; |
| backlogParent |kanbanBoard |&nbsp; |&nbsp; |&nbsp; |defaultShownTimesheetTasks |&nbsp; |
| kanbanBoardID |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |

{style="table-layout:auto"}

<sup>1</sup>Changes to possible values

### Team

| Fields |References |Collections |Search |Actions |Queries |Operations |
|---|---|---|---|---|---|---|
| agileMethodology |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |
| autoAddNextStory |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |
| includeIssues |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |
| teamStoryBoardIssueStatuses |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |
| wipLimit |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |

{style="table-layout:auto"}

### Template

| Fields |References |Collections |Search |Actions |Queries |Operations |
|---|---|---|---|---|---|---|
| &nbsp; |&nbsp; |resourcePools |&nbsp; |&nbsp; |&nbsp; |&nbsp; |

{style="table-layout:auto"}

### TemplateTask

| Fields |References |Collections |Search |Actions |Queries |Operations |
|---|---|---|---|---|---|---|
| auditTypes<sup>1</sup> |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |

{style="table-layout:auto"}

<sup>1</sup>Changes to possible values

Update 

| Fields |References |Collections |Search |Actions |Queries |Operations |
|---|---|---|---|---|---|---|
| updateType<sup>1</sup> |`updateEndorsement`  |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |

{style="table-layout:auto"}

<sup>1</sup>Changes to possible values

### User

| &nbsp; |&nbsp; |Fields |References |Collections |Search |Actions |Queries |Operations |
|---|---|---|---|---|---|---|---|---|
| &nbsp; |&nbsp; |resourcePools |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |
| &nbsp; |&nbsp; |userGroups |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |
| &nbsp; |&nbsp; |userRoles |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |

{style="table-layout:auto"}

### UserNote

| Fields |References |Collections |Search |Actions |Queries |Operations |
|---|---|---|---|---|---|---|
| `endorsementID`  |`endorsement`  |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |
| `endorsementShareID`  |`endorsementShare`  |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |
| eventType<sup>1</sup> |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |

{style="table-layout:auto"}

<sup>1</sup>Changes to possible values

### Work

| Fields |References |Collections |Search |Actions |Queries |Operations |
|---|---|---|---|---|---|---|
| auditTypes<sup>1</sup> |agileWork&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |
| backlogOrder<sup>2</sup> |kanbanBoard&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |
| backlogParent&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |
| kanbanBoardID |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |

{style="table-layout:auto"}

<sup>1</sup>Changes to possible values   
<sup>2</sup>Flags added: DYNAMIC, LAZY_READ, and NOT_GROUPABLE
