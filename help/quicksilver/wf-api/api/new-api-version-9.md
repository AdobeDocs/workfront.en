---
content-type: api
navigation-topic: api-navigation-topic
title: What's New in API Version 9
description: This is a list of resources that are new to API Version 9, to see a list of updates that have been made to the resources of version 9, please visit Updates to API Version 9
author: Becky
feature: Workfront API
role: Developer
exl-id: 29d922f4-f4c6-45e5-b9fa-43e2068ec66d
---
# What's New in API Version 9

## New Resources

This is a list of resources that are new to API&nbsp;Version 9, to see a list of updates that have been made to the resources of version 9, please visit [Updates to API Version 9](../../wf-api/api/new-api-version-9-updates.md)

### AccessLevel

| Fields |References |Collections |Search |Actions |Queries |Operations |
|---|---|---|---|---|---|---|
| `accessRestrictions`  | `customer`  | `accessLevelPermissions`  |  |  |  | `ADD`  |
| `customerID`  | `lastUpdatedBy`  | `accessRulePreferences`  |  |  |  | `COPY`  |
| `description`  |  |  |  |  |  | `COUNT`  |
| `descriptionKey`  |  |  |  |  |  | `DELETE`  |
| `entryDate`  |  |  |  |  |  | `EDIT`  |
| `extRefID`  |  |  |  |  |  | `GET`  |
| `fieldAccessPrivileges`  |  |  |  |  |  | `REPLACE`  |
| `ID`  |  |  |  |  |  | `REPORT`  |
| `isAdmin`  |  |  |  |  |  | `SEARCH`  |
| `isUnsupportedWorkerLicense`  |  |  |  |  |  |&nbsp; |
| `lastUpdatedByID`  |  |  |  |  |  |&nbsp; |
| `lastUpdatedDate`  |  |  |  |  |  |  |
| `licenseType`  |  |  |  |  |  |  |
| `name`  |  |  |  |  |  |  |
| `nameKey`  |  |  |  |  |  |  |
| `securityModelType`  |  |  |  |  |  |  |

{style="table-layout:auto"}

### AccessLevelPermissions

| Fields |References |Collections |Search |Actions |Queries |Operations |
|---|---|---|---|---|---|---|
| `coreAction`  |  |  |  |  |  |&nbsp; |
| `forbiddenActions`  |  |  |  |  |  |&nbsp; |
| `ID`  |  |  |  |  |  |&nbsp; |
| `isAdmin`  |  |  |  |  |  |&nbsp; |
| `objObjCode`  |  |  |  |  |  |  |
| `secondaryActions`  |  |  |  |  |  |  |

{style="table-layout:auto"}

### AccessRulePreference

| Fields |References |Collections |Search |Actions |Queries |Operations |
|---|---|---|---|---|---|---|
| `ID`  |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |

{style="table-layout:auto"}

### BudgetedHour

| Fields |References |Collections |Search |Actions |Queries |Operations |
|---|---|---|---|---|---|---|
| `allocationDate`  |  |  |  |  |  | `ADD`  |
| `budgetedHours`  |  |  |  |  |  | `DELETE`  |
| `GUID`  |  |  |  |  |  | `GET`  |
| `plannedBudgetedHours`  |  |  |  |  |  | `SEARCH`  |
| `projectID`  |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |
| `roleID`&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |
| `userID`&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |

{style="table-layout:auto"}

### CalendarPortalSection

| Fields |References |Collections |Search |Actions |Queries |Operations |
|---|---|---|---|---|---|---|
| `calendarInfoID`  | `customer`  |  | `displayDescription`  |  |  | `ADD`  |
| `customerID`  | `enteredBy`  |  | `displayName`  |  |  | `COPY`  |
| `enteredByID`  |  |  |  |  |  | `COUNT`  |
| `entryDate`  |  |  |  |  |  | `GET`  |
| `ID`  |  |  |  |  |  | `REPORT`  |
| `name`  |  |  |  |  |  | `SEARCH`  |
| `objID`&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |
| `objObjCode`&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |

{style="table-layout:auto"}

### CalendarSection

| Fields |References |Collections |Search |Actions |Queries |Operations |
|---|---|---|---|---|---|---|
| `calendarID`  | `customer`  | `filters`  |  | `getConcatenatedExpressionForm`  |  | `ADD`  |
| `calEvents`  |  |  |  | `getPrettyExpressionForm`  |  | `COUNT`  |
| `color`  |  |  |  |  |  | `DELETE`  |
| `customerID`  |  |  |  |  |  | `EDIT`  |
| `duration`  |  |  |  |  |  | `GET`  |
| `ID`  |  |  |  |  |  | `REPORT`  |
| `milestone`  |  |  |  |  |  | `SEARCH`  |
| `name`&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |
| `plannedDate`  |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |
| `startDate`  |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |

{style="table-layout:auto"}

### ExternalSection

| Fields |References |Collections |Search |Actions |Queries |Operations |
|---|---|---|---|---|---|---|
| `appGlobalID`  | `customer`  |  | `displayDescription`  | `calculateURL`  |  | `ADD`  |
| `calculatedURL`  | `enteredBy`  |  | `displayName`  | `calculateURLS`  |  | `COPY`  |
| `customerID`  | `view`  |  | `linkedCustomersMM`  |  |  | `COUNT`  |
| `description`  |  |  | `linkedUsersMM`  |  |  | `DELETE`  |
| `descriptionKey`  |  |  |  |  |  | `EDIT`  |
| `enteredByID`  |  |  |  |  |  | `GET`  |
| `entryDate`  |  |  |  |  |  | `REPORT`  |
| `extRefID`  |  |  |  |  |  | `SEARCH`  |
| `frame`&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |
| `friendlyURL`&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |
| `globalUIKey`&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |
| `height`&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |
| `ID`&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |
| `name`&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |
| `nameKey`&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |
| `objID`&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |
| `objInterface`&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |
| `objObjCode`&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |
| `scrolling`  |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |
| `url`  |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |
| `viewID`  |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |&nbsp; |

{style="table-layout:auto"}

&nbsp;

This list has been split into two halves. To view the second half, please see [What's New in API Version 9 (continued)](../../wf-api/api/new-api-version-9-continue.md). To view the list of version 9 updates, please visit [Updates to API Version 9](../../wf-api/api/new-api-version-9-updates.md)
