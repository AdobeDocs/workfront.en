---
content-type: overview;how-to-procedural
product-area: projects
navigation-topic: financials
title: Calculate Cost Schedule Performance Index (CSI)
description: The Cost Schedule Performance Index (CSI) is an automatic calculation which combines the Cost Performance Index (CPI) and Schedule Performance Index (SPI) into one general metric that balances cost and schedule.
author: Alina
feature: Work Management
exl-id: 38a8c5e0-b812-499d-8fe7-a71ddccb3aad
---
# Calculate Cost Schedule Performance Index (CSI)

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Linked to the product. Do not change link.) </p>
-->

## Overview of the Cost Schedule Performance Index (CSI)

The Cost Schedule Performance Index (CSI) is an automatic calculation which combines the Cost Performance Index (CPI) and Schedule Performance Index (SPI) into one general metric that balances cost and schedule. By multiplying these values together, a single metric can account for a protracted schedule at a lower budget or vice versa. Project managers may use this to determine general project or task health when cost is sacrificed to drive schedule mid-project.

>[!TIP]
>
>Adobe Workfront calculates CSI for both tasks and projects. Workfront does not calculate a CSI value for issues.

You can benefit from the information provided by this metric only if the following exist in your organization:

* Your users are logging time for the work they complete.  
  This calculates CSI based on Hours.
* Your users or job roles have Cost per Hour rates associated with them.&nbsp;

  This calculates CSI based on Costs.

## How Workfront calculates the Cost Schedule Performance Index (CSI)

Workfront calculates the Cost Performance Index (CSI) of a project or task using the following formula:

`CSI = CPI x SPI`

For information about CPI, see the article [Calculate Cost Performance Index (CPI)](../../../manage-work/projects/project-finances/calculate-cpi.md).

For information about SPI, see the article [Calculate Schedule Performance Index (SPI)](../../../manage-work/projects/project-finances/calculate-spi.md).

CSI has the following three possible values:

* 1 = Follows overall plan
* \>1 = Under budget schedule combination
* <1 = Over budget schedule combination

![](assets/csi-highlighted.png)

## Locate the Cost Schedule Performance Index (CSI)

>[!CAUTION]
>
>You must have access to View Financial Data in your Access Level and permissions to View the project or task in order to be able to see the CSI value of a project or task.

You can locate CSI in the following areas of Workfront:

* Finance area in the Project Details section. 
* Finance area in the Task Details section. 
* A project or task view
* A project or task report
