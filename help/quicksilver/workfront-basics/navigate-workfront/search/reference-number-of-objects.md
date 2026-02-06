---
content-type: reference
navigation-topic: search
title: Use the reference number of objects
description: In [!DNL Adobe Workfront], items are identified as objects. Objects correspond with the database and are used to correlate data with an item. Reference numbers are useful in distinguishing between two otherwise similar objects (such as tasks with the same name). You can search for reference numbers and include them in reports.
feature: Get Started with Workfront
author: Courtney
exl-id: 94f5a174-21cc-4c10-88ed-89a8014d28f4
---
# Use the reference number of objects

In [!DNL Adobe Workfront], items are identified as objects. Objects correspond with the database and are used to correlate data with an item.

Workfront automatically assigns each of the following objects a unique reference number when the object is created:

* Projects
* Tasks
* Issues
* Documents

Reference numbers are useful in distinguishing between two otherwise similar objects (such as tasks with the same name). You can search for reference numbers and include them in reports.

>[!IMPORTANT]
>
>* [!DNL Workfront] assigns reference numbers continuously across all customers and all objects. For example, when you create a task, [!DNL Workfront] might assign it a reference number of 00005. If another customer creates a project next, their project might receive the next available reference number, for example 00006. If you create an issue next, your issue might receive the reference number 00007, and so forth.
>* You cannot control the sequence of reference numbers for any objects in [!DNL Workfront]. The sequence is always controlled by our database.
>



## View an object's reference number

Reference numbers are displayed by default for tasks and issues. You can also easily configure [!DNL Workfront] to display reference numbers for other types of objects.

* [View reference numbers for tasks and issues](#view-reference-numbers-for-tasks-and-issues)
* [View reference numbers for other objects](#view-reference-numbers-for-other-objects)
* [View reference numbers in reports](#view-reference-numbers-in-reports)

### View reference numbers for tasks and issues 

Reference numbers are displayed by default when viewing a task or issue.  To see the reference number click **[!UICONTROL Task Details]** or **[!UICONTROL Issue Details]** in the left panel, then locate the **[!UICONTROL Basic Information]** section in the Overview.

![Reference number](assets/reference-number-nwe-350x184.png)

### View reference numbers for other objects  

To view reference numbers for objects, you can create a custom view or modify an existing view and add the [!UICONTROL Reference Number] field to a column in the view. For example, you can modify the [!UICONTROL Projects] view to display the reference number for all your projects.

For information about how to create or modify a View, see [Views overview in [!DNL Adobe Workfront]](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

### View reference numbers in reports 

You can display the reference number for objects in reports by adding the [!UICONTROL Reference Number] column to the report.

For information about how to add a column to a report, see [Create a custom report](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

## Search for an object by reference number

[!DNL Workfront] enables you to search for an object by reference number.

Type an object's reference number into the **[!UICONTROL Search]** field, then press **[!UICONTROL Enter]**.

For more information on searching in Workfront, see [Search [!DNL Adobe Workfront]](../../../workfront-basics/navigate-workfront/search/search-workfront.md).
