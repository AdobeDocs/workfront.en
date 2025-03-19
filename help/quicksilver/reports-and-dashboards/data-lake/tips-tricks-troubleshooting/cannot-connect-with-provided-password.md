---
content-type: overview;reference
product-area: reports and dashboards
navigation-topic: data connect
title: Cannot connect with provided password
description: Troubleshoot Workfront Data Connect
author: Courtney
feature: Reports and Dashboards

---

# Power BI tool cannot connect with provided password 

## Problem

When you try and sign into Data Connect from your Power BI tool, you see the following error:

`Cannot connect from BI tool with provided password`

## Cause

The password provided on creating a JDBC connection is a temporary password. It will only work from the Snowflake login page at the URL provided on creating the connection profile. 

## Solution

You need to change your temporary password. 

### Reset connection password

1. Go to Workfront > Setup > System > Data Connect.
1. Create a new connection or open an exiting connection. 


Go into WF data connect setup > reset password > log into snowflake with the 



WF setup seytem > data connect >
 


Need to finish setting up profile by logging in with the link provided in WF and then they need to create a new password. 

javadata base connection

Cannot connect to Workfront Snowflake data warehouse from my home after adding my IP address to the allowlist while at work. - Different?