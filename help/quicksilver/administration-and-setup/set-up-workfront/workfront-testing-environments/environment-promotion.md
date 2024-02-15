---
user-type: administrator
content-type: overview;how-to-procedural
product-area: system-administration
navigation-topic: workfront-testing-environments
title: Move objects from one environment to another
description: The Environment Promotion capability is intended to provide the ability to move configuration-related objects from one environment to another. It does not support the ability to move transactional objects (with limited exceptions).
author: Becky
feature: System Setup and Administration
role: Admin
hide: yes
hidefromtoc: yes
recommendations: noDisplay, noCatalog
exl-id: dd3c29df-4583-463a-b27a-bbfc4dda8184
---
# Move objects between [!DNL Workfront] environments using the [!DNL Workfront] Environment Promotion API

The Environment Promotion capability is intended to provide the ability to move configuration-related objects from one environment to another. You can move these objects using the Workfront API as described in this article.

For instructions on moving object between environments using the Workfront application, see:

* [Create or edit an environment promotion package](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion-create-pakcage.md)
* [Install an environment promotion package](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion-install-package.md)

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

For a list of promotable objects and their included promotable sub-objects, see [Supported objects for environment promotion](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion-in-wf.md#supported-objects-for-environment-promotion) in the article [Overview of moving objects between Workfront environments](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion-in-wf.md).

## Authentication

The API authenticates each request to ensure that the client has access to view or modify a requested object.

Authentication is performed by passing in a session ID or API key, which can be given using the following method:

### Request Header Authentication

The preferred method of authentication is to pass a request header named SessionID containing the session token. This has the advantage of being safe against [Cross-site Request Forgery (CSRF)](https://en.wikipedia.org/wiki/Cross-site_request_forgery) attacks and not interfering with the URI for caching purposes.

The following is an example of a request header:

```
GET /attask/api/v15.0/project/search
SessionID: abc1234
```

## API Endpoints

* [Create a package](#create-a-package)
* [Get a list of packages](#get-a-list-of-packages)
* [Get a package by ID](#get-a-package-by-id)
* [Update specific properties of a package](#update-specific-properties-of-a-package)
* [Delete a package](#delete-a-package)
* [Execute a pre-run](#execute-a-pre-run)
* [Execute an installation](#execute-an-installation)
* [Get a list of installations for a specific package](#get-a-list-of-installations-for-a-specific-package)
* [Get the installation details for an installation](#get-the-installation-details-for-an-installation)

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

The first step results in the creation of an empty promotion package in the status of "ASSEMBLING".

The second step uses the the `objectCollections` array provided in the POST body to assemble the requested records from Workfront. This step may take several minutes to complete, depending on the number of records requested and your Workfront configuration. At the end of this process, the empty promotion package is updated with the `packageEntities` and the status is automatically set to "DRAFT".


>[!NOTE]
>
>Note the structure of the `objectCollections`  array.
>
>Each item in the array contains an `objCode` key that corresponds to the object code documented in the Workfront API Explorer.
>
>Each item also contains an `entities` collection. This expects the `ID` field. It can also accept an optional `name` attribute to make it easier to know what the `ID` represents.
>
>For the list of allowed object codes to be requested in the `objectCollections` list, see the [Supported objects for environment promotion](#supported-objects-for-environment-promotion) section in this article.

#### URL

```
POST https://{domain}.{environment}.workfront.com/environment-promotion/api/v1/packages
```

#### Headers

```json
{
    "apikey": "**********",
    "Content-Type": "application/json"
}
```

Or

```json
{
    "sessionID": "*****************", 
    "Content-Type": "application/json"
}
```

#### Body

```json
{
    "name": "Agency Onboarding - 2023-06-06",
    "description": "This promotion package contains configuration to support the agency onboarding processes...",
    "source": "https://{domain}.{environment}.workfront.com",
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
        "source": "https://{domain}.{environment}.workfront.com",
        "status": "ASSEMBLING",
        "version": 1,
        "createdAt": "2023-06-06T17:29:21.600Z",
        "createdById": "61aa9d0e0005fcee8f212835bdaa2619",
        "publishedAt": null,
        "customerId": "61aa9d090005fa42152c1cb66659f38d"
    }
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
GET https://{domain}.{environment}.workfront.com/environment-promotion/api/v1/packages
```

#### Headers

```json
{
    "apikey": "**********"
}
```

Or

```json
{
    "sessionID": "*****************"
}
```

#### Body

_Empty_

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
            "status": "ASSEMBLING",
            "createdAt": "2023-06-06T17:29:21.600Z",
            "deletedAt": null
},
        {...}
    ]
}
```

<!--Check on "status" above--was it added?-->

### Get a package by ID

<table style="table-layout:auto"> 
 <col> 
 <tbody> 
  <tr> 
   <td><code>GET /packages/{id}</code></td> 
  </tr> 
  </tbody> 
</table>

This call returns a the details of a requested promotion package.

The request can be made through any environment regardless of the original source of the promotion package.

#### URL

```
GET https://{domain}.{environment}.workfront.com/environment-promotion/api/v1/packages/{id}
```

#### Headers

```json
{
    "apikey": "**********"
}
```

Or

```json
{
    "sessionID": "*****************"
}
```

#### Body

_Empty_

#### Response

```
200
```

```json
{
    "data": {
        "id": "1d5693b9-b7b5-492d-8219-c21f34bcaca6",
        "name": "Agency Onboarding - 2023-06-06",
        "description": "This promotion package contains configuration to support the agency onboarding processes...",
        "source": "https://{domain}.{environment}.workfront.com",
        "status": "DRAFT",
        "version": 1,
        "createdAt": "2023-06-06T17:29:21.600Z",
        "publishedAt": null,
        "customerId": "61aa9d090005fa42152c1cb66659f38d",
        "packageEntities": {
            "GROUP": [
               {
                   "id": "52aa9d0e0005fcee8f212835bdaa2691",
                   "name": "Default Group",
                   "description": "null"
                   - or -
                   "description": "..."
               }
            ],
            "ROLE": [
               {...}
            ],
            ...
        }
   }
}
```

### Update specific properties of a package

<table style="table-layout:auto"> 
 <col> 
 <tbody> 
  <tr> 
   <td><code>PATCH /packages/{id}</code></td> 
  </tr> 
  </tbody> 
</table>

This call updates any of the contents of the promotion package that are provided in the PATCH body.

The editable attributes are:

1. name (string)
1. description (string)
1. status (string with value validation)

For a detailed description of available statuses, see [Environment promotion statuses](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion-in-wf.md#environment-promotion-statuses) in the article [Overview of moving objects between Workfront environments](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion-in-wf.md).


#### URL

```
PATCH https://{domain}.{environment}.workfront.com/environment-promotion/api/v1/packages/{id}
```


#### Headers

```json
{
    "apikey": "**********",
    "Content-Type": "application/json"
}
```

Or

```json
{
    "sessionID": "*****************", 
    "Content-Type": "application/json"
}
```

#### Body

```json
{
    "status": "ACTIVE"
}
```

#### Response

```
200
```

```json
{
    "data": {
        "id": "1d5693b9-b7b5-492d-8219-c21f34bcaca6",
        "name": "Agency Onboarding - 2023-06-06",
        "description": "This promotion package contains configuration to support the agency onboarding processes...",
        "source": "https://{domain}.{environment}.workfront.com",
        "status": "ACTIVE",
        "version": 1,
        "createdAt": "2023-06-06T17:29:21.600Z",
        "publishedAt": "2023-06-06T19:39:01.600Z",
        "customerId": "61aa9d090005fa42152c1cb66659f38d",
        "packageEntities": {
            "GROUP": [
               {
                   "id": "52aa9d0e0005fcee8f212835bdaa2691",
                   "name": "Default Group",
                   "description": "..."
               }
            ],
            "ROLE": [
               {...}
            ],
            ...
        }
   }
}
```

### Delete a package

<table style="table-layout:auto"> 
 <col> 
 <tbody> 
  <tr> 
   <td><code>DELETE /packages/{id}</code></td> 
  </tr> 
  </tbody> 
</table>

This call deletes the promotion package record. This action is irreversible.

>[!NOTE]
>
>As opposed to deleting a promotion package, the recommendation is to change the status of the package to DISABLED. This will allow the package to be retrievable and retains the installation history of where it was deployed.

#### URL

```
DELETE https://{domain}.{environment}.workfront.com/environment-promotion/api/v1/packages/{id}
```

#### Headers

```json
{
    "apikey": "**********"
}
```

Or

```json
{
    "sessionID": "*****************"
}
```

#### Body

_Empty_

#### Response

```
200
```

```
Deleted
```

### Execute a pre-run

>[!IMPORTANT]
>
>Before you can execute an installation, you must execute this pre-run. You will use the ID generated from this call when you execute the installation.

<table style="table-layout:auto"> 
 <col> 
 <tbody> 
  <tr> 
   <td><code>POST  {customer-domain}/environment-promotion/api/v1/packages/{id}/prepare-installation</code></td> 
  </tr> 
  </tbody> 
</table>

This call conducts a comparison between the package definition and the target environment identified in the URL.

The result is a JSON body that identifies whether a promotion object is found or not in the target environment.

For each promotion object, one of the following `actions`  will be set:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>CREATE</td> 
   <td><p>When a corresponding record cannot be found in the target environment, the action is set to CREATE.</p><p>When this action is set in the <code>translationmap</code> that is provided to the <code>/install</code> endpoint, the installation service will create the record.</p></td> 
  </tr> 
  <tr> 
   <td>USEEXISTING</td> 
   <td><p>When a corresponding record is found in the target environment, the action is set to USEEXISTING and a <code>targetId</code> is also captured in the <code>translationmap</code>.</p><p>When this action is set in the <code>translationmap</code> that is provided to the <code>/install</code> endpoint, the installation service will not create the record. However, it will use the <code>targetId</code> included in the map entry for other objects that may have a reference to this record.</p><p>For example, a "Default Group" may be found in the target environment to which a package is being deployed. It is not possible to have two "Default Group" records, so the installation service will use the GUID for the existing group in any other object creation actions that include a reference to the "Default Group", such as a project, form, or any other entity that is related to this group.</p><p><b>Note:</b> <ul><li><p>When the USEEXISTING action is assigned, the existing record in the target environment will not be modified. </p><p>For example, if the description for the "Default Group" has changed in the sandbox where the package was built from, and the description value is different in the target environment, the value will remain unchanged after an installation with this <code>translationmap</code>.</li></ul></td> 
  </tr> 
  <tr> 
   <td>IGNORE</td> 
   <td><p>This action will not be automatically set.</p><p>It provides an ability to do a manual override of an assigned CREATE or USEEXISTING action before executing the <code>/install</code> call.</p><p><b>Notes: </b><ul><li><p>If a record that was originally set to CREATE is set to IGNORE, then any child records should also be set to IGNORE.</p><p>For example, if a Template record was mapped with a CREATE action, and the installing user wishes to exclude it from the deployment, they can set the Template's action to IGNORE.</p><p>In this case, if the installing user does not also set the Template Tasks, Template Task Assignments, Template Task Predecessors, Queue Definition, Queue Topics, Routing Rules, etc, to IGNORE, the deployment will result in a failed installation attempt.</p></li><li><p>If a record that was originally set to USEEXISTING is set to IGNORE, there may be some adverse effects during the installation process.</p><p>For example, if a Group record was mapped with the USEEXISTING action, and the installing user changes the action to IGNORE, for objects that require a group (e.g., a Project cannot exist without a group assigned), the system default group will be assigned to that project.</p></li><li><p>If a record that was originally set to USEEXISTING is set to CREATE, there may be some adverse effects during the installation process because many Workfront entities have unique name constraints.</p><p>For example, if a "Default Group" record was mapped with the USEEXISTING action, and the installing user changes the action to CREATE, because there is already a "Default Group" the installation attempt will fail to complete all the steps. Group names must be unique.</p><p>Some entities do not have a unique name constraint. For those objects, making this change will result in two identically named records. For example, Templates, Projects, Views, Filters, Groupings, Reports, and Dashboards do not require unique name constraints. It is a best practice to have unique names for these records, but it is not enforced.</p></li></ul></p></td> 
  </tr> 
  </tbody> 
</table>

There is currently no support for an UPDATE `action` in the alpha capabilities of this service. The option to allow for an UPDATE `action` is something we are researching.

#### URL

```
POST https://{domain}.{environment}.workfront.com/environment-promotion/api/v1/packages/:id/prepare-installation
```  
 
#### Headers 

```json
{
    "apikey": "**********",
    "Content-Type": "application/json"
}
``` 

Or

```json
{
    "sessionID": "*****************", 
    "Content-Type": "application/json"
}
``` 

#### Body

```json  
{}
``` 

#### Response

```
200
```

```json  
{
    "environmentPromotionPackageId": "45f2ae94-76c0-4b13-8f3b-f688de83043d",
    "environmentPromotionPackageVersion": 1,
    "id": "c0bc79bd-c9c1-4b5b-b118-b1241392de0e",
    "userId": "5ba38da500b752fd66439d4f6a9999a1",
    "customerId": "5ba38d9d00b74f0c7a38b1b487fc9710",
    "status": "PREPARING",
    "environment": "mmi.my.workfront.com",
    "registeredAt": "2023-10-19T20:00:16.697Z",
    "updatedAt": "2023-10-19T20:00:16.701Z",
    "translationMap": {
        "CTGY": {
            "62d9c9a0000013aeeefe7242a0a5fdb2": {
                "name": "Example Document Form",
                "action": "USEEXISTING",
                "isValid": true,
                "targetId": "62d9c9a0000013aeeefe7242a0a5fdb2"
            }
        },
        "PGRP": {
            "62d1eee4001c6618e6b9f9a588ba1598": {
                "name": "Asset Detail",
                "action": "USEEXISTING",
                "isValid": true,
                "targetId": "62d1eee4001c6618e6b9f9a588ba1598"
            }
        },
        "GROUP": {
            "5ba38da500b752b0f46d13186030b7ad": {
                "name": "Default Group",
                "action": "USEEXISTING",
                "isValid": true,
                "targetId": "5ba38da500b752b0f46d13186030b7ad"
            }
        },
        "PARAM": {
            "62d1eee400f8578895166ee91a83f97a": {
                "name": "Asset Type",
                "action": "USEEXISTING",
                "isValid": true,
                "targetId": "62d1eee400f8578895166ee91a83f97a"
            },
            "62d1eee50001407c713514a8970b58e4": {
                "name": "Keywords",
                "action": "USEEXISTING",
                "isValid": true,
                "targetId": "62d1eee50001407c713514a8970b58e4"
            },
            "62d1eee5000333ac3981ea4f3df6d88e": {
                "name": "Permitted Uses",
                "action": "USEEXISTING",
                "isValid": true,
                "targetId": "62d1eee5000333ac3981ea4f3df6d88e"
            },
            "62d1eee5000b188e9ec8039a097fc7ab": {
                "name": "File Format",
                "action": "USEEXISTING",
                "isValid": true,
                "targetId": "62d1eee5000b188e9ec8039a097fc7ab"
            },
            "62d1eee500100c159fd5f838ce560507": {
                "name": "CTA",
                "action": "USEEXISTING",
                "isValid": true,
                "targetId": "62d1eee500100c159fd5f838ce560507"
            },
            "62d9c988001c1f23954dbb9d646335b5": {
                "name": "Other CTA",
                "action": "USEEXISTING",
                "isValid": true,
                "targetId": "62d9c988001c1f23954dbb9d646335b5"
            },
            "62d9c9880070f546cf4c798ea6c3eaa4": {
                "name": "Other Audience",
                "action": "USEEXISTING",
                "isValid": true,
                "targetId": "62d9c9880070f546cf4c798ea6c3eaa4"
            },
            "62d9c990006258baf1b40f2569c3eab7": {
                "name": "Target Audience",
                "action": "USEEXISTING",
                "isValid": true,
                "targetId": "62d9c990006258baf1b40f2569c3eab7"
            }
        }
    }
}
``` 

>[!NOTE]
>
>The ID that you will need to execute the installation is the `id` field. In this example, the `id` field is third from the top, and has a value beginning with `c0bc79bd`.

### Execute an installation

>[!IMPORTANT]
>
>Before you can execute an installation, you must execute a pre-run. You will use the ID generated from the pre-run when you execute the installation.
>
>If any changes have been made to the destination environment (the environment that the package is being deployed to) after executing the pre-run, we recommend executing the pre-run again. If you do not execute the pre-run again, your execution may not complete accurately, or the installation may fail.
>
>For instructions on executing a pre-run, see [Execute a pre-run](#execute-a-pre-run).

<table style="table-layout:auto"> 
 <col> 
 <tbody> 
  <tr> 
   <td><code>POST /install</code></td> 
  </tr> 
  </tbody> 
</table>

This call initiates an installation attempt of a promotion package into the target environment identified in the POST URL.

#### URL

```
POST https://{domain}.{environment}.workfront.com/environment-promotion/api/v1/installations/{id}/install
```

#### Headers

```json
{
    "apikey": "**********",
    "Content-Type": "application/json"
}
```

Or

```json
{
    "sessionID": "*****************", 
    "Content-Type": "application/json"
}
```

#### Body

```json
{
}
```

#### Response

```
202
```


```json
{}
```

### Get a list of installations for a specific package

<table style="table-layout:auto"> 
 <col> 
 <tbody> 
  <tr> 
   <td><code>GET /v1/installations?environmentPromotionPackageId={environmentPromotionPackageId}
</code></td> 
  </tr> 
  </tbody> 
</table>

The results include installation events from all environments the package has been deployed to. They are not limited to the installations for the environment through which the request is being made. This allows you to identify which environments have received this package.

#### URL

```
GET https://{domain}.{environment}.workfront.com/environment-promotion/api/v1/installations?environmentPromotionPackageId={environmentPromotionPackageId}
```

#### Headers

```json
{
    "apikey": "**********"
}
```

Or

```json
{
    "sessionID": "*****************"
}
```

#### Body

_Empty_

#### Response

```
200
```

```json
[
    {
        "id": "2892b936-e09e-455a-935f-e1462ab9753c",
        "environmentPromotionPackageId": "4fae2b9d-d315-45f4-909f-a0c0d79fc65d",
        "environmentPromotionPackageVersion": 1,
        "userId": "8fbbc5bcf4f94a5b862483ee05573e73",
        "customerId": "54286d78b064451096752b99bf968481",
        "status": "INSTALLED",
        "environment": "https://{domain}.{environment}.workfront.com",
        "registeredAt": "2021-03-16T02:21:31.908Z",
        "updatedAt": null,
        "translationMap": {
            "ROLE": {
                "5f6d114f006883209828ddd9088e63b3": {
                    "name": "DAM Curator",
                    "action": "USEEXISTING",
                    "isValid": true,
                    "targetId": "600f4bed00028a718599f29575840053"
                },
                "ad535a9ebe647361e053a7656a0a1575": {
                    "name": "Copywriter",
                    "action": "USEEXISTING",
                    "isValid": true,
                    "targetId": "600f162700001ca051081c06667b14a4"
                },
                ...
            },
            "TMPL": {
                "5f9b317c00b3db5af69abcd1ed5f82aa": {
                    "name": "Digital Asset Production (Integrated)",
                    "action": "CREATE",
                    "isValid": true,
                    "targetId": "6054cda40000d5af63dc811d9c2b3a07"
                },
                ...
            },
            ...
        }
    },
    {...}
]
```

### Get the installation details for an installation

<table style="table-layout:auto"> 
 <col> 
 <tbody> 
  <tr> 
   <td><code>GET /installations/{id}</code></td> 
  </tr> 
  </tbody> 
</table>

This call will return the final `translationMap` produced by the installation service for a specific installation.

Each record will state what the prescribed `action` was and whether that action was successful or not.

For records with a CREATE `action` the `targetId` field will be set with the value of the newly created record in the target system. Additionally, the `installationStatus` field will be set to INSTALLED.

For records with the USEEXISTING `action` the `targetId` field will also be set, and the `installationStatus` field will be set to REGISTERED. This signifies that the mapping process was complete and the installation service acknowledges that it has evaluated the record and there is nothing to act on.

If the record has a CREATE `action` but it fails to successfully create the record, then the `installationStatus` will be set to FAILED and the reason for the failure will also be provided.

#### URL

```
GET https://{domain}.{environment}.workfront.com/environment-promotion/api/v1/installations/{id}
```

#### Headers

```json
{
    "apikey": "**********"
}
```

Or

```json
{
    "sessionID": "*****************"
}
```

#### Body

_Empty_

#### Response

```
200
```

```json
{
    "id": "2892b936-e09e-455a-935f-e1462ab9753c",
    "environmentPromotionPackageId": "4fae2b9d-d315-45f4-909f-a0c0d79fc65d",
    "environmentPromotionPackageVersion": 1,
    "userId": "8fbbc5bcf4f94a5b862483ee05573e73",
    "customerId": "54286d78b064451096752b99bf968481",
    "status": "INSTALLED",
    "environment": "https://{domain}.{environment}.workfront.com",
    "registeredAt": "2021-03-16T02:21:31.908Z",
    "updatedAt": null,
    "translationMap": {
        "ROLE": {
            "5f6d114f006883209828ddd9088e63b3": {
                "name": "DAM Curator",
                "action": "USEEXISTING",
                "isValid": true,
                "targetId": "600f4bed00028a718599f29575840053"
            },
            ...
        },
        "TMPL": {
            "5f9b317c00b3db5af69abcd1ed5f82aa": {
                "name": "Digital Asset Production (Integrated)",
                "action": "CREATE",
                "isValid": true,
                "targetId": "6054cda40000d5af63dc811d9c2b3a07"
            },
            ...
        },
        ...
    }
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
   <td><b></b></td> 
  </tr> 
  <tr> 
   <td><pre></pre></td> 
  </tr> 
  </tbody> 
</table>
-->
