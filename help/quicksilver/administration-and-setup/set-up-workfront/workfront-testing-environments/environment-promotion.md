---
user-type: administrator
content-type: overview;how-to-procedural
product-area: system-administration
navigation-topic: workfront-testing-environments
title: Environment promotion
description: Environment promotion
author: Becky
feature: System Setup and Administration
role: Admin
---
# Environment promotion

## Access requirements

You must have the following:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Workfront] plan</td> 
   <td> <p>Enterprise, Prime, or Ultimate</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p role="rowheader">[!DNL Workfront] license</p> </td> 
   <td> <p>[!UICONTROL Plan] </p> <p>You must be a [!DNL Workfront] administrator. For information on [!DNL Workfront] administrators, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Grant a user full administrative access</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p role="rowheader">Object permissions</p> </td> 
   <td> <p>All</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Support package</td> 
   <td> <p>[!UICONTROL Plus], [!UICONTROL Preferred], or [!UICONTROL Enterprise]</p> <p>The standard support package does not have access to the Custom Refresh Sandbox, but it does have access to the Preview Sandbox.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Prerequisites

The Create Promotion Package endpoint assumes that you have already configured the source environment. This API call requires manually creating an object map of [!DNL Workfront] objCodes and object GUIDs. The specific structure of this map is described below.

## Supported objects for environment promotion

The Environment Promotion capability is intended to provide the ability to move configuration-related objects from one environment to another. It does not support the ability to move transactional objects (with limited exceptions).

### Work objects

| Promotable object | Included sub-objects |
| --- | --- |
| Project (PROJ) | Project<br>Task<br>Assignment<br>Predecessor<br>Company<br>Override Rate<br>Group<br>Role<br>Team<br>Approval Process<br>Approval Path<br>Approval Step<br>Step Approver<br>Schedule<br>Non Work Day<br>Queue Definition<br>Queue Topic Group<br>Queue Topic<br>Routing Rule<br>Milestone Path<br>Milestone<br>Hour Type<br>Resource Pool<br>Category<br>Category Parameter<br>Parameter<br>Parameter Group<br>Parameter Option<br>Category Display Logic | 
| Template (TMPL) | Template<br>Template Task<br>Template Task Assignment<br>Template Task Predecessor<br>Company<br>Override Rate<br>Group<br>Role<br>Team<br>Approval Process<br>Approval Path<br>Approval Step<br>Step Approver<br>Schedule<br>Non Work Day<br>Queue Definition<br>Queue Topic Group<br>Queue Topic<br>Routing Rule<br>Milestone Path<br>Milestone<br>Hour Type<br>Resource Pool<br>Category<br>Category Parameter<br>Parameter<br>Parameter Group<br>Parameter Option<br>Category Display Logic | 

### Reporting objects

| Promotable object | Included sub-objects |
| --- | --- |
| Layout Template (UITMPL) | Layout Template<br>Dashboard<br>Calendar<br>Calendar Section<br>External Page<br>Report<br>Filter<br>Grouping<br>View<br>Parameter  | 
| Dashboard (PTLTAB) | Dashboard<br>Calendar<br>Calendar Section<br>External Page<br>Report<br>Filter<br>Grouping<br>View<br>Parameter  | 
| Calendar (CALEND) | Calendar<br>Calendar Section | 
| External Page (EXTSEC) | External Page |
| Report (PTLSEC) | Report<br>Filter<br>Grouping<br>View<br>Parameter | 
| Filter (UIFT) |  Filter<br>Parameter | 
| Grouping (UIGB) | Grouping<br>Parameter | 
| View (UIVW) | View<br>Parameter | 

### Custom data objects

| Promotable object | Included sub-objects |
| --- | --- |
| Category (CTGY) | Category<br>Category Parameter<br>Parameter<br>Parameter Group<br>Parameter Option<br>Category Display Logic<br>Group | 
| Parameter (PARAM) | Parameter<br>Parameter Option | 
| Parameter Group (PGRP) | Parameter Group |

### Organization objects

| Promotable object | Included sub-objects |
| --- | --- |
| Group (GROUP) | Group <br>Sub-groups (up to 5 levels)<br>Category<br>Category Parameter<br>Parameter<br>Parameter Group<br>Parameter Option<br>Category Display Logic |
| Role (ROLE) | Role |
| Team (TEAM) | Team<br>Group |
| Company (CMPY) | Company<br>Override Rate<br>Category<br>Category Parameter<br>Parameter<br>Parameter Group<br>Parameter <br>Category Display Logic<br>Group |
| Portfolio (PORT) | Portfolio<br>Program<br>Group<br>Category<br>Category Parameter<br>Parameter<br>Parameter Group<br>Parameter Option<br>Category Display Logic |
| Program (PRGM) | Program<br>Portfolio<br>Group<br>Category<br>Category Parameter<br>Parameter<br>Parameter Group<br>Parameter Option<br>Category Display Logic |

### Other configuration objects

| Promotable object | Included sub-objects |
| --- | --- |
| Approval Process (ARVPRC) | Approval Process<br>Approval Path<br>Approval Step<br>Step Approver<br>Role<br>Team<br>Group |
| Schedule (SCHED) | Schedule<br>Non Work Day<br>Group |
| Milestone Path (MPATH) | Milestone Path<br>Milestone |
| Timesheet Profile (TSPRO) | Timesheet Profile<br>Hour Type |
| Hour Type (HOURT) | Hour Type |
| Expense Type (EXPTYP) | Expense Type |
| Risk Type (RSKTYP) | Risk Type |
| Resource Pool (RSPL) | Resource Pool |

