---
filename: error-message-a-dependency-loop-was-detected
content-type: tips-tricks-troubleshooting
product-area: projects
navigation-topic: tips-tricks-and-troubleshooting-projects
title: Error Message: A Dependency Loop Was Detected
description: (Note: **replaced this with this arrticle: /Content/Manage work/Tasks/Use Prdcssrs/dependency-loop-overview.htm)
hidefromtoc: true
---

# Error Message: A Dependency Loop Was Detected

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(Note: **replaced this with this arrticle: /Content/Manage work/Tasks/Use Prdcssrs/dependency-loop-overview.htm) </p>
-->

## Problem

You cannot create a predecessor relationship between two tasks because you get a dependency loop error.

![Screen_Shot_2018-06-25_at_10.55.51_AM.png](assets/screen-shot-2018-06-25-at-10.55.51-am-350x84.png)

## Cause

Dependency loops happen when you have two or more tasks that depend on each other to be completed.&nbsp;A dependency loop can also happen if you try to make a parent the predecessor of a child.

For example, Task 2 is a predecessor to Task 1, which means you must complete Task 2 before you can start working on Task 1.

If you try to make Task 1 a predecessor to Task 2, you get a dependency loop error because you cannot start Task 1 until Task 2 has been completed, but task 2 cannot be started until Task 1 is finished.

>[!TIP]
>
>Dependency loops can involve more than two tasks. Sometimes any number of parents of the tasks you are connecting with a predecessor relationship are the ones creating the dependency loop.

&nbsp; ![Screen_Shot_2018-06-25_at_10.59.19_AM.png](assets/screen-shot-2018-06-25-at-10.59.19-am-350x146.png)&nbsp;

## Solution

Adobe Workfront does not allow you to create a predecessor relationship between tasks if it creates a dependency loop. In order to fix the dependency loop, you must reevaluate&nbsp;the predecessor relationship between the tasks listed in the error message.

&nbsp;
