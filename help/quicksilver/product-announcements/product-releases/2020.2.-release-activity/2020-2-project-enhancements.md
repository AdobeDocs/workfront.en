---
content-type: release-notes
navigation-topic: 2020-2-release-activity
title: 2020.2 Project enhancements
description: This page describes all Project enhancements made with the 2020.2 release to the Production environment. These enhancements were made available in the Production environment the week of May 11, 2020.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 150bc838-d6a5-445a-af77-62c4ed74dd1b
---
# 2020.2 Project enhancements

This page describes all Project enhancements made with the 2020.2 release to the Production environment. These enhancements were made available in the Production environment the week of May 11, 2020.

For a list of all changes available with the 2020.2 release, see [2020.2 release overview](../../../product-announcements/product-releases/2020.2.-release-activity/2020-2-release-overview.md).

## For Workfront administrators: New failsafe when the project status for new projects is hidden or unlocked

In Setup, you configure a preference to ensure that every new project has a certain status when the project is created. This is important because a project always needs a status in order to function properly in Workfront, even when the project is brand-new.

To make sure that new projects always have a status, even if an administrator hides or unlocks the status configured for new projects, the system now assigns the first status in the Status list to all new projects until you configure the new status for new projects once again.

For information about setting the preference for the status of all new projects, see [Configure system-wide project preferences](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md) (or if you are using Adobe Workfront Classic, see [Setting Project Preferences](https://experienceleague.adobe.com/en/docs/workfront/using/home)).

**Available in these environments:**

* Adobe Workfront Classic 
* The new Adobe Workfront experience

## For Workfront administrators: Improved design in Project Preferences

The experience of setting project preferences is now more intuitive and easy to use:

* Titles are larger than option labels so you can find what you're looking for faster.
* Dividing lines and extra white space separate each section so you can focus more easily on what you're doing.
* If you type an invalid number for an option such as "Typical hours per work day," a warning message appears immediately instead of appearing after you click Save.
* Option labels match corresponding interface text elsewhere in Workfront, such as the Details area and reports.

For information about the Project Preferences area, see [Configure system-wide project preferences](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md) (or if you are using Adobe Workfront Classic, see [Setting Project Preferences](https://experienceleague.adobe.com/en/docs/workfront/using/home)).

**Available in these environments:**

* Adobe Workfront Classic 
* The new Adobe Workfront experience

## Selected Filter, View, and Grouping retained in Report lists

Now, the last Filter, View, or Grouping applied to a specific report is selected, even if the user logs out and back in to Workfront.

Previously, after a user applied a Filter, View, or Grouping to a Report list and then navigated away from that page, the default Filter, View, or Grouping appeared the next time the user navigated to that same report. 

**Available in these environments:**

* The new Adobe Workfront experience 
* Adobe Workfront Classic

## Moving and copying tasks to another project keeps the task constraint when tasks can fit within the project's timeline

We have made an improvement to the way Workfront handles the date-specific Task Constraint of a task when you copy the task or move it to another project. Examples of date-specific Task Constraints are Must Start on, Must Finish On, Fixed Dates, Start No Later Than, and so forth.

For example, when you move or copy a task with a Must Start On constraint to another project whose Planned Start Date is prior to the Start Date of the task, the task keeps the constraint after it is copied or moved. When you move or copy a task with a Must Start On constraint to a project whose Planned Start Date is after the Start Date of the task, the Task Constraint changes to As Soon As Possible.

Prior to this change, the Task Constraint always changes to As Soon As Possible.

For information about moving tasks see, [Move tasks](../../../manage-work/tasks/manage-tasks/move-tasks.md) (or if you are using Adobe Workfront Classic, see [Moving Tasks](https://experienceleague.adobe.com/en/docs/workfront/using/home)).

For information about copying tasks, see [Copy and duplicate tasks](../../../manage-work/tasks/manage-tasks/copy-and-duplicate-tasks.md) (or if you are using Adobe Workfront Classic, see [Copy and Duplicate Tasks](https://experienceleague.adobe.com/en/docs/workfront/using/home)).

For an overview of all Task Constraints, see [Task Constraint overview](../../../manage-work/tasks/task-constraints/task-constraint-overview.md) (or if you are using Adobe Workfront Classic, see [Task Constraint Overview](https://experienceleague.adobe.com/en/docs/workfront/using/home)).

**Available in these environments:**

* Adobe Workfront Classic 
* The new Adobe Workfront experience

## Preventing data loss while making changes in the Details tab or a task list

To prevent data loss when you are updating information on the Details page on an object or tasks in a task list at the project level when saving changes manually, a warning message now displays, to notify you that you have unsaved changes before you attempt to edit information in the header. The only actions allowed before you save your changes are subscribing or adding the object to your favorites.

For information about editing tasks in a list, see [Edit tasks in a list](../../../manage-work/tasks/manage-tasks/edit-tasks-in-a-list.md)

**Available in these environments:**

* The new Adobe Workfront experience

