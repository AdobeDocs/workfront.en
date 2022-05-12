---
filename: new-api-version-10
content-type: api
navigation-topic: api-navigation-topic
title: What's New in API Version 10
description: Updated Resources
---

# What's New in API Version 10

>[!IMPORTANT]
>
>You're currently viewing the Adobe Workfront Classic version of this document. Adobe Workfront Classic is no longer supported. All Adobe Workfront Classic functionality, along with this documentation, will be removed in July 2022. Please transition to the the new Adobe Workfront experienceas soon as possible, and switch to the new Adobe Workfront experience version of this document.

* [New Resources](#new-resources) 
* [Updated Resources](#updated-resources) 
* [Removed Resources](#removed-resources)

## New Resources {#new-resources}

### ActivityLog

| Fields |References |Collections |Search |Actions |Queries |Operations |
|---|---|---|---|---|---|---|
| &nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |ADD |
| &nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |COUNT |
| &nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |GET |
| &nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |SEARCH |

### CalendarEntry

| Fields |References |Collections |Search |Actions |Queries |Operations |
|---|---|---|---|---|---|---|
| ID |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |ADD |
| &nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |COUNT&nbsp; |
| &nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |DELETE&nbsp; |
| &nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |EDIT&nbsp; |
| &nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |GET&nbsp; |
| &nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |REPORT&nbsp; |
| &nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |SEARCH |

### CalendarEntryExternalReference

| Fields |References |Collections |Search |Actions |Queries |Operations |
|---|---|---|---|---|---|---|
| ID |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |COUNT  |
| &nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |GET&nbsp; |
| &nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |REPORT&nbsp; |
| &nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |SEARCH&nbsp; |

### ExternalAuthToken

| Fields |References |Collections |Search |Actions |Queries |Operations |
|---|---|---|---|---|---|---|
| ID |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |ADD |
| &nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |COUNT |
| &nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |DELETE&nbsp; |
| &nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |EDIT&nbsp; |
| &nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |GET&nbsp; |
| &nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |REPORT&nbsp; |
| &nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |SEARCH&nbsp; |

### LicenseTypeGroupLimit

| Fields |References |Collections |Search |Actions |Queries |Operations |
|---|---|---|---|---|---|---|
| customerID |customer |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |
| groupID  |group |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |
| planLimit |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |
| usedLicenses |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |
| worklimit |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |
| &nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |
| &nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |

### UserHomeCalendarPreference

| Fields |References |Collections |Search |Actions |Queries |Operations |
|---|---|---|---|---|---|---|
| customerID |customer |&nbsp; |&nbsp; |&nbsp; |&nbsp; |ADD |
| edTime |user |&nbsp; |&nbsp; |&nbsp; |&nbsp; |COUNT |
| firstDayOfWeek |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |DELETE |
| ID |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |EDIT |
| showPTO |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |GET |
| startTime |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |REPORT |
| userID |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |SEARCH |
| workDate |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |

**Updated Resources**

The following existing resources have been updated with this release of the Workfront API. Changes made to a resource are indicated as follows:

* Additions are simply listed
* Removals are indicated with strikethrough text
* Changes are listed in the note after the table

### Approval

| Fields |References |Collections |Search |Actions |Queries |Operations |
|---|---|---|---|---|---|---|
| kanbanFlag |  |  |pendingApproval `¹` &nbsp; |&nbsp; |&nbsp; |&nbsp; |
| `masterTaskID`  |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |
| priorityColor&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |
| projectBudgetedCost&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |
| projectNetValue&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |
| projectRoi&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |
| resourcePlannerBudgetedLaborCost&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |

`¹ Type changed from null to boolean`

### Assignment

| Fields |References |Collections |Search |Actions |Queries |Operations |
|---|---|---|---|---|---|---|
| assignmentPercent `¹` |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |
| viewedByAssignedToUser |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |

`¹`added validator LESS_THAN_EQUAL

### BudgetedHour

| Fields |References |Collections |Search |Actions |Queries |Operations |
|---|---|---|---|---|---|---|
| ID  |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |

&nbsp;

### CustomerPreferences

| Fields |References |Collections |Search |Actions |Queries |Operations |
|---|---|---|---|---|---|---|
| name `¹` |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |

¹ Changes to possibleValues

### DocMetadataLinkGroup

| Fields |References |Collections |Search |Actions |Queries |Operations |
|---|---|---|---|---|---|---|
| &nbsp; |&nbsp; |&nbsp; |&nbsp; |getMetadataForDocument |&nbsp; |&nbsp; |

### Document

| Fields |References |Collections |Search |Actions |Queries |Operations |
|---|---|---|---|---|---|---|
| `masterTaskID`  |  |   |   |   |   |   |

### DocumentRequest

| Fields |References |Collections |Search |Actions |Queries |Operations |
|---|---|---|---|---|---|---|
| `masterTaskID`  |   |   |   |   |   |   |

DocumentVersion 

| Fields |References |Collections |Search |Actions |Queries |Operations |
|---|---|---|---|---|---|---|
| externalIntegrationType ¹ |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |
| &nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |
| &nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |
| &nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |

¹ Changes to possibleValues

Expense 

| Fields |References |Collections |Search |Actions |Queries |Operations |
|---|---|---|---|---|---|---|
| `masterTaskID`  |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |

### Group

| Fields |References |Collections |Search |Actions |Queries |Operations |
|---|---|---|---|---|---|---|
| &nbsp; |licenseTypeLimit |&nbsp; |&nbsp; |addRemoveLicenseTypeLimits&nbsp; |&nbsp; |&nbsp; |
| &nbsp; |&nbsp; |&nbsp; |&nbsp; |setLicenseTypeLimit |&nbsp; |&nbsp; |

### LinkedFolder

| Fields |References |Collections |Search |Actions |Queries |Operations |
|---|---|---|---|---|---|---|
|  externalIntegrationType¹  |  |  |  |  |   |   |

¹ Changes to possibleValues

### OpTask

| Fields |References |Collections |Search |Actions |Queries |Operations |
|---|---|---|---|---|---|---|
| priorityColor |   |  | pendingApproval¹   |   |   |   |

¹ Type changed from null to boolean

### PortalSection

| Fields |References |Collections |Search |Actions |Queries |Operations |
|---|---|---|---|---|---|---|
|   |  |   |groupIDs  |   |   |   |

### Portfolio

| Fields |References |Collections |Search |Actions |Queries |Operations |
|---|---|---|---|---|---|---|
| portfolioNetValue  |   |   |   |  |  |   |
| portfolioRoi |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |

### Project

| Fields |References |Collections |Search |Actions |Queries |Operations |
|---|---|---|---|---|---|---|
| projectBudgetedCost&nbsp; |&nbsp; |&nbsp; |&nbsp; |linkExternalObject&nbsp; |&nbsp; | &nbsp;  |
| projectNetValue |&nbsp; |&nbsp; |&nbsp; |unlinkExternalObject |&nbsp; |&nbsp; |
| projectRoi |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |
| resourcePlannerBudgetedLaborCost |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |

### ProofApproval

| Fields |References |Collections |Search |Actions |Queries |Operations |
|---|---|---|---|---|---|---|
| approverDecision |   |   |   |   |   |   |

### Rate

| Fields |References |Collections |Search |Actions |Queries |Operations |
|---|---|---|---|---|---|---|
| rateValue ¹ |  |  |  |  |  |   |

¹added validator CURRENCY

### Task

| Fields |References |Collections |Search |Actions |Queries |Operations |
|---|---|---|---|---|---|---|
| kanbanFlag |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |
| `masterTaskID`  |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |
| priorityColor&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |

&nbsp;

### Team

| Fields |References |Collections |Search |Actions |Queries |Operations |
|---|---|---|---|---|---|---|
| hoursPerPoint ¹ |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |

¹ added validator LESS_THAN

### TeamAssignment

| Fields |References |Collections |Search |Actions |Queries |Operations |
|---|---|---|---|---|---|---|
| `masterTaskID`  |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |

### TeamTask

| Fields |References |Collections |Search |Actions |Queries |Operations |
|---|---|---|---|---|---|---|
| `masterTaskID`  |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |

### Timesheet

| Fields |References |Collections |Search |Actions |Queries |Operations |
|---|---|---|---|---|---|---|
| &nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |

### Update

| Fields |References |Collections |Search |Actions |Queries |Operations |
|---|---|---|---|---|---|---|
| updateType `¹` |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |objectUpdatesWithNoteAndJournalEntryIndex&nbsp; |

¹ changes to possibleValues

### User

| Fields |References |Collections |Search |Actions |Queries |Operations |
|---|---|---|---|---|---|---|
| &nbsp; |accessLevel&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |

### UserNote

| Fields |References |Collections |Search |Actions |Queries |Operations |
|---|---|---|---|---|---|---|
| eventType ¹ |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |

¹ changes to possibleValues

### Work

| Fields |References |Collections |Search |Actions |Queries |Operations |
|---|---|---|---|---|---|---|
| kanbanFlag |  |  |pendingApproval ¹&nbsp; |&nbsp; |&nbsp; |&nbsp; |
| `masterTaskID`  |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |
| priorityColor&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |

¹ Type changed from null to boolean

## Removed Resources {#removed-resources}

### ResourceBudgetedHour

| Fields |References |Collections |Search |Actions |Queries |Operations |
|---|---|---|---|---|---|---|
| allocationDate |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |ADD&nbsp; |
| budgetedHours |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |COUNT&nbsp; |
| ID |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |DELETE&nbsp; |
| plannedBudgetedHours |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |EDIT&nbsp; |
| projectID |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |GET&nbsp; |
| roleID |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |REPORT&nbsp; |
| userID |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |SEARCH |

&nbsp;

&nbsp;

&nbsp;
