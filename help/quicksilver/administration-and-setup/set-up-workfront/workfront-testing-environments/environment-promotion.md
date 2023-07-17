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
| Project (PROJ) | <p>Project</p><p>Task</p><p>Assignment</p><p>Predecessor</p><p>Company</p><p>Override Rate</p><p>Group</p><p>Role</p><p>Team</p><p>Approval Process</p><p>Approval Path</p><p>Approval Step</p><p>Step Approver</p><p>Schedule</p><p>Non Work Day</p><p>Queue Definition</p><p>Queue Topic Group</p><p>Queue Topic</p><p>Routing Rule</p><p>Milestone Path</p><p>Milestone</p><p>Hour Type</p><p>Resource Pool</p><p>Category</p><p>Category Parameter</p><p>Parameter</p><p>Parameter Group</p><p>Parameter Option</p><p>Category Display Logic</p> |
| Template (TMPL) | <p>Template</p><p>Template Task</p><p>Template Task Assignment</p><p>Template Task Predecessor</p><p>Company</p><p>Override Rate</p><p>Group</p><p>Role</p><p>Team</p><p>Approval Process</p><p>Approval Path</p><p>Approval Step</p><p>Step Approver</p><p>Schedule</p><p>Non Work Day</p><p>Queue Definition</p><p>Queue Topic Group</p><p>Queue Topic</p><p>Routing Rule</p><p>Milestone Path</p><p>Milestone</p><p>Hour Type</p><p>Resource Pool</p><p>Category</p><p>Category Parameter</p><p>Parameter</p><p>Parameter Group</p><p>Parameter Option</p><p>Category Display Logic</p> |

### Reporting objects

| Promotable object | Included sub-objects |
| --- | --- |
| Layout Template (UITMPL) | <p>Layout Template</p><p>Dashboard</p><p>Calendar</p><p>Calendar Section</p><p>External Page</p><p>Report</p><p>Filter</p><p>Grouping</p><p>View</p><p>Parameter </p> |
| Dashboard (PTLTAB) | <p>Dashboard</p><p>Calendar</p><p>Calendar Section</p><p>External Page</p><p>Report</p><p>Filter</p><p>Grouping</p><p>View</p><p>Parameter </p> |
| Calendar (CALEND) | <p>Calendar</p><p>Calendar Section</p> |
| External Page (EXTSEC) | External Page |
| Report (PTLSEC) | <p>Report</p><p>Filter</p><p>Grouping</p><p>View</p><p>Parameter</p> |
| Filter (UIFT) | <p> Filter</p><p>Parameter</p> |
| Grouping (UIGB) | <p>Grouping</p><p>Parameter</p> |
| View (UIVW) | <p>View</p><p>Parameter</p> |

### Custom data objects

| Promotable object | Included sub-objects |
| --- | --- |
| Category (CTGY) | <p>Category</p><p>Category Parameter</p><p>Parameter</p><p>Parameter Group</p><p>Parameter Option</p><p>Category Display Logic</p><p>Group</p> |
| Parameter (PARAM) | <p>Parameter</p><p>Parameter Option</p> |
| Parameter Group (PGRP) | Parameter Group |

### Organization Objects

| Promotable object | Included sub-objects |
| --- | --- |




