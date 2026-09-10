---
content-type: overview;reference
product-area: reports and dashboards
navigation-topic: data connect
title: Tableau Desktop cannot establish a connection
description: When you try to connect Tableau Desktop to Data Connect, you get an error.
author: Courtney
feature: Reports and Dashboards
exl-id: 2a25d99a-a05e-4f60-ae1a-51ee137ad5f3
TQID: https://experienceleague.adobe.com/-V1TT-X0FjMm2PIKDy0JVFkvt-A-a7f8fRbVzGzy1jg
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
    internal-label: Reporting
  - id: c1579802-ddd4-4214-8a91-97b2066abe11
    internal-label: Troubleshooting
  - id: d095671a-1355-40aa-8b5f-06c33c68080b
    internal-label: Security
---
# Tableau Desktop cannot establish a connection

## Problem

When you try to connect Tableau Desktop to Data Connect, you see the following error:

`Cannot load data into PowerBI. Receiving an HY000 [Microsoft][Snowflake] (25) message`

## Cause

This error is caused by a proxy setting on your local machine that prevents data from being loaded from Data Connect.

Data Connect is provided through third-party Snowflake cloud services. Tableau requires networking opened up to communicate with Snowflake.

## Solution

You can try the following to resolve this problem:

* **Troubleshoot by disabling your security tool**: Turn off your security tool, like Zscaler or Cisco, to see if it resolves the connectivity issue. If this resolves the connection issue, make sure that your security tool is upgraded to the latest version, add the Data Connect (Snowflake) IP address to the VPN allowlist with your internal network team.

* **Add IP Addresses to Allowlist**: Ensure that your firewall settings allow the IP addresses used by Data Connect. Use the command `SYSTEM$ALLOWLIST()` to obtain the IP address, which you can then allowlist in the VPN.

* **Check firewall and Proxy Settings**: Check if any firewall or proxy configurations on your network are blocking access to Snowflake's endpoints. You might need to contact your network administrator to add the required Snowflake IP addresses and ports to your company's allowlist.

* **Workaround option**: Create an extract from a worksheet screen instead of the Data Source pane in Tableau. The connection doesn't get lost and the extract process completes.
