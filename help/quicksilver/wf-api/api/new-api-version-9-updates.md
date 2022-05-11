---
filename: new-api-version-9-updates
content-type: api
navigation-topic: api-navigation-topic
title: Updates to API Version 9
description: Updated Resources
---

# Updates to API Version 9

## Updated Resources

The following existing resources have been updated with this release of the Adobe Workfront API. To view the resources that are new to version 9 you can visit [What's New in API Version 9](../../wf-api/api/new-api-version-9.md) and [What's New in API Version 9 (continued)](../../wf-api/api/new-api-version-9-continue.md). Changes made to a resource are indicated in the following manner:

* Additions are simply listed
* Removals are indicated with strikethrough text
* Changes are noted in the note after the table

### AgileWork

<!--WRITER check tables-->

| Fields |References |Collections |Search |Actions |Queries |Operations |
|---|---|---|---|---|---|---|
| `opTaskID`<sup>2</sup> |  |   |  |   |   |  |
| `taskID`<sup>2</sup>  |   |   |  |  |  |  |

¹ Flag removed: REPORTABLE   
² Flag removed: NOT_GROUPABLE

### Approval

| Fields |References |Collections |Search |Actions |Queries |Operations |
|---|---|---|---|---|---|---|
| `storyBoardOrder`  | `agileWork`  |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |

Assignment

| Fields |References |Collections |Search |Actions |Queries |Operations |
|---|---|---|---|---|---|---|
| |   |  |  | `assignUserToRoleOnProjects`<sup>1</sup> |   |   |
|   |   |   |   | `assignUserToRoleOnTasks`<sup>1</sup>  |   |   |
|   |   |   |   | `swapUsersOnProjects`<sup>1</sup>  |   |   |
|   |   |   |   | `swapUsersOnTasks`<sup>1</sup>  |   |   |

¹ Added field: lockToRole

### CustomerPreferences

| Fields |References |Collections |Search |Actions |Queries |Operations |
|---|---|---|---|---|---|---|
| `name`<sup>1</sup>  |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |

¹ Changes to possibleValues

### Hour

| Fields |References |Collections |Search |Actions |Queries |Operations |
|---|---|---|---|---|---|---|
| `days`  |   |   |   |   |   |   |
| `workHoursPerDay`  |   |   |   |   |   |   |

### Iteration

| Fields |References |Collections |Search |Actions |Queries |Operations |
|---|---|---|---|---|---|---|
|   |   |   |   | `moveIssues`  |   |   |

### LayoutTemplates

| Fields |References |Collections |Search |Actions |Queries |Operations |
|---|---|---|---|---|---|---|
| `groupID`  | `group`  |   |   |   |   |   |

### Note

| Fields |References |Collections |Search |Actions |Queries |Operations |
|---|---|---|---|---|---|---|
| `html`  |   |   |   |   |   |   |
| `json`  |   |   |   |   |   |   |
| `richTextNoteID`  |   |   |   |   |   |   |

### OpTask

| Fields |References |Collections |Search |Actions |Queries |Operations |
|---|---|---|---|---|---|---|
| `color`  | agileWork  |   |   | `convertToProject`  |   |   |
| `isReady`  |   |   |   | `convertToTask`  |   |   |
| `storyBoardOrder`  |   |   |   | `linkExternalObject`  |   |   |
|   |   |   |   | `unlinkExternalObject`  |   |   |

### ResourceBudget

| Fields |References |Collections |Search |Actions |Queries |Operations |
|---|---|---|---|---|---|---|
| `ID`  |   |   |   |   |   |   |

¹ Flag removed: REPORTABLE

### Schedule

| Fields |References |Collections |Search |Actions |Queries |Operations |
|---|---|---|---|---|---|---|
| `homeGroupID`  | `homeGroup`  |   |   |   |   |   |

### Task

| Fields |References |Collections |Search |Actions |Queries |Operations |
|---|---|---|---|---|---|---|
|   | agileWork  |   |   | `convertToProject`  |   |   |
|   |   |   |   | `linkExternalObject`  |   |   |
|   |   |   |   | `unlinkExternalObject`  |   |   |

### Team

| Fields |References |Collections |Search |Actions |Queries |Operations |
|---|---|---|---|---|---|---|
| includeIssues  |   |   |   |   |   |   |

### TimesheetProfile

| Fields |References |Collections |Search |Actions |Queries |Operations |
|---|---|---|---|---|---|---|
| `groupID`  | `group`  |   |   |   |   |   |

### UIFilter

| Fields |References |Collections |Search |Actions |Queries |Operations |
|---|---|---|---|---|---|---|
|   |   |   |   |   | `filtersForObjCode`  |   |

### UIView

| Fields |References |Collections |Search |Actions |Queries |Operations |
|---|---|---|---|---|---|---|
|   |   |   |   |   | `viewsForObjCode`  |   |

### User

| Fields |References |Collections |Search |Actions |Queries |Operations |
|---|---|---|---|---|---|---|
| `logTimeInDays`  |   |   |   |   |   |   |
| `workHoursPerDay`  |   |   |   |   |   |   |

### Work

| Fields |References |Collections |Search |Actions |Queries |Operations |
|---|---|---|---|---|---|---|
| `storyBoardOrder`  |  agileWork  |   |   | `getWFHomeObjects`  |   |   |

