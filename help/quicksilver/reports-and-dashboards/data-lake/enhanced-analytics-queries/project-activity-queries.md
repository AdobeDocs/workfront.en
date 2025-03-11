---
content-type: overview;reference
product-area: reports and dashboards
navigation-topic: data connect
title: Project activity queries
description: Enhanced Analytics queries
author: Courtney
feature: Reports and Dashboards
recommendations: noDisplay, noCatalog
hide: yes
hidefromtoc: yes
exl-id: b7155160-4537-4919-bebf-72056b181bb6
---
# Project activity queries

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

## Projects users' login events 

Shows the number people assigned to the project who logged in on a given day.

```
WITH userlogins as ( 
    SELECT 
        userid, 
        lastlogindate 
    FROM ( 
        SELECT 
            userid, 
            lastlogindate, 
            lag(lastlogindate, 1, '1990-01-01') OVER (PARTITION BY userid ORDER BY begin_effective_timestamp) as previous_login 
        FROM users_event 
    ) 
    WHERE lastlogindate != previous_login 
) 
 
SELECT 
    tds.projectid, 
    ads.calendardate, 
    count(1) 
FROM assignments_daily_history ads 
    INNER JOIN tasks_daily_history tds ON ads.taskid = tds.taskid AND tds.calendardate = ads.calendardate 
    INNER JOIN userlogins ul ON ads.assignedtoid = ul.userid and TO_DATE(ul.lastlogindate) = ads.calendardate 
GROUP BY tds.projectid, ads.calendardate
```

### Projects users' login events: drill down

```
WITH userlogins as ( 
    SELECT 
        userid, 
        lastlogindate 
    FROM ( 
        SELECT 
            userid, 
            lastlogindate, 
            lag(lastlogindate, 1, '1990-01-01') OVER (PARTITION BY userid ORDER BY begin_effective_timestamp) as previous_login 
        FROM users_event 
    ) 
    WHERE lastlogindate != previous_login 
) 

SELECT 
    tds.projectid, 
    ul.userid, 
    ads.calendardate, 
    count(1) 
FROM assignments_daily_history ads 
INNER JOIN tasks_daily_history tds ON ads.taskid = tds.taskid AND tds.calendardate = ads.calendardate 
INNER JOIN userlogins ul ON ads.assignedtoid = ul.userid AND TO_DATE(ul.lastlogindate) = ads.calendardate 
group by tds.projectid, ul.userid, ads.calendardate
 
```

## Projects users' task status change events 

Shows the number of people who changed the status of a task for the project on a given day.

```
WITH task_status_changes as (  
    SELECT 
        taskid, 
        status, 
        begin_effective_timestamp  
    FROM (  
        SELECT 
            taskid, 
            status, 
            begin_effective_timestamp, 
            lag(status, 1, 'NOSTATUS') OVER (PARTITION BY taskid ORDER BY begin_effective_timestamp) as previous_status 
        FROM tasks_event 
        WHERE status != 'CPL' 
    )  
    WHERE status != previous_status  
)  
 
SELECT 
    tds.projectid, 
    count(tds.status), 
    ads.calendardate 
FROM assignments_daily_history ads 
    INNER JOIN tasks_daily_history tds ON ads.taskid = tds.taskid AND tds.calendardate = ads.calendardate 
    INNER JOIN task_status_changes tsc ON tsc.taskid = ads.taskid AND tsc.taskid = tds.taskid and TO_DATE(tsc.begin_effective_timestamp) = tds.calendardate 
GROUP BY tds.projectid, ads.calendardate
```

### Projects users' task status change events: drill down

```
WITH task_status_changes as (  
    SELECT 
        taskid, 
        status, 
        lastupdatedbyid, 
        begin_effective_timestamp  
    FROM (  
        SELECT 
            taskid, 
            status, 
            begin_effective_timestamp, 
            lastupdatedbyid, 
            lag(status, 1, 'NOSTATUS') OVER (PARTITION BY taskid ORDER BY begin_effective_timestamp) as previous_status  
        FROM tasks_event  
        WHERE status != 'CPL'  
    )  
    WHERE status != previous_status  
)  
 
SELECT 
    tds.projectid, 
    tsc.lastupdatedbyid, 
    count(tcs.status), 
    ads.calendardate 
FROM assignments_daily_history ads 
    INNER JOIN tasks_daily_history tds ON ads.taskid = tds.taskid AND tds.calendardate = ads.calendardate 
    INNER JOIN task_status_changes tsc ON tsc.taskid = ads.taskid AND tsc.taskid = tds.taskid AND TO_DATE(tsc.begin_effective_timestamp) = tds.calendardate 
GROUP BY tds.projectid, tsc.lastupdatedbyid, ads.calendardate
```

## Projects users' task completion events 

Show the number of people who completed a task for the project on a given day.

```
WITH task_status_changes as (  
    SELECT 
        taskid, 
        status, 
        begin_effective_timestamp  
    FROM (  
        SELECT 
            taskid, 
            status, 
            begin_effective_timestamp, 
            lag(status, 1, 'NOSTATUS') OVER (PARTITION BY taskid ORDER BY begin_effective_timestamp) as previous_status  
        FROM tasks_event  
        WHERE status = 'CPL'  
    )  
    WHERE status != previous_status  
) 
 
SELECT 
    tds.projectid, 
    count(tds.status), 
    ads.calendardate 
FROM assignments_daily_history ads 
    INNER JOIN tasks_daily_history tds ON ads.taskid = tds.taskid and tds.calendardate = ads.calendardate 
    INNER JOIN task_status_changes tsc ON tsc.taskid = ads.taskid and tsc.taskid = tds.taskid and TO_DATE(tsc.begin_effective_timestamp) = tds.calendardate 
GROUP BY tds.projectid, ads.calendardate
```

### Projects users' task completion events: drill down

```
WITH task_status_changes as (  
    SELECT 
        taskid, 
        status, 
        lastupdatedbyid, 
        begin_effective_timestamp  
    FROM (  
        SELECT 
            taskid, 
            status, 
            begin_effective_timestamp, 
            lastupdatedbyid, 
            lag(status, 1, 'NOSTATUS') OVER (PARTITION BY taskid ORDER BY begin_effective_timestamp) as previous_status  
        FROM tasks_event  
        WHERE status = 'CPL'  
    )  
    WHERE status != previous_status  
)  
 
SELECT 
    tds.projectid, 
    tsc.lastupdatedbyid, 
    count(tsc.status), 
    ads.calendardate 
FROM assignments_daily_history ads 
    INNER JOIN tasks_daily_history tds ON ads.taskid = tds.taskid AND tds.calendardate = ads.calendardate 
    INNER JOIN task_status_changes tsc ON tsc.taskid = ads.taskid AND tsc.taskid = tds.taskid AND TO_DATE(tsc.begin_effective_timestamp) = tds.calendardate 
GROUP BY tds.projectid, tsc.lastupdatedbyid, ads.calendardate
```