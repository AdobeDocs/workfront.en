---
title: Formula Fields Overview
description: In Adobe Workfront Planning, you can create formula fields that use functions and existing  fields to calculate a new custom value.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 5027d611-916e-492d-9a44-841bdde11c94
---
# Formula fields overview

<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

{{planning-important-intro}}

You can create custom fields in Adobe Workfront Planning by referring to existing fields and connecting them in a Formula-type field.

Formula fields generate a new value using existing values from other fields in a record type and a function that indicates how the existing values should be calculated. 

For information, see the "Formula" section in the article [Create fields](/help/quicksilver/planning/fields/create-fields.md). 

## Access requirements

+++ Expand to view the access requirements for the functionality in this article. 

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
</tr>   
<tr> 
   <td role="rowheader"><p>Adobe Workfront package</p></td> 
   <td> 
<ul> 
<li><p>Any Workfront and any Planning package</p></li>
Or
<li><p>Any Workflow and any Planning packages</li></ul>
<p>For more information about what is included in each Workfront Planning package, contact your Workfront account representative. </p> 
   </td> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront license</p></td> 
   <td><p>Standard</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Object permissions</p></td> 
   <td>   <p>Manage permissions to a workspace</a> </p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p>  </td> 
  </tr>  
</tbody> 
</table> 

For more information about Workfront access requirements, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++   

<!--Old:

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
<td> 
   <p> Products</p> </td> 
   <td> 
   <ul><li><p> Adobe Workfront</p></li> 
   <li><p> Adobe Workfront Planning<p></li></ul></td> 
  </tr>   
<tr> 
   <td role="rowheader"><p>Adobe Workfront plan*</p></td> 
   <td> 
<p>Any of the following Workfront plans:</p> 
<ul><li>Select</li> 
<li>Prime</li> 
<li>Ultimate</li></ul> 
<p>Workfront Planning is not available for legacy Workfront plans</p> 
   </td> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront Planning package*</p></td> 
   <td> 
<p>Any </p> 
<p>For more information about what is included in each Workfront Planning plan, contact your Workfront account manager. </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>Adobe Workfront platform</p></td> 
   <td> 
<p>Your organization's instance of Workfront must be onboarded to the Adobe Unified Experience to be able to access Workfront Planning.</p> 
<p>For more information, see <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience for Workfront</a>. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront license*</p></td> 
   <td><p> Standard</p>
   <p>Workfront Planning is not available for legacy Workfront licenses</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Access level configuration</p></td> 
   <td> <p>There are no access level controls for Adobe Workfront Planning</p>   
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Object permissions</p></td> 
   <td>   <p>Manage permissions to a workspace and record type </a> </p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p> </td> 
  </tr> 
 
</tbody> 
</table> -->

## Considerations about formula fields

* Formula fields reference fields that belong to the same record type. 
* You can reference fields from other record types only when you connect another record type to the one you're creating a formula field for. 
* Referencing connected record types or their lookup fields in a formula depends on your permissions to the connected record types. If you have no permissions to view the record type, you cannot reference their fields in a formula. 
* You cannot change the Field type of a Formula field after you save it. 
* You can update the calculation of a formula field after you save it, and the results of the calculation update automatically for all the records of the same type. 
* You must add the fields you reference in formulas as they display in the Workfront Planning interface. 
* You can reference only fields that display in the table view of a record type or on the record details page. 
* You can define the format for the value of a formula calculation by choosing from the following format options:

   * Text
   * Number
   * Percent
   * Currency
   * Tags
   * Date

   For more information, see the "Formula" section in the article [Create fields](/help/quicksilver/planning/fields/create-fields.md).
* You can reference formula fields in new formulas. Once the value is updated in a field referenced in a formula field, all subsequent fields referencing that field or formula fields that contain that field will update automatically.

<div class="preview">

