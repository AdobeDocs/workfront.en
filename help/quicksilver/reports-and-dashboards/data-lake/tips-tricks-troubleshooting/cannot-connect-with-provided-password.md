---
content-type: overview;reference
product-area: reports and dashboards
navigation-topic: data connect
title: Cannot connect with provided password
description: Troubleshoot Workfront Data Connect
author: Courtney
feature: Reports and Dashboards

---

# Cannot connect with provided password 

## Problem

You receive the following error when ___

_Cannot connect from BI tool with provided password_

## Cause

The password provided on creating a JDBC connection is a temporary password. It will only work from the Snowflake login page at the URL provided on creating the connection profile. 

## Solution

Reset the password and then try to establish a connection from your BI tool.

