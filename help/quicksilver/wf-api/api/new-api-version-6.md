---
content-type: api
navigation-topic: api-navigation-topic
title: What's New in API Version 6
description: What's New in API Version 6
author: Becky
feature: Workfront API
role: Developer
exl-id: e671a881-b8c2-4234-a3a0-76b1fbfafd32
---
# What's New in API Version 6

## New Objects

### Resource Manager

| Fields |References |Collections |Search |Actions |Queries |Operations |
|---|---|---|---|---|---|---|
| ID |customer |&nbsp; |&nbsp; |&nbsp; |&nbsp; |Add |
| customerID |project |&nbsp; |&nbsp; |&nbsp; |&nbsp; |Count |
| projectID |resourceManager |&nbsp; |&nbsp; |&nbsp; |&nbsp; |Delete |
| resourceManagerID |template |&nbsp; |&nbsp; |&nbsp; |&nbsp; |Get |
| templateID |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |Report&nbsp; |
| &nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |Search&nbsp; |


### Ews

| Fields |References |Collections |Search |Actions |Queries |Operations |
|---|---|---|---|---|---|---|
| fileName |&nbsp; |&nbsp; |&nbsp; |&nbsp; |upload |&nbsp; |
| handle |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |
| objCode |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |


### Custom Label

| Fields |References |Collections |Search |Actions |Queries |Operations |
|---|---|---|---|---|---|---|
| ID |&nbsp; |&nbsp; |&nbsp; |checkDelete |customLabels |Add |
| &nbsp; |&nbsp; |&nbsp; |&nbsp; |inUseByOtherLayoutTemplate |userCustomLabels |Count |
| &nbsp; |&nbsp; |&nbsp; |&nbsp; |removeCustomLabel |&nbsp; |Delete |
| &nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |Get |
| &nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |Report |
| &nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |Search |


## Updated Objects

Changes to existing objects: additions are simply listed, removals have strikethrough, changes to existing have an attached note after the table

### Update

&nbsp;

| Fields |References |Collections |Search |Actions |Queries |Operations |
|---|---|---|---|---|---|---|
| updateType<sup>1</sup> |&nbsp; |&nbsp; |&nbsp; |&nbsp; |`sinceDate`  |&nbsp; |
| &nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |objectUpdatesByCommentID<sup>2</sup> |&nbsp; |

{style="table-layout:auto"}

<sup>1</sup> Changes to possible values

<sup>2</sup> hasFilters attribute changed to true

&nbsp;

### Approval

| Fields |References |Collections |Search |Actions |Queries |Operations |
|---|---|---|---|---|---|---|
| completedHours |&nbsp; |resourceManagers |resourceManagerIDs |&nbsp; |&nbsp; |&nbsp; |
| constraintDate<sup>1</sup> |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |
| isOriginalPlannedHoursSet |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |
| syncBurndownDate |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |
| workRequired<sup>2</sup> |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |

{style="table-layout:auto"}

<sup>1</sup> Date validation added

<sup>2</sup> NOT_FILTERABLE flag added

&nbsp;

### Approval Process

| &nbsp; |Fields |References |Collections |Search |Actions |Queries |Operations |
|---|---|---|---|---|---|---|---|
|   |  | `attachedApprovalPaths`  |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |

{style="table-layout:auto"}

&nbsp;

### Approval Step

&nbsp;

| Fields |References |Collections |Search |Actions |Queries |Operations |
|---|---|---|---|---|---|---|
| approvalType<sup>1</sup> |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |

{style="table-layout:auto"}

<sup>1</sup> Changes to possible Values

&nbsp;

### Approval Path<sup>1</sup>

| Fields |References |Collections |Search |Actions |Queries |Operations |
|---|---|---|---|---|---|---|
| approvedStatus |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |Add |
| approvedStatusLabel |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |Count |
| comment |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |Delete |
| enteredByID |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |Edit |
| entryDate |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |Get |
| globalPathID |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |Report |
| isPrivate |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |Search |
| lastUpdateDate |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |
| lastUpdateByID |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |
| name<sup>2</sup> |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |

{style="table-layout:auto"}

<sup>1</sup> Changed to Reportable

<sup>2</sup> Added Max Length Validator

