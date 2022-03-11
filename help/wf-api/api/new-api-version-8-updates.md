---
filename: new-api-version-8-updates
content-type: api
navigation-topic: api-navigation-topic
title: Updates to API Version 8
description: The following existing resources have been updated with this release of the Adobe Workfront API. To view the resources that are new to versions 8, please see What's New in API Version 8. Changes made to a resource are indicated in the following manner:
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
| action¹&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |

`¹ Changes to possible values`

### AccessRule¹&nbsp;

| Fields |References |Collections |Search |Actions |Queries |Operations |
|---|---|---|---|---|---|---|
| coreAction²&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |
| forbiddenActions² |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |
| secondaryActions² |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |

`¹ Flag removed: REPORTABLE`   
`² Changes to possible values`

### Approval

| Fields |References |Collections |Search |Actions |Queries |Operations |
|---|---|---|---|---|---|---|
| auditTypes¹ |agileWork&nbsp; |resourcePools |&nbsp; |&nbsp; |&nbsp; |&nbsp; |
| backlogOrder² |kanbanBoard&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |
| backlogParent |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |
| kanbanBoardID |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |

`¹Changes to possible values`   
`²Flags added: DYNAMIC, LAZY_READ, and NOT_GROUPABLE`

### Assignment

| &nbsp; |&nbsp; |&nbsp; |&nbsp; |Fields |References |Collections |Search |Actions |Queries |Operations |
|---|---|---|---|---|---|---|---|---|---|---|
| &nbsp; |&nbsp; |&nbsp; |&nbsp; |assignUserToRoleOnTasks |getAssignAssignmentsForTasks&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |
| &nbsp; |&nbsp; |&nbsp; |&nbsp; |swapUsersOnTasks |getUnassignAssignmentsForTasks |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |
| &nbsp; |&nbsp; |&nbsp; |&nbsp; |unassignUserFromTasks |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |

### Customer

| Fields |References |Collections |Search |Actions |Queries |Operations |
|---|---|---|---|---|---|---|
| bizRuleExclusions¹ |&nbsp; |&nbsp; |&nbsp; |getPackagingOptionValue |&nbsp; |&nbsp; |
| proofPlan¹ |&nbsp; |&nbsp; |&nbsp; |isPackagingOptionEnabled |&nbsp; |&nbsp; |

`¹Changes to possible values`

### CustomerPreferences

| Fields |References |Collections |Search |Actions |Queries |Operations |
|---|---|---|---|---|---|---|
| name¹ |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |

`¹Changes to possible values`

### DocumentApproval

| Fields |References |Collections |Search |Actions |Queries |Operations |
|---|---|---|---|---|---|---|
| ID¹ |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |

`¹Flag added: NOT_FILTERABLE`

### DocumentVersion

| Fields |References |Collections |Search |Actions |Queries |Operations |
|---|---|---|---|---|---|---|
| activeProofStages |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |

### Group

| Fields |References |Collections |Search |Actions |Queries |Operations |
|---|---|---|---|---|---|---|
| &nbsp; |&nbsp; |owners |&nbsp; |&nbsp; |&nbsp; |&nbsp; |

### HourType

| Fields |References |Collections |Search |Actions |Queries |Operations |
|---|---|---|---|---|---|---|
| appGlobalID¹ |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |

`¹Flag added: NOT_FILTERABLE`

### Iteration

| Fields |References |Collections |Search |Actions |Queries |Operations |
|---|---|---|---|---|---|---|
| &nbsp; |&nbsp; |&nbsp; |&nbsp; |moveStories |&nbsp; |&nbsp; |

### Like

| Fields |References |Collections |Search |Actions |Queries |Operations |
|---|---|---|---|---|---|---|
| `<del>endorsementID</del>`  |`<del>endorsement</del>`  |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |

### Note

| Fields |References |Collections |Search |Actions |Queries |Operations |
|---|---|---|---|---|---|---|
| auditType¹ |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |

`¹Changes to possible values`

### OpTask

| Fields |References |Collections |Search |Actions |Queries |Operations |
|---|---|---|---|---|---|---|
| auditTypes¹ |agileWork&nbsp; |&nbsp; |&nbsp; |&nbsp; |defaultShownTimesheetIssues&nbsp; |&nbsp; |
| backlogOrder |iteration |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |
| backlogParent |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |
| estimate |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |
| iterationID |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |

`¹Changes to possible values`

### Portfolio

| Fields |References |Collections |Search |Actions |Queries |Operations |
|---|---|---|---|---|---|---|
| auditTypes¹ |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |

`¹Changes to possible values`

### Program

| Fields |References |Collections |Search |Actions |Queries |Operations |
|---|---|---|---|---|---|---|
| auditTypes¹ |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |

`¹Changes to possible values`

### Project

| Fields |References |Collections |Search |Actions |Queries |Operations |
|---|---|---|---|---|---|---|
| auditTypes¹ |&nbsp; |resourcePools |&nbsp; |&nbsp; |defaultShownTimesheetProjects |&nbsp; |

`¹Changes to possible values`

### ProofApproval

| Fields |References |Collections |Search |Actions |Queries |Operations |
|---|---|---|---|---|---|---|
| approverID |approver |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |
| documentVersionID |documentVersion |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |
| ID¹ |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |
| proofCreationDate |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |

`¹Flag added: NOT_FILTERABLE`

### QueueDef

| Fields |References |Collections |Search |Actions |Queries |Operations |
|---|---|---|---|---|---|---|
| requestorCoreAction¹ |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |
| requestorForbiddenActions¹ |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |

`¹Changes to possible values`

### Rate

| Fields |References |Collections |Search |Actions |Queries |Operations |
|---|---|---|---|---|---|---|
| endDate |&nbsp; |&nbsp; |&nbsp; |setRatesForRole&nbsp; |&nbsp; |&nbsp; |
| name |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |
| startDate |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |

### ReservedTime

| Fields |References |Collections |Search |Actions |Queries |Operations |
|---|---|---|---|---|---|---|
| extRefID |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |

### ResourceManager

| Fields |References |Collections |Search |Actions |Queries |Operations |
|---|---|---|---|---|---|---|
| projectPriority |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |

### Task

| Fields |References |Collections |Search |Actions |Queries |Operations |
|---|---|---|---|---|---|---|
| auditTypes¹ |agileWork&nbsp; |&nbsp; |&nbsp; |&nbsp; |allTasksOnIterations&nbsp; |&nbsp; |
| backlogParent |kanbanBoard |&nbsp; |&nbsp; |&nbsp; |defaultShownTimesheetTasks |&nbsp; |
| kanbanBoardID |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |

`¹Changes to possible values`

### Team

| Fields |References |Collections |Search |Actions |Queries |Operations |
|---|---|---|---|---|---|---|
| agileMethodology |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |
| autoAddNextStory |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |
| includeIssues |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |
| teamStoryBoardIssueStatuses |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |
| wipLimit |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |

### Template

| Fields |References |Collections |Search |Actions |Queries |Operations |
|---|---|---|---|---|---|---|
| &nbsp; |&nbsp; |resourcePools |&nbsp; |&nbsp; |&nbsp; |&nbsp; |

### TemplateTask

| Fields |References |Collections |Search |Actions |Queries |Operations |
|---|---|---|---|---|---|---|
| auditTypes¹ |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |

`¹Changes to possible values`

`Update` 

| Fields |References |Collections |Search |Actions |Queries |Operations |
|---|---|---|---|---|---|---|
| updateType¹ |`<del>updateEndorsement</del>`  |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |

`¹Changes to possible values`

### User

| &nbsp; |&nbsp; |Fields |References |Collections |Search |Actions |Queries |Operations |
|---|---|---|---|---|---|---|---|---|
| &nbsp; |&nbsp; |resourcePools |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |
| &nbsp; |&nbsp; |userGroups |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |
| &nbsp; |&nbsp; |userRoles |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |

### UserNote

| Fields |References |Collections |Search |Actions |Queries |Operations |
|---|---|---|---|---|---|---|
| `<del>endorsementID</del>`  |`<del>endorsement</del>`  |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |
| `<del>endorsementShareID</del>`  |`<del>endorsementShare</del>`  |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |
| eventType¹ |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |

`¹Changes to possible values`

### Work

| Fields |References |Collections |Search |Actions |Queries |Operations |
|---|---|---|---|---|---|---|
| auditTypes¹ |agileWork&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |
| backlogOrder² |kanbanBoard&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |
| backlogParent&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |
| kanbanBoardID |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |

`¹Changes to possible values`   
`²Flags added: DYNAMIC, LAZY_READ, and NOT_GROUPABLE`