## API Endpoints

* Obtaining a Bearer Token
* Create a package
* Get a list of packages
* Get a package by ID
* Get a package's configuration definition
* Replace a package details and definition
* Update specific properties of a package
* Delete a package
* Execute a pre-run
* Execute an installation
* Get a list of installations for a specific package
* Get the installation details for a installation

### Obtaining a Bearer Token

### Create a package

<table style="table-layout:auto"> 
 <col> 
 <tbody> 
  <tr> 
   <td><code>POST /packages</code></td> 
  </tr> 
  </tbody> 
</table>

This call executes a multi-step process. 

The first step results in the creation of an empty promotion package in the status of "EXTRACTING".

The second step uses the the `objectCollections` array provided in the POST body to assemble the requested records from Workfront. This step may take several minutes to complete, depending on the number of records requested and your Workfront configuration. At the end of this process, the empty promotion package is updated with the `packageEntities` and the status is automatically set to "BUILDING".


>[!NOTE]
>
>Note the structure of the `objectCollections`  array.
>
>Each item in the array contains an `objCode` key that corresponds to the object code documented in the Workfront API Explorer.
>
>Each item also contains an `entities` collection. This expects the `ID` and `name` keys to be present.
>
>For the list of allowed object codes to be requested in the `objectCollections` list, see the [Supported objects for environment promotion](#supported-objects-for-environment-promotion) section in this article.

#### URL

```
POST https://<domain>.<environment>.workfront.com/environment-promotion/v1/packages
```

#### Headers

```json
{
    "Authorization": "Bearer ****************",
    "Content-Type": "application/json"
}
```

#### Body

```json
{
    "packageName": "Agency Onboarding - 2023-06-06",
    "description": "This promotion package contains configuration to support the agency onboarding processes...",
    "source": "https://{{domain}}.{{env}}.workfront.com",
    "objectCollections": [
        {
            "objCode": "PROJ",
            "entities": [
                {
                    "ID": "6419b8b9001151ee258921a4f7597ba1",
                    "name": "Agency Request"
                }
            ]
        },
        {
            "objCode": "TMPL",
            "entities": [
                {
                    "ID": "6419b8b9001151ee258921a4f7597bb2",
                    "name": "New Agency Onboarding"
                },
                {
                    "ID": "6419b8b9001151ee258921a4f7597bc3",
                    "name": "New Agency Offboarding"
                }
            ]
        },
        {
            "objCode": "PTLTAB",
            "entities": [
                {
                    "ID": "645e6435000b4aaebe4776f4a42ed5ad",
                    "name": "Agency Performance and Readiness"
                }
            ]
        }
    ]
}
```

#### Response

```json
200
```

```json
{
    "data": {
        "id": "1d5693b9-b7b5-492d-8219-c21f34bcaca6",
        "name": "Agency Onboarding - 2023-06-06",
        "description": "This promotion package contains configuration to support the agency onboarding processes...",
        "status": "EXTRACTING",
        "version": 1,
        "installationCounts": {},
        "createdAt": "2023-06-06T17:29:21.600Z",
        "createdById": "61aa9d0e0005fcee8f212835bdaa2619",
        "publishedAt": null,
        "isPrivate": true,
        "customerId": "61aa9d090005fa42152c1cb66659f38d"
}
```

### Get a list of packages

<table style="table-layout:auto"> 
 <col> 
 <tbody> 
  <tr> 
   <td><code>GET /packages</code></td> 
  </tr> 
  </tbody> 
</table>

This call returns an unfiltered list of promotion packages belonging to the customer.

The response will include all packages created from any of the customer's sandbox, preview, or production instances of Workfront.

#### URL

```
GET https://{{domain}}.{{env}}.workfront.com/environment-promotion/v1/packages
```

#### Headers

```json
{
    "Authorization": "Bearer ****************"
}
```

#### Body

```json
<empty>
```

#### Response

```
200
```

```json
{
    "data": [
        {
            "id": "1d5693b9-b7b5-492d-8219-c21f34bcaca6",
            "name": "Agency Onboarding - 2023-06-06",
            "description": "This promotion package contains configuration to support the agency onboarding processes...",
            "status": "EXTRACTING",
            "version": 1,
            "installationCounts": {},
            "createdAt": "2023-06-06T17:29:21.600Z",
            "createdById": "61aa9d0e0005fcee8f212835bdaa2619",
            "publishedAt": null,
            "isPrivate": true,
            "customerId": "61aa9d090005fa42152c1cb66659f38d"
        },
        {...}
    ]
}
```

<!--table templates

<table style="table-layout:auto"> 
 <col> 
 <tbody> 
  <tr> 
   <td><code>POST /packages</code></td> 
  </tr> 
  </tbody> 
</table>

<table style="table-layout:fixed"> 
 <col> 
 <tbody> 
  <tr> 
   <td><b></b</td> 
  </tr> 
  <tr> 
   <td><pre></pre></td> 
  </tr> 
  </tbody> 
</table>
-->