&nbsp;

### Work Service Object

| Fields |References |Collections |Search |Actions |Queries |Operations |
|---|---|---|---|---|---|---|
| constraintDate<sup>1</sup> |&nbsp; |&nbsp; |&nbsp; |getMyWorkCountFiltered |&nbsp; |&nbsp; |
| workRequired<sup>2</sup> |&nbsp; |&nbsp; |&nbsp; |workItemStatusLabels&nbsp; |&nbsp; |&nbsp; |

{style="table-layout:auto"}

<sup>1</sup> Date Validation Added

<sup>2</sup> Not_Filterable Flag Added

&nbsp;

### Assignment

| Fields |References |Collections |Search |Actions |Queries |Operations |
|---|---|---|---|---|---|---|
| &nbsp; |&nbsp; |&nbsp; |&nbsp; |assignUserToRoleOnProjects |&nbsp; |&nbsp; |
| &nbsp; |&nbsp; |&nbsp; |&nbsp; |swapUsersOnProjects |&nbsp; |&nbsp; |
| &nbsp; |&nbsp; |&nbsp; |&nbsp; |unassignUserFromProjects |&nbsp; |&nbsp; |

{style="table-layout:auto"}

&nbsp;

### Baseline&nbsp;

| Fields |References |Collections |Search |Actions |Queries |Operations |
|---|---|---|---|---|---|---|
| workRequired<sup>1</sup> |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |

{style="table-layout:auto"}

<sup>1</sup> Not_Filterable Flag Added

&nbsp;

### Baseline Task

| Fields |References |Collections |Search |Actions |Queries |Operations |
|---|---|---|---|---|---|---|
| workRequired<sup>1</sup> |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |

{style="table-layout:auto"}

<sup>1</sup> Not_Filterable Flag Added

&nbsp;

### Billing Record

| Fields |References |Collections |Search |Actions |Queries |Operations |
|---|---|---|---|---|---|---|
| billingDate<sup>1</sup> |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |

{style="table-layout:auto"}

<sup>1</sup> added NO_TIME field flag

### Burndown Event&nbsp;

| Fields |References |Collections |Search |Actions |Queries |Operations |
|---|---|---|---|---|---|---|
| eventInitiator |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |`ADD`  |
| &nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |`DELETE`  |

{style="table-layout:auto"}

&nbsp;

### Category&nbsp;

| Fields |References |Collections |Search |Actions |Queries |Operations |
|---|---|---|---|---|---|---|
| &nbsp; |&nbsp; |&nbsp; |&nbsp; |getCascadingRules |&nbsp; |&nbsp; |
| &nbsp; |&nbsp; |&nbsp; |&nbsp; |reorderCategories |&nbsp; |&nbsp; |

{style="table-layout:auto"}

&nbsp;

Custom Enum&nbsp;

| Fields |References |Collections |Search |Actions |Queries |Operations |
|---|---|---|---|---|---|---|
| &nbsp; |&nbsp; |&nbsp; |&nbsp; |getGroupDefaultProjectStatus |opTaskGroupStatuses |&nbsp; |
| &nbsp; |&nbsp; |&nbsp; |&nbsp; |isPossibleToUnlockStatus |projectGroupStatuses |&nbsp; |
| &nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |taskGroupStatuses |&nbsp; |

{style="table-layout:auto"}

&nbsp;

Document&nbsp;

| Fields |References |Collections |Search |Actions |Queries |Operations |
|---|---|---|---|---|---|---|
| `checkedOutByID`  |`checkedOutBy`&nbsp; |&nbsp; |&nbsp;isDir |&nbsp; |&nbsp; |&nbsp; |
| `isDir`&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |

{style="table-layout:auto"}

&nbsp;

Exchange Rate&nbsp;

| Fields |References |Collections |Search |Actions |Queries |Operations |
|---|---|---|---|---|---|---|
| rate<sup>1</sup> |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |

{style="table-layout:auto"}

<sup>1</sup> Changed PRECISION validator for 8 to 9

&nbsp;

### Integration

| Fields |References |Collections |Search |Actions |Queries |Operations |
|---|---|---|---|---|---|---|
| syncBurndownDate |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |

{style="table-layout:auto"}

&nbsp;

