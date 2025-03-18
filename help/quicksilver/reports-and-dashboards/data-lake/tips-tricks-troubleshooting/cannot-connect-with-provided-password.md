---
content-type: overview;reference
product-area: reports and dashboards
navigation-topic: data connect
title: Cannot connect with provided password
description: Troubleshoot Workfront Data Connect
author: Courtney
feature: Reports and Dashboards

---

# Power BI tool Cannot connect with provided password 

## Problem

When you try and sign into Snowflake from your Power BI tool, you see the following error:

`Cannot connect from BI tool with provided password`

## Cause

The password provided on creating a JDBC connection is a temporary password. It will only work from the Snowflake login page at the URL provided on creating the connection profile. 

## Solution

Reset the password and then try to establish a connection from your BI tool.





Cannot connect to Workfront Snowflake data warehouse from my home after adding my IP address to the allowlist while at work. - Different?