* When you update a formula field or a field that could impact it, an alert notifies you of the impact of your change. The alert displays in the following cases:   

   * When you update a formula field (excluding name and description changes) when that field has dependent formula or lookup fields. The alert lists those dependent fields and asks you whether you want to continue. 

   * When you delete a field that is used in a formula expression or as a lookup field. The alert lists the dependent formula and lookup fields and asks you whether you want to continue with the deletion.

</div>



<div class="preview">

## Limitations of formula fields

* You can add a maximum of 20 formula fields for one record type. 

   Formula lookup fields added from connected record types do not count against this limit. 

* The formula expression cannot exceed 50,000 characters. 

* Formula fields might display as `#ERROR!` in the following cases:
   * When a field used in a formula is deleted.
   * When a field used in an aggregated lookup field displays as `#ERROR!`. 
   
      For example, if you display a lookup field that contains aggregated lookup formula fields and one of the referenced formula fields  displays as `#ERROR!`. 
   *  When a formula value cannot be displayed in the selected format. 
   
      For example, if I select Number for the Format of a formula field, and the fields used in the formula are text fields that display only non-numeric text values, the formula result will display as `#ERROR!`, because it cannot parse the text into a number.
 
 </div>
 
## Supported formulas

Adobe Workfront Planning formula fields support most of the expressions from the Workfront calculated fields. 

>[!NOTE]
>
>The following Workfront expressions are not supported for Workfront Planning formula fields: 
>
><!--* SORTASCARRAY-->
><!--* SORTDESCARRAY-->
>* ADDHOUR
>* SWITCH
>* FORMAT

<!--remove the ones commented out when we go live to Preview and Prod, if they truly are added to Planning-->

For a complete list of Workfront expressions, see [Overview of calculated data expressions](/help/quicksilver/reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md).

In addition, we support the following expressions for Workfront Planning formula fields. The following expressions are not supported for Workfront expressions:

<!--take these three out when they also come to WF and Lisa has added them to the WF expression article linked above-->

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Expression</th> 
   <th>Explanation and example</th> 
  </tr> 
 </thead> 
 <tbody> 

 <tr> 
   <td><strong>ARRAYJOIN</strong> </td> 
   <td> <p>Returns concatenated string by delimiter.</p> <p>The expression is formatted as follows:
   
   <code>ARRAYJOIN(delimiter,array)</code>
   </p>
   </td></tr>
    <tr> 
   <td><strong>ARRAYUNIQUE</strong> </td> 
   <td> <p>Returns array with unique values.</p> <p>The expression is formatted as follows:

   <code>ARRAYUNIQUE(array)</code>
   </p>
   </td></tr>
     <tr> 
   <td><strong>ID</strong> </td> 
   <td> <p>Returns the ID of a record. Each record has a unique ID.</p> <p>The expression is formatted as follows:
   
   <code>{ID}</code>
   </p>
   </td></tr>
  <tr> 
   <td><strong>JSONELEMENT</strong> </td> 
   <td> <p>Returns the data from JSON by the provided JSONPath. If the JSONPath doesn't exist in the JSON, an empty result will be returned. </p> <p>The expression is formatted as follows:
      <code>JSONELEMENT(JSONString, JSONPathString) </code>
   </p>
   </td></tr>
  <tr> 
   <td><strong>SETTIMEZONE</strong> </td> 
   <td> <p>Sets the timezone of a date and time to a specific timezone.</p> <p>The expression is formatted as follows:
   
   <code>SETTIMEZONE(date,'America/Los_Angeles')</code>
   </p>
   </td></tr>
   
   <tr> 
   <td><strong>WEEKOFYEAR</strong> </td> 
   <td> <p>Returns the week number in a year. Optionally, you can indicate which day the week starts on (use 1 for Sunday, or 2 for Monday). If omitted, weeks start on Sunday, by default.</p> <p>The expression is formatted as follows:
   
   <code>WEEKOFYEAR(date,2)</code>
      or
   <code>WEEKOFYEAR(date)</code>
   </p>
   </td></tr>
   
   </table>
