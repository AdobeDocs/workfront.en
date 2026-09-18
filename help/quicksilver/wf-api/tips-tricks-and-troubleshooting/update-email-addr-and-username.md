---
content-type: api;tips-tricks-troubleshooting
navigation-topic: workfront-api
title: Update to emailAddr does not update the username
description: Update to emailAddr does not update the usernam
author: Becky
feature: Workfront API
role: Developer
exl-id: 2d24d1b8-9504-484f-9cc0-d2f1abd6391a
TQID: https://experienceleague.adobe.com/dkceJuJ6WfaZTnbD6zdP6TsHR5bvkERD-EiBgVmrCck
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
# Update to emailAddr does not update the username

## Problem

Normally, `emailAddr` and `username` are the same attribute. Therefore, if you change a user's `emailAddr` attribute, the `username` attribute is automatically updated to match.

When the `username` does not match the `emailAddr`, an update to the `emailAddr` does not update the `username` automatically. This is true for both `emailAddr` changes through the user interface and through the API.

## Cause

The mismatch may be created in several ways:

* Users created before the synchronization rule existed. Very old user accounts may not have these attributes in sync.

* Users created via SSO at a time when the emailAddr in Workfront was case-sensitive. The SSO auto-provision option would run a case-sensitive check for users based on the attributes of the user from the identity provider. When an exact match did not exist, the auto-provision services would create a new user. If a user already existed, there was a potential that the username and `emailAddr` would not have the same casing.

* Users that have had the `username` attribute updated directly via the API, and their `emailAddr` was not updated. The `username` and `emailAddr` possibly do not match.

## Solution

Use the API to change the `username` attribute to be the same as the `emailAddr`. After synchronizing the attributes, any update to the `emailAddr` will also update the `username` to match (when the username field is not included in the update).