### Journal Entry

| Fields |References |Collections |Search |Actions |Queries |Operations |
|---|---|---|---|---|---|---|
| changeType<sup>1</sup> |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |

{style="table-layout:auto"}

<sup>1</sup> Changes to possible Values

&nbsp;

### Optask (Issue)<sup>1</sup>&nbsp;

| Fields |References |Collections |Search |Actions |Queries |Operations |
|---|---|---|---|---|---|---|
| workRequired<sup>2</sup> |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |

{style="table-layout:auto"}

<sup>1</sup> Flagged as RESTORABLE

<sup>2</sup> Not_Filterable Flag Added

&nbsp;

### Project<sup>1</sup>&nbsp;

| Fields |References |Collections |Search |Actions |Queries |Operations |
|---|---|---|---|---|---|---|
| completedHours |&nbsp; |`openOpTasks`  |&nbsp;openOpTasks |&nbsp; |&nbsp; |&nbsp; |
| isOriginalPlannedHoursSet |&nbsp; |resourceManagers |resourceManagerIDs&nbsp; |&nbsp; |&nbsp; |&nbsp; |
| originalWorkRequired |&nbsp; |&nbsp; |`work`  |&nbsp; |&nbsp; |&nbsp; |
| syncBurndownDate |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |
| work |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |
| workRequired |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |

{style="table-layout:auto"}

<sup>1</sup> Flagged as RESTORABLE and RESOURCE_MANAGEABLE

<sup>2</sup> Not_Filterable Flag Added

&nbsp;

### Task<sup>1</sup>

| Fields |References |Collections |Search |Actions |Queries |Operations |
|---|---|---|---|---|---|---|
| constraintDate<sup>2</sup> |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |
| workRequired<sup>3</sup> |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |

{style="table-layout:auto"}

<sup>1</sup> Flagged as RESTORABLE

<sup>2</sup> AT_DATE_YEAR_BEFORE validator added

<sup>3</sup> Not_Filterable Flag Added

&nbsp;

### Team

| Fields |References |Collections |Search |Actions |Queries |Operations |
|---|---|---|---|---|---|---|
| `myWorkViewID`  |&nbsp;`myWorkView` |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |
| `requestsViewID`&nbsp; |`myRequestsView`&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |

{style="table-layout:auto"}

&nbsp;

### Template<sup>1</sup>&nbsp;

| Fields |References |Collections |Search |Actions |Queries |Operations |
|---|---|---|---|---|---|---|
| &nbsp; |&nbsp; |resourceManagers |resourceManagerIDs |&nbsp; |&nbsp; |&nbsp; |

{style="table-layout:auto"}

<sup>1</sup> Flagged as RESTORABLE and RESOURCE_MANAGEABLE

### Template Task<sup>1</sup>&nbsp;

| Fields |References |Collections |Search |Actions |Queries |Operations |
|---|---|---|---|---|---|---|
| workRequired<sup>2</sup> |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |

{style="table-layout:auto"}

<sup>1</sup> Flagged as RESTORABLE

<sup>2</sup> Not_Filterable Flag Added

&nbsp;

### User

| Fields |References |Collections |Search |Actions |Queries |Operations |
|---|---|---|---|---|---|---|
| myInfo<sup>1</sup> |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |

{style="table-layout:auto"}

<sup>1</sup> MAX_LENGTH violators

&nbsp;

### User Note

| Fields |References |Collections |Search |Actions |Queries |Operations |
|---|---|---|---|---|---|---|
| eventType<sup>1</sup> |&nbsp; |&nbsp; |&nbsp; |&nbsp; |myNotifications<sup>2</sup> |&nbsp; |

{style="table-layout:auto"}

<sup>1</sup> Possible Values Changed

<sup>2</sup> has filters Changed to `[true]`

&nbsp;

### Announcement

| Fields |References |Collections |Search |Actions |Queries |Operations |
|---|---|---|---|---|---|---|
| &nbsp; |&nbsp; |&nbsp; |&nbsp; |`fileHandle`  |&nbsp; |&nbsp; |
| &nbsp; |&nbsp; |&nbsp; |&nbsp; |`zipAnnouncementAttachments`&nbsp; |&nbsp; |&nbsp; |
