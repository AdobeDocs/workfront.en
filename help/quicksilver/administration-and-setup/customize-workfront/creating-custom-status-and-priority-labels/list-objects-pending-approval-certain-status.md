---
filename: list-objects-pending-approval-certain-status
user-type: administrator
product-area: system-administration
navigation-topic: create-custom-status-and-priority-labels
title: List objects with a pending approval processes using a certain status
description: If you try to delete a status, an error message might tell you that it can't be deleted because it's being used in pending approval processes on objects in your system. If you want to find and review those objects to decide what you need to do, you can run a report that lists them.
---

# List objects with a pending approval processes using a certain status

<!-- Mini toc link to this is drafted and also needs to be added to vsc.  -->

If you try to delete a status, an error message might tell you that it can't be deleted because it's being used in pending approval processes on objects in your system. If you want to find and review those objects to decide what you need to do, you can run a report that lists them.
In Standard Mode

In Text Mode


In Standard Mode
Go to the Reporting area in the Global Navigation Bar, then select the Reports tab.
Click the Main Menu icon  in the upper-right corner, then click Reports.

Click New Report, then select Project Report, Task Report, or Issue Report.

Open the Filters tab.

Click Add a Filter Rule, then do the following to set up the rule:
Start typing status, then select Status when it displays.


Leave Equal in the second field.


Select the name of the status in the third field.



Click Add a Filter Rule again, then do the following to set up the rule
Start typing Pending Status, then select that item when it displays under the object type where you are looking (Project, Task, or Issue).

Leave Equal in the second field.


Type in in the third field.



Click Add a Filter Rule again, then do the following to set up the rule
Start typing approval process, then select Group ID when it displays under Approval Process.

Select IsBlank in the second field.




Click Save + Close to run the report and list any objects of the type you specified with approval processes in pending state based on the status you specified (Project, Task, or Issue).

Repeat these steps to find the same information for the other two object types.


In Text Mode
Go to the Reporting area in the Global Navigation Bar, then select the Reports tab.
Click the Main Menu icon  in the upper-right corner, then click Reports.

Click New Report, then select Project Report, Task Report, or Issue Report.

Open the Filters tab.

Select Switch to Text Mode.

Copy and paste the following into the editing window, replacing XXX with the 3-letter key for the status:
status=XXX
status_Mod=in
approvalProcess:groupID_Mod=isblank
You can view the key in the list of statuses, as shown in these articles:
Access the list of system project statuses

Access the list of system task statuses

Access the list of system issue statuses



Click Save + Close to run the report and list any objects of the type you specified with approval processes in pending state based on the status you specified (Project, Task, or Issue).

Repeat these steps to find the same information for the other two object types.