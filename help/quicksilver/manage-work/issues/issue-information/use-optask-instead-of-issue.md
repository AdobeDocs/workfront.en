---
product-area: projects
navigation-topic: issue-information
title: Use "opTask" and "issue" when referencing issues
description: The name of an issue appears as opTask in the Adobe Workfront database. Although there are times when you need to use the issue field name to refer to issues, most of the time you must use the opTask field name instead of issue when referencing issues.
author: Alina
feature: Work Management
exl-id: 91107c04-616c-49b2-aa78-10e373d11f6b
---
# Use "opTask" and "issue" when referencing issues

The name of an issue appears as `opTask` in the Adobe Workfront database. Although there are times when you need to use the `issue` field name to refer to issues, most of the time you must use the `opTask` field name instead of `issue` when referencing issues.

For more information about how objects appear in the Workfront database, refer to the [API Explorer](https://developer.adobe.com/workfront/api-explorer/).

## `opTask` filename

Use the `opTask` field name when referencing issues in the following contexts:

* When you create a text mode custom report for issues, and you want to reference issues in views, filters, groupings, or prompts.  
 
  For more information about using text mode in a report, see [Text Mode overview](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md).

<!--* When you pull information about issues using our API.  
  For more information about the Workfront API, see [Adobe Workfront API](../../../wf-api/workfront-api.md)-->

* When you update issue fields in a Kick-Start data importer sheet. 

  For more information about importing data in Workfront using a Kick-Start, see [Import data into Adobe Workfront using a Kick-Start template](../../../administration-and-setup/manage-workfront/using-kick-starts/import-data-via-kickstarts.md).

## `issue` field ename 

Use the `issue` field name to reference issues in the following contexts:

* When you reference issues in a collection using text mode in a report. 
* When you reference an issue collection using the Workfront API.

For information about reporting on collections, see [Reference collections in a report](../../../reports-and-dashboards/reports/text-mode/reference-collections-report.md).

<!--
<note type="tip">
For information about how issues appear in a collection, see the
<a href="https://developer.adobe.com/workfront/api-explorer/" target="_blank">API Explorer</a> and select the API Unsupported option from the upper-right corner of the page.
<br>(NOTE: Drafted because this might not be needed.)
</note>
-->
