---
content-type: api
navigation-topic: api-navigation-topic
title: What's New in API Version 10
description: Updated Resources
author: Becky
feature: Workfront API
role: Developer
exl-id: 8ac384ae-5d65-4c0e-98c1-cf38cfbff460
---
# What's New in API Version 10

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

{style="table-layout:auto"}

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

{style="table-layout:auto"}

### CalendarEntryExternalReference

| Fields |References |Collections |Search |Actions |Queries |Operations |
|---|---|---|---|---|---|---|
| ID |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |COUNT  |
| &nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |GET&nbsp; |
| &nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |REPORT&nbsp; |
| &nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |SEARCH&nbsp; |

{style="table-layout:auto"}

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

{style="table-layout:auto"}

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

{style="table-layout:auto"}

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

{style="table-layout:auto"}

**Updated Resources**

The following existing resources have been updated with this release of the Workfront API. Changes made to a resource are indicated as follows:

* Additions are simply listed
* Removals are indicated with strikethrough text
* Changes are listed in the note after the table

### Approval

| Fields |References |Collections |Search |Actions |Queries |Operations |
|---|---|---|---|---|---|---|
| kanbanFlag |  |  |pendingApproval `<sup>1</sup>` &nbsp; |&nbsp; |&nbsp; |&nbsp; |
| `masterTaskID`  |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |
| priorityColor&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |
| projectBudgetedCost&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |
| projectNetValue&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |
| projectRoi&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |
| resourcePlannerBudgetedLaborCost&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |

{style="table-layout:auto"}

`<sup>1</sup> Type changed from null to boolean`

### Assignment

| Fields |References |Collections |Search |Actions |Queries |Operations |
|---|---|---|---|---|---|---|
| assignmentPercent `<sup>1</sup>` |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |
| viewedByAssignedToUser |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |

{style="table-layout:auto"}

`<sup>1</sup>`added validator LESS_THAN_EQUAL

### BudgetedHour

| Fields |References |Collections |Search |Actions |Queries |Operations |
|---|---|---|---|---|---|---|
| ID  |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |

{style="table-layout:auto"}

&nbsp;

### CustomerPreferences

| Fields |References |Collections |Search |Actions |Queries |Operations |
|---|---|---|---|---|---|---|
| name `<sup>1</sup>` |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |

{style="table-layout:auto"}

<sup>1</sup> Changes to possibleValues

### DocMetadataLinkGroup

| Fields |References |Collections |Search |Actions |Queries |Operations |
|---|---|---|---|---|---|---|
| &nbsp; |&nbsp; |&nbsp; |&nbsp; |getMetadataForDocument |&nbsp; |&nbsp; |

{style="table-layout:auto"}

### Document

| Fields |References |Collections |Search |Actions |Queries |Operations |
|---|---|---|---|---|---|---|
| `masterTaskID`  |  |   |   |   |   |   |

{style="table-layout:auto"}

### DocumentRequest

| Fields |References |Collections |Search |Actions |Queries |Operations |
|---|---|---|---|---|---|---|
| `masterTaskID`  |   |   |   |   |   |   |

{style="table-layout:auto"}

DocumentVersion 

| Fields |References |Collections |Search |Actions |Queries |Operations |
|---|---|---|---|---|---|---|
| externalIntegrationType <sup>1</sup> |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |
| &nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |
| &nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |
| &nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |

{style="table-layout:auto"}

<sup>1</sup> Changes to possibleValues

Expense 

| Fields |References |Collections |Search |Actions |Queries |Operations |
|---|---|---|---|---|---|---|
| `masterTaskID`  |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |

{style="table-layout:auto"}

### Group

| Fields |References |Collections |Search |Actions |Queries |Operations |
|---|---|---|---|---|---|---|
| &nbsp; |licenseTypeLimit |&nbsp; |&nbsp; |addRemoveLicenseTypeLimits&nbsp; |&nbsp; |&nbsp; |
| &nbsp; |&nbsp; |&nbsp; |&nbsp; |setLicenseTypeLimit |&nbsp; |&nbsp; |

{style="table-layout:auto"}

### LinkedFolder

| Fields |References |Collections |Search |Actions |Queries |Operations |
|---|---|---|---|---|---|---|
|  externalIntegrationType<sup>1</sup>  |  |  |  |  |   |   |

