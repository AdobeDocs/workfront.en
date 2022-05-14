---
title: Assignments in a deleted object appear unexpectedly in assignee reports
description: Assignments in a deleted object appear unexpectedly in assignee reports
draft: Probably
---
# Assignments in a deleted object appear unexpectedly in assignee reports

>[!IMPORTANT]
>
>You're currently viewing the Adobe Workfront Classic version of this document. Adobe Workfront Classic is no longer supported. All Adobe Workfront Classic functionality, along with this documentation, will be removed in July 2022. Please transition to the the new Adobe Workfront experienceas soon as possible, and switch to the new Adobe Workfront experience version of this document.

## Problem

After you delete an object that has an assignment, both the object and the assignment are deleted. But the assignment might still show up in some reports.

For example, if you delete a task that was assigned to a user, the assignment to the user is also deleted. However, if you later run a task report that is filtered by assignee, with that user specified, the report still lists the deleted task if the task is still in the Recycle Bin.

## Cause

This is due to architectural limitations of the Recycle Bin. There are currently no plans on the roadmap to address this issue because of the scale of architectural redesign that would be necessary. 
