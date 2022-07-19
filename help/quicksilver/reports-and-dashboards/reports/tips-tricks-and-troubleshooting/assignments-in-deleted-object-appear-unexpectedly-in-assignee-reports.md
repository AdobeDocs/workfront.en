---
title: Assignments in a deleted object appear unexpectedly in assignee reports
description: Assignments in a deleted object appear unexpectedly in assignee reports
author: Nolan
draft: Probably
---
# Assignments in a deleted object appear unexpectedly in assignee reports

## Problem

After you delete an object that has an assignment, both the object and the assignment are deleted. But the assignment might still show up in some reports.

For example, if you delete a task that was assigned to a user, the assignment to the user is also deleted. However, if you later run a task report that is filtered by assignee, with that user specified, the report still lists the deleted task if the task is still in the Recycle Bin.

## Cause

This is due to architectural limitations of the Recycle Bin. There are currently no plans on the roadmap to address this issue because of the scale of architectural redesign that would be necessary. 
