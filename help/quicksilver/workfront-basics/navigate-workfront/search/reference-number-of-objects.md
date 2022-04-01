---
filename: reference-number-of-objects
content-type: reference
navigation-topic: search
title: Use the reference number of objects
description: In Adobe Workfront, items are identified as objects. Objects correspond with the database and are used to correlate data with an item.
---

# Use the reference number of objects

In Adobe Workfront, items are identified as objects. Objects correspond with the database and are used to correlate data with an item.

Workfront automatically assigns each of the following objects a unique reference number when the object is created:

* Projects
* Tasks
* Issues
* Documents

Reference numbers are useful in distinguishing between two otherwise similar objects (such as tasks with the same name). You can search for reference numbers and include them in reports.

>[!IMPORTANT]
>
>* Workfront assigns reference numbers continuously across all customers and all objects.&nbsp;For example, when you create a task, Workfront might assign it a reference number of 00005. If another customer creates a project next, their project might receive the next available reference number, for example 00006. If you create an issue next, your issue might receive the reference number 00007, and so forth. 
>* You cannot control the sequence of reference numbers for any objects in Workfront. The sequence is always controlled by our database. 
>

## View an object's reference number

Reference numbers are displayed by default for tasks and issues. You can also easily configure Workfront to display reference numbers for other types of objects.

* [View reference numbers for tasks and issues](#view-reference-numbers-for-tasks-and-issues) 
* [View reference numbers for other objects](#view-reference-numbers-for-other-objects) 
* [View reference numbers in reports](#view-reference-numbers-in-reports)

### View reference numbers for tasks and issues {#view-reference-numbers-for-tasks-and-issues}

Reference numbers are displayed by default when viewing a task or issue.  To see the reference number click **Task Details** or **Issue Details** in the left panel, then locate the **Basic Information** section in the Overview.

![](assets/reference-number-nwe-350x184.png)

### View reference numbers for other objects  {#view-reference-numbers-for-other-objects}

To view reference numbers for objects, you can create a custom view or modify an existing view and add the Reference Number field to a column in the view. For example, you can modify the Projects view to display the reference number for all your projects.

For information about how to create or modify a View, see [Views overview in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

### View reference numbers in reports {#view-reference-numbers-in-reports}

You can display the reference number for objects in reports by adding the Reference Number column to the report.

For information about how to add a column to a report, see [Create a custom report](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

## Search for an object by reference number

Workfront enables you to search for an object by reference number.

Type an object's reference number into the **Search** field, then press **Enter**.

For more information on searching in Workfront, see [Search Adobe Workfront](../../../workfront-basics/navigate-workfront/search/search-workfront.md).
