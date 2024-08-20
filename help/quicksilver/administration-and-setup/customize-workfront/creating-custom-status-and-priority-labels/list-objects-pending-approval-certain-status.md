---
user-type: administrator
product-area: system-administration
navigation-topic: create-custom-status-and-priority-labels
title: List Objects with a Pending Approval Process Using a Certain Status
description: If you try to delete a status, an error message might tell you that it can't be deleted because it's being used in pending approval processes on objects in your system. If you want to find and review those objects to decide what you need to do, you can run a report that lists them.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 52dd8750-9a6f-4ac6-9779-ba4ea9b6f4e0
---
# List objects with a pending approval process using a certain status

If you try to delete a status, an error message might tell you that it can't be deleted because it's in at least one pending approval process in your system. You can run a report to list the objects where it is in an pending approval process, then decide what you need to do for each one.

## In Standard Mode

{{step1-to-reports}}

1. Click **New Report**, then select **Project Report**, **Task Report**, or **Issue Report**.
1. Open the **Filters** tab.
1. Click **Add a Filter Rule**, then do the following to set up the rule:
   1. Start typing `status`, then select **Status** when it displays.
   1. Leave **Equal** in the second field.
   1. Select the name of the status in the third field.
1. Click **Add a Filter Rule** again, then do the following to set up the rule
   1. Start typing `pending status`, then select that item when it displays under the object type where you are looking (**Project**, **Task**, or **Issue**).
   1. Leave **Equal** in the second field.
   1. Type `in` in the third field.
1. Click **Add a Filter Rule** again, then do the following to set up the rule
   1. Start typing approval process, then select **Group ID** when it displays under **Approval Process**.
   1. Select **Is Blank** in the second field.
1. Click **Save + Close** to run the report and list any objects of the type you specified with approval processes in pending state based on the status you specified (**Project**, **Task**, or **Issue**).
1. Repeat these steps to find the same information for the other two object types.


## In Text Mode

{{step1-to-reports}}

1. Click **New Report**, then select **Project Report**, **Task Report**, or **Issue Report**.
1. Open the **Filters** tab.
1. Select **Switch to Text Mode**.
1. Copy and paste the following into the editing window, replacing XXX with the 3-letter key for the status:

   `status=XXX`

   `status_Mod=in`

   `approvalProcess:groupID_Mod=isblank`

   You can view the key in the list of statuses, as shown in these articles:
   * [Access the list of system project statuses](project-statuses.md)
   * [Access the list of system task statuses](task-statuses.md)
   * [Access the list of system issue statuses](issue-statuses.md)

1. Click **Save + Close** to run the report and list any objects of the type you specified with approval processes in pending state based on the status you specified (**Project**, **Task**, or **Issue**).
1. Repeat these steps to find the same information for the other two object types.
