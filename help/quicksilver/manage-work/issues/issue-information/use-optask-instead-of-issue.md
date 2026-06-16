---
product-area: projects
navigation-topic: issue-information
title: Use "opTask" and "issue" when Referencing Issues
description: The name of an issue appears as opTask in the Adobe Workfront database. Although there are times when you need to use the issue field name to refer to issues, most of the time you must use the opTask field name instead of issue when referencing issues.
author: Alina
feature: Work Management
exl-id: 91107c04-616c-49b2-aa78-10e373d11f6b
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/jrNMdSfyMO3MgzcxxKSNtrgzuY3e4ZNJpJ-JdvylJN4
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
    internal-label: Work management
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
    internal-label: Administration
subfeature_v2:
  - id: f0dd7b45-76b5-49d4-afe3-39f436b6fbd3
    internal-label: Projects
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
    internal-label: Reporting
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
---
# Use "opTask" and "issue" when referencing issues

<!--Audited: 08/2025-->

The name of an issue appears as `opTask` in the Adobe Workfront database. Although there are times when you need to use the `issue` field name to refer to issues, most of the time you must use the `opTask` field name instead of `issue` when referencing issues.

For more information about how objects appear in the Workfront database, refer to the [API Explorer](https://developer.adobe.com/workfront/api-explorer/).

## `opTask` field name

Use the `opTask` field name when referencing issues in the following contexts:

* When you create a text mode custom report for issues, and you want to reference issues in views, filters, groupings, or prompts.  
 
  For more information about using text mode in a report, see [Text Mode overview](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md).

<!--
* When you pull information about issues using our API.  
  For more information about the Workfront API, see [Adobe Workfront API](../../../wf-api/workfront-api.md)
  -->

* When you update issue fields in a Kick-Start data importer sheet. 

  For more information about importing data in Workfront using a Kick-Start, see [Import data into Adobe Workfront using a Kick-Start template](../../../administration-and-setup/manage-workfront/using-kick-starts/import-data-via-kickstarts.md).

## `issue` field name 

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
