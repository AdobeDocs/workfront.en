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
| Approval Process (ARVPRC) | Approval Process<br>Approval Path
Approval Step
Step Approver
Role
Team
Group |
| --- | --- |
| --- | --- |
| --- | --- |
| --- | --- |
| --- | --- |
| --- | --- |
| --- | --- |
| --- | --- |




