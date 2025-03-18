---
content-type: overview;reference
product-area: reports and dashboards
navigation-topic: data connect
title: Cannot load data
description: Troubleshoot Workfront Data Connect
author: Courtney
feature: Reports and Dashboards

---

# Tableau Desktop cannot establish a connection

## Problem

When you try and connect Tableau Desktop to Snowflake, you see the following error:

`Cannot load data into PowerBI. Receiving an HY000 [Microsoft][Snowflake] (25) message`

## Cause

This is caused by a proxy setting on your local machine that prevents data from being loaded from Snowflake.

^ is this

## Solution

You can try the following to resolve this problem:

* Troubleshooting option: Turn off Zscaler to see if it resolves the connectivity issue.

* Workaround option: Create an extract from a worksheet screen instead of the Data Source pane in Tableau. The connection doesn't get lost and the extract process completes.

Tableau recommended resolution: Upgrade Zscaler to latest version, and add IP address to the VPN allowlist with your internal network team.

Snowflake recommended resolution: Use the command SYSTEM$ALLOWLIST() to obtain the IP address, which you can then whitelist in the VPN. Please let us know if this resolves the issue."