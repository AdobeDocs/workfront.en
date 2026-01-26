---
content-type: reference
product-area: reporting
keywords: audit,trail,custom,field
navigation-topic: calculate-custom-data-reports
title: "Calculated custom field example: display a field's edit history"
description: If users update custom fields on a regular basis and you want to capture a log of all the changes made to a field as well as a date when the changes happen, you can capture this information in a calculated custom field.
author: Jenny
feature: Reports and Dashboards
exl-id: e233ef28-c95a-42a1-b2eb-448dad5feddb
---
# Calculated custom field example: display a field's edit history

If users update custom fields on a regular basis and you want to capture a log of all the changes made to a field as well as a date when the changes happen, you can capture this information in a calculated custom field.

The following example shows you how to build the Instructions Edit History calculated field to capture all the change made to a single-line text field called Instructions.

>[!TIP]
>
>You can follow this example for all types of custom fields, not just single-line text fields.

This does this following: 

* Limits the Instructions Edit History field to the most recent 2000 characters to stay within the Workfront database limit. 
* Checks if the current value of the Instructions field matches the front of the Instructions Edit History value; it assumes it is blank and if it is not, it does the following: 

   * If they match, it leaves the Instructions Edit History as is; 
   * If they do not match, it replaces the Instructions Edit History with the latest value in the Instructions field, followed by the current date in parentheses, a vertical bar, and the previous Instructions Edit History, which preserves the previous value(s) and the date(s) when they were entered.

## Access requirements

## Access requirements

+++ Expand to view access requirements for the functionality in this article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>Adobe Workfront package</p> </td> 
   <td><p>Any</p></td> 
  </tr> 
  <tr> 
   <td> <p>Adobe Workfront license</p> </td> 
   <td>
      <p>Standard</p>
      <p>Plan</p></td>
  </tr> 
  <tr> 
   <td><p>Access level configurations</p></td> 
   <td> <p>Administrative access to Custom Forms</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Object permissions</p> </td> 
   <td> <p>Manage permissions on the custom forms</p></td> 
  </tr> 
 </tbody> 
</table>

For information, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Prerequisites

To add a calculated field that displays a field's edit history to a custom form, you must first:

* Create the custom form 
* Add the field whose history you want to capture to the custom form

## Display a field's edit history

1. Go to a custom form where you want to add the calculated field.

1. To create the single-line text custom field, for example, do the following:

   1. Click **Single line text**.
   1. Specify a **Label** for the custom field. For example, you can name it " Instructions".
   1. Click **Apply**.

1. Click **Calculated** to add a calculated custom field to the form.
1. Specify a **Label** for the calculated custom field. For example, you can name it "Instructions Edit History".

   This is the field that will capture any changes made to the first field you created ("Instructions").

1. Click **Save and Close**.
1. Click the name of the form where you have now added two fields to re-open it.
1. Click the calculated custom field **Instructions Edit History**, then copy and paste the following in the **Calculation** box:

   ```
   LEFT(IF(LEFT({DE:Instructions Edit History},LEN(IF(ISBLANK({DE:Instructions}),"-",{DE:Instructions})))={DE:Instructions},{DE:Instructions Edit History},CONCAT(IF(ISBLANK({DE:Instructions}),"-",{DE:Instructions})," (",$$NOW,") | ",{DE:Instructions Edit History})),2000)
   ```

1. (Recommended) Paste the same calculation in the **Instructions** field on the calculated field on the form. 
1. Make sure that  **Text** is selected in the **Format** field to format the calculated custom field as text.
   
   This is the default. 

1. Click **Save and Close**.

   Now, when you attach the custom form to an object and then someone changes the information in the **Instructions** field, the **Instructions Edit History** field displays the latest value, followed by the current date in parentheses, and a vertical bar. If further changes are made, they are added to this information in the same way.

   In the above calculation, you can replace *Instructions* with the exact name of your single-line text field whose history you want to track, and **Instructions Edit History** with the exact name of your calculated field.