{style="table-layout:auto"}

<sup>1</sup> Changes to possibleValues

### OpTask

| Fields |References |Collections |Search |Actions |Queries |Operations |
|---|---|---|---|---|---|---|
| priorityColor |   |  | pendingApproval<sup>1</sup>   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> Type changed from null to boolean

### PortalSection

| Fields |References |Collections |Search |Actions |Queries |Operations |
|---|---|---|---|---|---|---|
|   |  |   |groupIDs  |   |   |   |

{style="table-layout:auto"}

### Portfolio

| Fields |References |Collections |Search |Actions |Queries |Operations |
|---|---|---|---|---|---|---|
| portfolioNetValue  |   |   |   |  |  |   |
| portfolioRoi |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |

{style="table-layout:auto"}

### Project

| Fields |References |Collections |Search |Actions |Queries |Operations |
|---|---|---|---|---|---|---|
| projectBudgetedCost&nbsp; |&nbsp; |&nbsp; |&nbsp; |linkExternalObject&nbsp; |&nbsp; | &nbsp;  |
| projectNetValue |&nbsp; |&nbsp; |&nbsp; |unlinkExternalObject |&nbsp; |&nbsp; |
| projectRoi |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |
| resourcePlannerBudgetedLaborCost |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |

{style="table-layout:auto"}

### ProofApproval

| Fields |References |Collections |Search |Actions |Queries |Operations |
|---|---|---|---|---|---|---|
| approverDecision |   |   |   |   |   |   |

{style="table-layout:auto"}

### Rate

| Fields |References |Collections |Search |Actions |Queries |Operations |
|---|---|---|---|---|---|---|
| rateValue <sup>1</sup> |  |  |  |  |  |   |

{style="table-layout:auto"}

<sup>1</sup>added validator CURRENCY

### Task

| Fields |References |Collections |Search |Actions |Queries |Operations |
|---|---|---|---|---|---|---|
| kanbanFlag |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |
| `masterTaskID`  |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |
| priorityColor&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |

{style="table-layout:auto"}

&nbsp;

### Team

| Fields |References |Collections |Search |Actions |Queries |Operations |
|---|---|---|---|---|---|---|
| hoursPerPoint <sup>1</sup> |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |

{style="table-layout:auto"}

<sup>1</sup> added validator LESS_THAN

### TeamAssignment

| Fields |References |Collections |Search |Actions |Queries |Operations |
|---|---|---|---|---|---|---|
| `masterTaskID`  |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |

{style="table-layout:auto"}

### TeamTask

| Fields |References |Collections |Search |Actions |Queries |Operations |
|---|---|---|---|---|---|---|
| `masterTaskID`  |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |

{style="table-layout:auto"}

### Timesheet

| Fields |References |Collections |Search |Actions |Queries |Operations |
|---|---|---|---|---|---|---|
| &nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |

{style="table-layout:auto"}

### Update

| Fields |References |Collections |Search |Actions |Queries |Operations |
|---|---|---|---|---|---|---|
| updateType `<sup>1</sup>` |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |objectUpdatesWithNoteAndJournalEntryIndex&nbsp; |

{style="table-layout:auto"}

<sup>1</sup> changes to possibleValues

### User

| Fields |References |Collections |Search |Actions |Queries |Operations |
|---|---|---|---|---|---|---|
| &nbsp; |accessLevel&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |

{style="table-layout:auto"}

### UserNote

| Fields |References |Collections |Search |Actions |Queries |Operations |
|---|---|---|---|---|---|---|
| eventType <sup>1</sup> |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |

{style="table-layout:auto"}

<sup>1</sup> changes to possibleValues

### Work

| Fields |References |Collections |Search |Actions |Queries |Operations |
|---|---|---|---|---|---|---|
| kanbanFlag |  |  |pendingApproval <sup>1</sup>&nbsp; |&nbsp; |&nbsp; |&nbsp; |
| `masterTaskID`  |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |
| priorityColor&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |

{style="table-layout:auto"}

<sup>1</sup> Type changed from null to boolean

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

{style="table-layout:auto"}

&nbsp;

&nbsp;

&nbsp;
