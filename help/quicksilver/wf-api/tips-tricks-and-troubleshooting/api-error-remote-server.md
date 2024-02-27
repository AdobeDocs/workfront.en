---
content-type: api;tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-api
title: API error message 400 Bad Request
description: API error message 400 Bad Request
author: Becky
feature: Workfront API
role: Developer
exl-id: ab7c76a9-16ce-41f9-b7af-5943eb2dfdff
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
