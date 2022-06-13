---
content-type: api;tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-api
title: "API Error: “The remote server returned an error: (400) Bad Request”"
description: You get the following error while attempting to use the API to import a custom field to an issue - EDIT ME.
feature: Workfront API
---

# API Error: “The remote server returned an error: (400) Bad Request”

## Problem

You get the following error while attempting to use the API to import a custom field&nbsp;to an issue:

“The remote server returned an error: (400) Bad Request”

## Cause

This error occurs when you try to import, via the API, a custom field from a project that does not have a custom form associated with a Queue Topic.&nbsp;&nbsp;

## Solution

Add the correct custom form to the Queue Topic.

To learn more about Queue Topics, see [Create Queue Topics](../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md).
