---
content-type: overview;reference
product-area: reports and dashboards
navigation-topic: data connect
title: KPI queries
description: Enhanced Analytics queries
author: Courtney
feature: Reports and Dashboards
recommendations: noDisplay, noCatalog
hide: yes
hidefromtoc: yes
---

# KPI queries

You can use the queries in this article to create data visualizations similar to those in Enhanced Analytics.

>[!IMPORTANT]
>
>Queries will produce similar results to those shown in Enhanced Analytics, but they may not match exactly.


## Prerequisites

Before you begin, you must

1. Establish a connection with your Business Intelligence (BI) tool:
    1. [Create a reader account or connection for Snowflake](/help/quicksilver/reports-and-dashboards/data-lake/create-a-reader-account.md)
    1. [Establish a connection to Workfront Data Connect](/help/quicksilver/reports-and-dashboards/data-lake/share-data-externally.md)

Once you establish a connection, you can use the queries in this aticle to extract and visualize data.

## Projects completed

The Projects completed KPI shows how many projects within the filtered time period have been completed, as well as how the percentage increased or decreased since the previous time period. Below these numbers, you can see the number of projects completed in the previous time period, as well as the number of days in the previous time period.

![KPI projects completed](assets/kpi-projects-completed-350x182.png)

### Query

```
WITH completedProjectsInRange as ( 
SELECT COUNT(t0.PROJECTID) as PROJECT_COUNT FROM PROJECTS_CURRENT t0 
WHERE t0.ACTUALCOMPLETIONDATE >= '2025-01-01' 
AND t0.ACTUALCOMPLETIONDATE <= '2025-01-31' 
), completedProjectsPreviousRange as ( 
SELECT COUNT(t0.PROJECTID) as PROJECT_COUNT FROM PROJECTS_CURRENT t0 
WHERE t0.ACTUALCOMPLETIONDATE >= '2024-12-01' 
AND t0.ACTUALCOMPLETIONDATE <= '2024-12-31' 
), rawChange as ( 
SELECT (a.PROJECT_COUNT - b.PROJECT_COUNT) as CHANGE_FROM_PREVIOUS_PERIOD FROM completedProjectsInRange a, completedProjectsPreviousRange b 
), percentChange as ( 
SELECT  
CASE 
WHEN a.PROJECT_COUNT = b.PROJECT_COUNT THEN 0.00 
WHEN b.PROJECT_COUNT > 0 THEN ((a.PROJECT_COUNT - b.PROJECT_COUNT) / b.PROJECT_COUNT * 100) 
END AS PERCENT_CHANGE_FROM_PREVIOUS_PERIOD 
FROM completedProjectsInRange a, completedProjectsPreviousRange b 
) 
SELECT 
a.PROJECT_COUNT, 
b.PROJECT_COUNT as PREVIOUS_PROJECT_COUNT, 
c.CHANGE_FROM_PREVIOUS_PERIOD, 
d.PERCENT_CHANGE_FROM_PREVIOUS_PERIOD 
FROM completedProjectsInRange a, completedProjectsPreviousRange b, rawChange c, 
percentChange d

```
## Projects completed on time

The Projects completed on time KPI shows the percentage of projects within the filtered time period that were completed on time, as well as how the percentage increased or decreased since the previous time period. Below these numbers, you can see the percentage of projects completed on time in the previous time period, as well as the number of days in the previous time period.

![KPI projects completed on time](assets/kpi-projects-completed-on-time-350x180.png)

## Avg. project duration

The Avg. project duration KPI shows the average amount of completion time—in days, weeks, or years—for projects with actual end dates within the filtered time period, as well as how the percentage increased or decreased since the previous time period. Below these numbers, you can see the average amount of completion time for projects with actual end dates in the previous time period, as well as the number of days in the previous time period.

![KPI average project duration](assets/kpi-avg.-project-duration-350x168.png)

## Average tasks per project

The Avg, tasks per project KPI shows the average number of tasks assigned to projects within the filtered time period, as well as how the percentage increased or decreased since the previous time period. Below these numbers, you can see the the average number of tasks assigned to projects in the previous time period, as well as the number of days in the previous time period.

![KPI average tasks per project](assets/kpi-average-tasks-per-project-350x179.png)