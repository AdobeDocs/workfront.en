---
filename: api-error-remote-server
content-type: api;tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-api
---



# API Error: “The remote server returned an error: (400) Bad Request” {#api-error-the-remote-server-returned-an-error-bad-request}



## Problem {#problem}

You get the following error while attempting to use the API to import a custom field&nbsp;to an issue:


“The remote server returned an error: (400) Bad Request”


## Cause {#cause}

This error occurs when you try to import, via the API, a custom field from a project that does not have a custom form associated with a Queue Topic.&nbsp;&nbsp;


## Solution {#solution}

Add the correct custom form to the Queue Topic.


To learn more about Queue Topics, see [Create Queue Topics](create-queue-topics.md).
