---
content-type: api
navigation-topic: api-navigation-topic
title: What's New in API Version 6
description: What's New in API Version 6
feature: Workfront API
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

{style="table-layout:auto"}

### Ews

| Fields |References |Collections |Search |Actions |Queries |Operations |
|---|---|---|---|---|---|---|
| fileName |&nbsp; |&nbsp; |&nbsp; |&nbsp; |upload |&nbsp; |
| handle |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |
| objCode |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |

{style="table-layout:auto"}

### Custom Label

| Fields |References |Collections |Search |Actions |Queries |Operations |
|---|---|---|---|---|---|---|
| ID |&nbsp; |&nbsp; |&nbsp; |checkDelete |customLabels |Add |
| &nbsp; |&nbsp; |&nbsp; |&nbsp; |inUseByOtherLayoutTemplate |userCustomLabels |Count |
| &nbsp; |&nbsp; |&nbsp; |&nbsp; |removeCustomLabel |&nbsp; |Delete |
| &nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |Get |
| &nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |Report |
| &nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |Search |

{style="table-layout:auto"}

&nbsp;

## Updated Objects

Changes to existing objects: additions are simply listed, removals have strikethrough, changes to existing have an attached&nbsp;note after the table

### Update

&nbsp;

| Fields |References |Collections |Search |Actions |Queries |Operations |
|---|---|---|---|---|---|---|
| updateType¹ |&nbsp; |&nbsp; |&nbsp; |&nbsp; |`sinceDate`  |&nbsp; |
| &nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |objectUpdatesByCommentID² |&nbsp; |

{style="table-layout:auto"}

¹ Changes to possible values

² hasFilters attribute changed to true

&nbsp;

### Approval

| Fields |References |Collections |Search |Actions |Queries |Operations |
|---|---|---|---|---|---|---|
| completedHours |&nbsp; |resourceManagers |resourceManagerIDs |&nbsp; |&nbsp; |&nbsp; |
| constraintDate¹ |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |
| isOriginalPlannedHoursSet |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |
| syncBurndownDate |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |
| workRequired² |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |

{style="table-layout:auto"}

¹ Date validation added

² NOT_FILTERABLE flag added

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
| approvalType¹ |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |

{style="table-layout:auto"}

¹ Changes to possible Values

&nbsp;

### Approval Path¹

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
| name² |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |

{style="table-layout:auto"}

¹ Changed to Reportable

² Added Max Length Validator

&nbsp;

### Work Service Object

| Fields |References |Collections |Search |Actions |Queries |Operations |
|---|---|---|---|---|---|---|
| constraintDate¹ |&nbsp; |&nbsp; |&nbsp; |getMyWorkCountFiltered |&nbsp; |&nbsp; |
| workRequired² |&nbsp; |&nbsp; |&nbsp; |workItemStatusLabels&nbsp; |&nbsp; |&nbsp; |

{style="table-layout:auto"}

¹ Date Validation Added

² Not_Filterable Flag Added

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
| workRequired¹ |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |

{style="table-layout:auto"}

¹ Not_Filterable Flag Added

&nbsp;

### Baseline Task

| Fields |References |Collections |Search |Actions |Queries |Operations |
|---|---|---|---|---|---|---|
| workRequired¹ |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |

{style="table-layout:auto"}

¹ Not_Filterable Flag Added

&nbsp;

### Billing Record

| Fields |References |Collections |Search |Actions |Queries |Operations |
|---|---|---|---|---|---|---|
| billingDate¹ |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |

{style="table-layout:auto"}

¹ added NO_TIME field flag

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
| rate¹ |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |

{style="table-layout:auto"}

¹ Changed PRECISION validator for 8 to 9

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
| changeType¹ |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |

{style="table-layout:auto"}

¹ Changes to possible Values

&nbsp;

### Optask (Issue)¹&nbsp;

| Fields |References |Collections |Search |Actions |Queries |Operations |
|---|---|---|---|---|---|---|
| workRequired² |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |

{style="table-layout:auto"}

¹ Flagged as RESTORABLE

² Not_Filterable Flag Added

&nbsp;

### Project¹&nbsp;

| Fields |References |Collections |Search |Actions |Queries |Operations |
|---|---|---|---|---|---|---|
| completedHours |&nbsp; |`openOpTasks`  |&nbsp;openOpTasks |&nbsp; |&nbsp; |&nbsp; |
| isOriginalPlannedHoursSet |&nbsp; |resourceManagers |resourceManagerIDs&nbsp; |&nbsp; |&nbsp; |&nbsp; |
| originalWorkRequired |&nbsp; |&nbsp; |`work`  |&nbsp; |&nbsp; |&nbsp; |
| syncBurndownDate |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |
| work |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |
| workRequired |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |

{style="table-layout:auto"}

¹ Flagged as RESTORABLE and RESOURCE_MANAGEABLE

² Not_Filterable Flag Added

&nbsp;

### Task¹

| Fields |References |Collections |Search |Actions |Queries |Operations |
|---|---|---|---|---|---|---|
| constraintDate² |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |
| workRequired³ |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |

{style="table-layout:auto"}

¹ Flagged as RESTORABLE

² AT_DATE_YEAR_BEFORE validator added

³ Not_Filterable Flag Added

&nbsp;

### Team

| Fields |References |Collections |Search |Actions |Queries |Operations |
|---|---|---|---|---|---|---|
| `myWorkViewID`  |&nbsp;`myWorkView` |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |
| `requestsViewID`&nbsp; |`myRequestsView`&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |

{style="table-layout:auto"}

&nbsp;

### Template¹&nbsp;

| Fields |References |Collections |Search |Actions |Queries |Operations |
|---|---|---|---|---|---|---|
| &nbsp; |&nbsp; |resourceManagers |resourceManagerIDs |&nbsp; |&nbsp; |&nbsp; |

{style="table-layout:auto"}

¹ Flagged as RESTORABLE and RESOURCE_MANAGEABLE

### Template Task¹&nbsp;

| Fields |References |Collections |Search |Actions |Queries |Operations |
|---|---|---|---|---|---|---|
| workRequired² |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |

{style="table-layout:auto"}

¹ Flagged as RESTORABLE

² Not_Filterable Flag Added

&nbsp;

### User

| Fields |References |Collections |Search |Actions |Queries |Operations |
|---|---|---|---|---|---|---|
| myInfo¹ |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |

{style="table-layout:auto"}

¹ MAX_LENGTH violators

&nbsp;

### User Note

| Fields |References |Collections |Search |Actions |Queries |Operations |
|---|---|---|---|---|---|---|
| eventType¹ |&nbsp; |&nbsp; |&nbsp; |&nbsp; |myNotifications² |&nbsp; |

{style="table-layout:auto"}

¹ Possible Values Changed

² has filters Changed to `[true]`

&nbsp;

### Announcement

| Fields |References |Collections |Search |Actions |Queries |Operations |
|---|---|---|---|---|---|---|
| &nbsp; |&nbsp; |&nbsp; |&nbsp; |`fileHandle`  |&nbsp; |&nbsp; |
| &nbsp; |&nbsp; |&nbsp; |&nbsp; |`zipAnnouncementAttachments`&nbsp; |&nbsp; |&nbsp; |

