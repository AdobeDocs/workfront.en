---
filename: new-api-version-8
content-type: api
navigation-topic: api-navigation-topic
title: What's New in API Version 8
description: This is a list of resources that are new to API Version 9. For a list of updates that have been made to the resources of version 8 please visit Updates to API Version 8
---

# What's New in API Version 8

>[!IMPORTANT]
>
>You're currently viewing the Adobe Workfront Classic version of this document. Adobe Workfront Classic is no longer supported. All Adobe Workfront Classic functionality, along with this documentation, will be removed in July 2022. Please transition to the the new Adobe Workfront experienceas soon as possible, and switch to the new Adobe Workfront experience version of this document.

## New Resources

This is a list of resources that are new to API&nbsp;Version 9. For a list of updates that have been made to the resources of version 8 please visit [Updates to API Version 8](../../wf-api/api/new-api-version-8-updates.md)

```AgileWork``` 

| Fields |References |Collections |Search |Actions |Queries |Operations |
|---|---|---|---|---|---|---|
| backlogOrder |customer |&nbsp; |&nbsp; |bulkCopy&nbsp; |&nbsp; |COPY |
| color |iteration&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |COUNT |
| customerID |lastUpdatedBy |&nbsp; |&nbsp; |&nbsp; |&nbsp; |DELETE |
| estimate |opTask |&nbsp; |&nbsp; |&nbsp; |&nbsp; |EDIT |
| ID |project |&nbsp; |&nbsp; |&nbsp; |&nbsp; |GET&nbsp; |
| isReady |storyboardParent |&nbsp; |&nbsp; |&nbsp; |&nbsp; |REPORT |
| iterationID |task |&nbsp; |&nbsp; |&nbsp; |&nbsp; |SEARCH |
| lastUpdateDate |team |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |
| lastUpdatedByID |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |
| name |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |
| opTaskID |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |
| parentStoryBoardOrder |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |
| projectID |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |
| storyBoardOrder |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |
| storyBoardParentID |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |
| taskID&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |
| teamID |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |
| type |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |
| uiObjCode |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |
| uiObjectID |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |

### APIVersionMetadata

| Fields |References |Collections |Search |Actions |Queries |Operations |
|---|---|---|---|---|---|---|
| deprecationRelease |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |COUNT&nbsp; |
| removalRelease |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |GET |
| versionName |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |REPORT |
| &nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |SEARCH |

```KanbanBoard``` 

| Fields |References |Collections |Search |Actions |Queries |Operations |
|---|---|---|---|---|---|---|
| ID |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |ADD |
| name |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |COUNT |
| &nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |DELETE |
| &nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |EDIT |
| &nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |GET |
| &nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |REPORT |
| &nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |SEARCH |

### ProofApprovalStatus

| Fields |References |Collections |Search |Actions |Queries |Operations |
|---|---|---|---|---|---|---|
| ID |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |
| proofApprovalStatusID |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |
| proofApprovalStatusLabel |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |

```ProofFileMetadata``` 

| Fields |References |Collections |Search |Actions |Queries |Operations |
|---|---|---|---|---|---|---|
| documentVersionID |documentVersion |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |
| fileIndex |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |
| fileName |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |
| ID |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |
| isURL |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |

```ResourceBudgetedHour``` 

| Fields |References |Collections |Search |Actions |Queries |Operations |
|---|---|---|---|---|---|---|
| allocationDate |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |ADD |
| budgetedHours |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |COUNT |
| plannedBudgetedHours |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |DELETE |
| projectID |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |EDIT |
| roleID |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |GET |
| userID |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |REPORT |
| &nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |SEARCH |

### ResourcePlannerFilter

| Fields |References |Collections |Search |Actions |Queries |Operations |
|---|---|---|---|---|---|---|
| ID |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |ADD |
| name |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |COUNT |
| &nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |DELETE |
| &nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |EDIT |
| &nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |GET |
| &nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |REPORT |
| &nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |SEARCH |

```RichTextNote``` 

| Fields |References |Collections |Search |Actions |Queries |Operations |
|---|---|---|---|---|---|---|
| ID |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |COUNT |
| &nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |GET |
| &nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |REPORT |
| &nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |SEARCH |

### Subscribe

| Fields |References |Collections |Search |Actions |Queries |Operations |
|---|---|---|---|---|---|---|
| &nbsp;ID |&nbsp; |&nbsp; |&nbsp; |addSubscribers |subscribers |ADD |
| &nbsp; |&nbsp; |&nbsp; |&nbsp; |removeSubscribers |&nbsp; |COUNT&nbsp; |
| &nbsp; |&nbsp; |&nbsp; |&nbsp; |subscribes |&nbsp; |DELETE |
| &nbsp; |&nbsp; |&nbsp; |&nbsp; |unsubscribes |&nbsp; |GET |
| &nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |REPORT |
| &nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |SEARCH |

### UserRole

| Fields |References |Collections |Search |Actions |Queries |Operations |
|---|---|---|---|---|---|---|
| roleID |role |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |
| timePercentage |user |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |
| userID |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |

