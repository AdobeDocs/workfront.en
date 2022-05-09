---
filename: calculate-spi
content-type: overview;how-to-procedural
product-area: projects
navigation-topic: financials
title: Calculate Schedule Performance Index (SPI)
description: Calculate Schedule Performance Index (SPI)
---

# Calculate Schedule Performance Index (SPI)

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Linked to the product. Do not change link.)</p>
-->

The Schedule Performance Index (SPI) describes the relationship between the planned schedule and actual schedule.&nbsp;Adobe Workfront calculates SPI&nbsp;at the project and task levels. Project managers review this metric to identify whether tasks or projects are currently tracking ahead of or behind schedule. &nbsp;

## Access requirements

You must have the following access to perform the steps in this article:

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Review or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>View access to Projects and Financial&nbsp;Data</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View or higher permissions to the project with permissions to View Finance</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your Workfront administrator.

## Schedule Performance Index (SPI) overview

* [What the SPI value shows](#what-the-spi-value-shows) 
* [How Workfront calculates SPI](#how-workfront-calculates-spi)

### What the SPI&nbsp;value shows {#what-the-spi-value-shows}

Project managers understand that a SPI&nbsp;value of 1 means the project is on plan or on schedule. &nbsp;Values greater than 1 indicate a project is ahead of schedule, and values less than 1 mean a project is behind schedule. &nbsp;The further from 1, the greater deviation from the plan.

| **SPI Value** |**Indication of "On Schedule"** |
|---|---|
| 1 |On plan or on schedule |
| > 1 (greater than 1) |Ahead of schedule |
| < 1 (less than 1) |Behind schedule |

### How Workfront calculates SPI  {#how-workfront-calculates-spi}

Workfront calculates SPI by the following formula:

```
SPI = (Total Planned Hours x % Complete) / Planned Hours Scheduled to Date*
```

*&#42;If Planned Hours Scheduled to Date = 0, SPI = 1*.

Planned Hours Schedule to Date are calculated at the minute when you perform&nbsp;the calculations. It shows the number of Planned Hours planned to the current date.&nbsp;It can be recalculated automatically when you change your finance data to be accurate. There is no&nbsp;field in Workfront that indicates&nbsp;this value.

For example, if you have a project with 1 task and the task has 10 planned hours and a 10-day Duration, the Planned Hours Schedule to Date on the 5th day are&nbsp;5.&nbsp;

## Locate SPI in a project or task

1. Go to the project or task where you want to view SPI.
1. Depending on whether you want to view SPI on a project or a task, do one of the following:

   1. Click **Project Details** in the left panel, then view the **Finance** area.
   
   1. Click **Task Details** in the left panel, then view the **Finance** area.

      ![](assets/spi-on-project-nwe.png)

1. Find the **CPI/ SPI/ CSI** field.

