---
user-type: administrator
content-type: overview;how-to-procedural
product-area: system-administration
navigation-topic: workfront-testing-environments
title: Move objects from one environment to another within Workfront
description: The Environment Promotion capability is intended to provide the ability to move configuration-related objects from one environment to another. It does not support the ability to move transactional objects (with limited exceptions).
author: Becky
feature: System Setup and Administration
role: Admin
hide: yes
hidefromtoc: yes
recommendations: noDisplay, noCatalog
exl-id: 8b4c04f5-f519-44e9-8429-0ce80c2d7c5b
---
# Overview of moving objects between Workfront environments (Environment promotion)

The environment promotion capability is intended to provide the ability to move objects from one Workfront environment to another. For example, you can create a template and configure it in your sandbox environment, knowing that any testing you do will not affect your organization's actual data. After the template is configured and tested, you can move it to your production environment, ready to use.

This process is referred to as "environment promotion."

You can perform this process in Workfront by creating a package of objects to move, and then installing that package in the new environment.

* For specific instructions on performing this process within Workfront, see:

   * [Create or edit an environment promotion package](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion-create-package.md)
   * [Install an environment promotion package](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion-install-package.md)

* For instructions on performing this process through the Workfront API, see [Move objects between [!DNL Workfront] environments using the [!DNL Workfront] API](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion.md).

## Supported objects for environment promotion

The Environment Promotion capability is intended to provide the ability to move configuration-related objects from one environment to another. It does not support the ability to move transactional objects (with limited exceptions).

* [Work objects](#work-objects)
* [Reporting objects](#reporting-objects)
* [Custom data objects](#custom-data-objects)
* [Organization objects](#organization-objects)
* [Other configuration objects](#other-configuration-objects)


### Work objects

| Promotable object | Included promotable linked objects |
| --- | --- |
| Project (PROJ) | Project<br>Task<br>Assignment<br>Predecessor<br>Company<br>Override Rate<br>Group<br>Role<br>Team<br>Approval Process<br>Approval Path<br>Approval Step<br>Step Approver<br>Schedule<br>Non Work Day<br>Queue Definition<br>Queue Topic Group<br>Queue Topic<br>Routing Rule<br>Milestone Path<br>Milestone<br>Hour Type<br>Resource Pool<br>Category<br>Category Parameter<br>Parameter<br>Parameter Group<br>Parameter Option<br>Category Display Logic | 
| Template (TMPL) | Template<br>Template Task<br>Template Task Assignment<br>Template Task Predecessor<br>Company<br>Override Rate<br>Group<br>Role<br>Team<br>Approval Process<br>Approval Path<br>Approval Step<br>Step Approver<br>Schedule<br>Non Work Day<br>Queue Definition<br>Queue Topic Group<br>Queue Topic<br>Routing Rule<br>Milestone Path<br>Milestone<br>Hour Type<br>Resource Pool<br>Category<br>Category Parameter<br>Parameter<br>Parameter Group<br>Parameter Option<br>Category Display Logic | 

### Reporting objects

| Promotable object | Included promotable linked objects |
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

| Promotable object | Included promotable linked objects |
| --- | --- |
| Category (CTGY) | Category<br>Category Parameter<br>Parameter<br>Parameter Group<br>Parameter Option<br>Category Display Logic<br>Group | 
| Parameter (PARAM) | Parameter<br>Parameter Option | 
| Parameter Group (PGRP) | Parameter Group |

### Organization objects

| Promotable object | Included promotable linked objects |
| --- | --- |
| Group (GROUP) | Group <br>Sub-groups (up to 5 levels) *<br>Category<br>Category Parameter<br>Parameter<br>Parameter Group<br>Parameter Option<br>Category Display Logic |
| Role (ROLE) | Role |
| Team (TEAM) | Team<br>Group |
| Company (CMPY) | Company<br>Override Rate<br>Category<br>Category Parameter<br>Parameter<br>Parameter Group<br>Parameter <br>Category Display Logic<br>Group |
| Portfolio (PORT) | Portfolio<br>Program<br>Group<br>Category<br>Category Parameter<br>Parameter<br>Parameter Group<br>Parameter Option<br>Category Display Logic |
| Program (PRGM) | Program<br>Portfolio<br>Group<br>Category<br>Category Parameter<br>Parameter<br>Parameter Group<br>Parameter Option<br>Category Display Logic |

### Other configuration objects

| Promotable object | Included promotable linked objects |
| --- | --- |
| Approval Process (ARVPRC) | Approval Process<br>Approval Path<br>Approval Step<br>Step Approver<br>Role<br>Team<br>Group |
| Schedule (SCHED) | Schedule<br>Non Work Day<br>Group |
| Milestone Path (MPATH) | Milestone Path<br>Milestone |
| Timesheet Profile (TSPRO) | Timesheet Profile<br>Hour Type |
| Hour Type (HOURT) | Hour Type |
| Expense Type (EXPTYP) | Expense Type |
| Risk Type (RSKTYP) | Risk Type |
| Resource Pool (RSPL) | Resource Pool |

\* Not currently available 

>[!NOTE]
>
>Overwriting is currently available for the following objects:
>
>* Role
>* Team
>* Company
>* Group


## Environment promotion statuses

Environment promotion packages proceed through several statuses as they are created and prepared to move between environments. You can see these statuses in your list of packages inside Workfront, or in the API responses if you are using the Workfront API. 

These statuses include the following:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>ASSEMBLING</td> 
   <td><p>This status is automatically assigned while objects are being assembled. </p><p>Assembling refers to the automated process of identifying objects and sub-objects to include in a package, and adding those objects and their data to the package.</p><p>This status cannot be set by a customer directly.</p></td> 
  </tr> 
  <tr> 
   <td>DRAFT</td> 
   <td><p>This status is assigned at the conclusion of an assembly process, or when creating an empty promotion package.</p><p>It is possible for a customer to move the promotion package back to this status.</p><p>While in this status, the promotion package cannot be installed in any environment.</p></td> 
  </tr> 
  <tr> 
   <td>TESTING</td> 
   <td><p>This status allows a promotion package to be installed in any Preview or Custom Refresh sandbox. While in this status, the package cannot be installed in Production.</p></td> 
  </tr> 
  <tr> 
   <td>ACTIVE</td> 
   <td><p>This status allows a promotion package to be installed in any environment, including Production.</p><p>When a package status is set to ACTIVE, the <code>publishedAt</code> date is automatically set to the current timestamp of the request.</p></td> 
  </tr> 
  <tr> 
   <td>DISABLED</td> 
   <td><p>This status will be used to hide previously used promotion packages that will not be installed into any environment in the future.</p><p>When a package is in this status, it cannot be installed into any environment.</p><p>When a package status is set to DISABLED, the <code>retiredAt</code> date is automatically set to the current timestamp of the request.</p><p>Using this status is recommended over using the<code>DELETE /package</code> endpoint because it is retrievable and the installation history is retained for any deployments made with this package.</p></td> 
  </tr> 
  <tr> 
   <td>ASSEMBLING_FAILED</td> 
   <td><p>The promotion package is automatically put in this status if the ASSEMBLING stage fails.</p><p>To return the package to the ASSEMBLING stage, you must trigger the extraction process again.</p></td> 
  </tr> 
  </tbody> 
</table>

