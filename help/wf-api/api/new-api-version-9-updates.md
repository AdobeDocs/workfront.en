---
filename: new-api-version-9-updates
content-type: api
navigation-topic: api-navigation-topic
title: Updates to API Version 9
description: Updated Resources
---

# Updates to API Version 9

`Updated Resources`

The following existing resources have been updated with this release of the *Adobe Workfront* API. To view the resources that are new to version 9 you can visit [What's New in API Version 9](../../wf-api/api/new-api-version-9.md) and [What's New in API Version 9 (continued)](../../wf-api/api/new-api-version-9-continue.md). Changes made to a resource are indicated in the following manner:

* Additions are simply listed
* Removals are indicated with strikethrough text
* Changes are noted in the note after the table

### AgileWork`<sup>1</sup>`

| Fields |References |Collections |Search |Actions |Queries |Operations |
|---|---|---|---|---|---|---|
| `opTaskID` ``<sup>2</sup>`` ``  | ``  | ``  | ``  | ``  | ``  | ``  |
| `taskID`<sup>2</sup>``  | ``  | ``  | ``  | ``  | ``  | ``  |

`¹ Flag removed: REPORTABLE`   
`² Flag removed: NOT_GROUPABLE`

### Approval

| Fields |References |Collections |Search |Actions |Queries |Operations |
|---|---|---|---|---|---|---|
| `storyBoardOrder`  | ``<strike> agileWork</strike>``  |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |

Assignment

| Fields |References |Collections |Search |Actions |Queries |Operations |
|---|---|---|---|---|---|---|
| ``  | ``  | ``  | ``  | `assignUserToRoleOnProjects`<sup>1</sup>``  | ``  | ``  |
| ``  | ``  | ``  | ``  | `assignUserToRoleOnTasks`<sup>1</sup>``  | ``  | ``  |
| ``  | ``  | ``  | ``  | `swapUsersOnProjects`<sup>1</sup>``  | ``  | ``  |
| ``  | ``  | ``  | ``  | `swapUsersOnTasks`<sup>1</sup>``  | ``  | ``  |

`¹ Added field: lockToRole`

### `<font size="4">CustomerPreferences</font>`

| Fields |References |Collections |Search |Actions |Queries |Operations |
|---|---|---|---|---|---|---|
| `name`<sup>1</sup>``  |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |

`¹ Changes to possibleValues`

### Hour

| Fields |References |Collections |Search |Actions |Queries |Operations |
|---|---|---|---|---|---|---|
| `days`  | ``  | ``  | ``  | ``  | ``  | ``  |
| `workHoursPerDay`  | ``  | ``  | ``  | ``  | ``  | ``  |

### `<font size="4">Iteration</font>`

| Fields |References |Collections |Search |Actions |Queries |Operations |
|---|---|---|---|---|---|---|
| ``  | ``  | ``  | ``  | `moveIssues`  | ``  | ``  |

### `<font size="4">LayoutTemplates</font>`

| Fields |References |Collections |Search |Actions |Queries |Operations |
|---|---|---|---|---|---|---|
| `groupID`  | `group`  | ``  | ``  | ``  | ``  | ``  |

### `<font size="4">Note</font>`

| Fields |References |Collections |Search |Actions |Queries |Operations |
|---|---|---|---|---|---|---|
| `html`  | ``  | ``  | ``  | ``  | ``  | ``  |
| `json`  | ``  | ``  | ``  | ``  | ``  | ``  |
| `richTextNoteID`  | ``  | ``  | ``  | ``  | ``  | ``  |

### `<font size="4">OpTask</font>`

| Fields |References |Collections |Search |Actions |Queries |Operations |
|---|---|---|---|---|---|---|
| `color`  | ``<strike> agileWork</strike>``  | ``  | ``  | `convertToProject`  | ``  | ``  |
| `isReady`  | ``  | ``  | ``  | `convertToTask`  | ``  | ``  |
| `storyBoardOrder`  | ``  | ``  | ``  | `linkExternalObject`  | ``  | ``  |
| ``  | ``  | ``  | ``  | `unlinkExternalObject`  | ``  | ``  |

### ResourceBudget`<sup>1</sup>`

| Fields |References |Collections |Search |Actions |Queries |Operations |
|---|---|---|---|---|---|---|
| `ID`  | ``  | ``  | ``  | ``  | ``  | ``  |

`¹ Flag removed: REPORTABLE`

### `<font size="4">Schedule</font>`

| Fields |References |Collections |Search |Actions |Queries |Operations |
|---|---|---|---|---|---|---|
| `homeGroupID`  | `homeGroup`  | ``  | ``  | ``  | ``  | ``  |

### `<font size="4">Task</font>`

| Fields |References |Collections |Search |Actions |Queries |Operations |
|---|---|---|---|---|---|---|
| ``  | ``<strike> agileWork</strike>``  | ``  | ``  | `convertToProject`  | ``  | ``  |
| ``  | ``  | ``  | ``  | `linkExternalObject`  | ``  | ``  |
| ``  | ``  | ``  | ``  | `unlinkExternalObject`  | ``  | ``  |

### `<font size="4">Team</font>`

| Fields |References |Collections |Search |Actions |Queries |Operations |
|---|---|---|---|---|---|---|
| ``<strike> includeIssues</strike>``  | ``  | ``  | ``  | ``  | ``  | ``  |

### `<font size="4">TimesheetProfile</font>`

| Fields |References |Collections |Search |Actions |Queries |Operations |
|---|---|---|---|---|---|---|
| `groupID`  | `group`  | ``  | ``  | ``  | ``  | ``  |

### `<font size="4">UIFilter</font>`

| Fields |References |Collections |Search |Actions |Queries |Operations |
|---|---|---|---|---|---|---|
| ``  | ``  | ``  | ``  | ``  | `filtersForObjCode`  | ``  |

### `<font size="4">UIView</font>`

| Fields |References |Collections |Search |Actions |Queries |Operations |
|---|---|---|---|---|---|---|
| ``  | ``  | ``  | ``  | ``  | `viewsForObjCode`  | ``  |

### `<font size="4">User</font>`

| Fields |References |Collections |Search |Actions |Queries |Operations |
|---|---|---|---|---|---|---|
| `logTimeInDays`  | ``  | ``  | ``  | ``  | ``  | ``  |
| `workHoursPerDay`  | ``  | ``  | ``  | ``  | ``  | ``  |

### `<font size="4">Work</font>`

| Fields |References |Collections |Search |Actions |Queries |Operations |
|---|---|---|---|---|---|---|
| `storyBoardOrder`  | ``<strike> agileWork</strike>``  | ``  | ``  | `getWFHomeObjects`  | ``  | ``  |

