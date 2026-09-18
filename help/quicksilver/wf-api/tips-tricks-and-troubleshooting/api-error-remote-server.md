---
content-type: api;tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-api
title: API error message 400 Bad Request
description: API error message 400 Bad Request
author: Becky
feature: Workfront API
role: Developer
exl-id: ab7c76a9-16ce-41f9-b7af-5943eb2dfdff
TQID: https://experienceleague.adobe.com/19PIdv4u8de0BlasXD0Yy6GssO3vv6Jt8BzcljB-m1w
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: b58ad82f-df6b-4b01-81a3-3a02ab9567a0
    internal-label: APIs
role_v2:
  - id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
    internal-label: Developer
topic_v2:
  - id: c1579802-ddd4-4214-8a91-97b2066abe11
    internal-label: Troubleshooting
---
# API Error: "The remote server returned an error (400) Bad Request"

## Problem

You get the following error while attempting to use the API to import a custom field to an issue:

`The remote server returned an error: (400) Bad Request`

## Cause

This error occurs when you try to import, via the API, a custom field from a project that does not have a custom form associated with a Queue Topic.

## Solution

Add the correct custom form to the Queue Topic.

To learn more about Queue Topics, see [Create Queue Topics](../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md).
