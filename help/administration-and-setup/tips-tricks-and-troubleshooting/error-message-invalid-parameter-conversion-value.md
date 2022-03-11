---
filename: error-message-invalid-parameter-conversion-value
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: Error message: Invalid Parameter: conversion value
description: You receive the following error message when attempting to change the Format of a Custom Field on an existing Custom Form: "Invalid Parameter: conversion value "<...>""
---

# Error message: Invalid Parameter: conversion value

## Problem

You receive the following error message when attempting to change the Format of a Custom Field on an existing Custom Form: "Invalid Parameter: conversion value "<...>""  
![custom_field_format_invalid_parameter_error.png](assets/custom-field-format-invalid-parameter-error-350x148.png)

## Cause

This message occurs in the following scenario:

For example, you have a Custom Field formatted as Text.  Now, you want to change the Format of the Custom Field to Currency. Somewhere in your `Adobe Workfront` instance, this field is already attached to an object and it has information already specified in it. The existing information in at least one such field is already formatted as Text. Therefore, the Format of the field cannot be changed to Currency.

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p><a href="https://www.workfront.com/plans" target="_blank">Workfront plan</a>*</p> </td> 
   <td>Any</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p><a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront licenses overview</a>*</p> </td> 
   <td> <p><span>Plan</span> </p> </td> 
  </tr> Access level* Edit access to: Create Reports, Dashboards, and Calendars Create Filters, Views, and Groupings Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see Create or modify custom access levels. 
 </tbody> 
</table>

## Solution

Do the following:

1. Build reports for all the objects that might have this field associated with their Custom Forms.  
   For information about building a report, see [Create a custom report](../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

1. Include the Custom Field you are trying to edit in the view of the report, so you can see which object has this field populated with a text value.&nbsp;
1. Correct the Custom Field values of the objects that display in a text format and give them a value formatted as Currency; then attempt to change the Format field on the Custom Form again.  
   Or  
   If you have too many field values already populated with text-formatted information, consider adding a new Custom Field to your Custom Form and format it as Currency.&nbsp;&nbsp;

