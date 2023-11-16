---
content-type: api
navigation-topic: api-navigation-topic
title: Updates to API Version 9
description: Updated Resources
author: Becky
feature: Workfront API
role: Developer
exl-id: 51892846-d93f-4363-8416-4118fb2ef84d
---
# Updates to API Version 9

## Updated Resources

The following existing resources have been updated with this release of the Adobe Workfront API. To view the resources that are new to version 9 you can visit [What's New in API Version 9](../../wf-api/api/new-api-version-9.md) and [What's New in API Version 9 (continued)](../../wf-api/api/new-api-version-9-continue.md). Changes made to a resource are indicated in the following manner:

* Additions are simply listed
* Removals are indicated with strikethrough text
* Changes are noted in the note after the table

### AgileWork

| Fields |References |Collections |Search |Actions |Queries |Operations |
|---|---|---|---|---|---|---|
| `opTaskID`<sup>2</sup> |  |   |  |   |   |  |
| `taskID`<sup>2</sup>  |   |   |  |  |  |  |

{style="table-layout:auto"}

<sup>1</sup> Flag removed: REPORTABLE   
<sup>2</sup> Flag removed: NOT_GROUPABLE

### Approval

| Fields |References |Collections |Search |Actions |Queries |Operations |
|---|---|---|---|---|---|---|
| `storyBoardOrder`  | `agileWork`  |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |

{style="table-layout:auto"}

Assignment

| Fields |References |Collections |Search |Actions |Queries |Operations |
|---|---|---|---|---|---|---|
| |   |  |  | `assignUserToRoleOnProjects`<sup>1</sup> |   |   |
|   |   |   |   | `assignUserToRoleOnTasks`<sup>1</sup>  |   |   |
|   |   |   |   | `swapUsersOnProjects`<sup>1</sup>  |   |   |
|   |   |   |   | `swapUsersOnTasks`<sup>1</sup>  |   |   |

{style="table-layout:auto"}

<sup>1</sup> Added field: lockToRole

### CustomerPreferences

| Fields |References |Collections |Search |Actions |Queries |Operations |
|---|---|---|---|---|---|---|
| `name`<sup>1</sup>  |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |

{style="table-layout:auto"}

<sup>1</sup> Changes to possibleValues

### Hour

| Fields |References |Collections |Search |Actions |Queries |Operations |
|---|---|---|---|---|---|---|
| `days`  |   |   |   |   |   |   |
| `workHoursPerDay`  |   |   |   |   |   |   |

{style="table-layout:auto"}

### Iteration

| Fields |References |Collections |Search |Actions |Queries |Operations |
|---|---|---|---|---|---|---|
|   |   |   |   | `moveIssues`  |   |   |

{style="table-layout:auto"}

### LayoutTemplates

| Fields |References |Collections |Search |Actions |Queries |Operations |
|---|---|---|---|---|---|---|
| `groupID`  | `group`  |   |   |   |   |   |

{style="table-layout:auto"}

### Note

| Fields |References |Collections |Search |Actions |Queries |Operations |
|---|---|---|---|---|---|---|
| `html`  |   |   |   |   |   |   |
| `json`  |   |   |   |   |   |   |
| `richTextNoteID`  |   |   |   |   |   |   |

{style="table-layout:auto"}

### OpTask

| Fields |References |Collections |Search |Actions |Queries |Operations |
|---|---|---|---|---|---|---|
| `color`  | `agileWork`  |   |   | `convertToProject`  |   |   |
| `isReady`  |   |   |   | `convertToTask`  |   |   |
| `storyBoardOrder`  |   |   |   | `linkExternalObject`  |   |   |
|   |   |   |   | `unlinkExternalObject`  |   |   |

{style="table-layout:auto"}

### ResourceBudget

| Fields |References |Collections |Search |Actions |Queries |Operations |
|---|---|---|---|---|---|---|
| `ID`  |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> Flag removed: REPORTABLE

### Schedule

| Fields |References |Collections |Search |Actions |Queries |Operations |
|---|---|---|---|---|---|---|
| `homeGroupID`  | `homeGroup`  |   |   |   |   |   |

{style="table-layout:auto"}

### Task

| Fields |References |Collections |Search |Actions |Queries |Operations |
|---|---|---|---|---|---|---|
|   | `agileWork`  |   |   | `convertToProject`  |   |   |
|   |   |   |   | `linkExternalObject`  |   |   |
|   |   |   |   | `unlinkExternalObject`  |   |   |

{style="table-layout:auto"}

### Team

| Fields |References |Collections |Search |Actions |Queries |Operations |
|---|---|---|---|---|---|---|
| `includeIssues`  |   |   |   |   |   |   |

{style="table-layout:auto"}

### TimesheetProfile

| Fields |References |Collections |Search |Actions |Queries |Operations |
|---|---|---|---|---|---|---|
| `groupID`  | `group`  |   |   |   |   |   |

{style="table-layout:auto"}

### UIFilter

| Fields |References |Collections |Search |Actions |Queries |Operations |
|---|---|---|---|---|---|---|
|   |   |   |   |   | `filtersForObjCode`  |   |

{style="table-layout:auto"}

### UIView

| Fields |References |Collections |Search |Actions |Queries |Operations |
|---|---|---|---|---|---|---|
|   |   |   |   |   | `viewsForObjCode`  |   |

{style="table-layout:auto"}

### User

| Fields |References |Collections |Search |Actions |Queries |Operations |
|---|---|---|---|---|---|---|
| `logTimeInDays`  |   |   |   |   |   |   |
| `workHoursPerDay`  |   |   |   |   |   |   |

{style="table-layout:auto"}

### Work

| Fields |References |Collections |Search |Actions |Queries |Operations |
|---|---|---|---|---|---|---|
| `storyBoardOrder`  |  `agileWork`  |   |   | `getWFHomeObjects`  |   |   |
