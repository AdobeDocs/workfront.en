---
title: Formula fields overview
description: In Adobe Workfront Planning, you can create formula fields that use functions and existing  fields to calculate a new custom value.
hidefromtoc: yes
hide: yes
recommendations: noDisplay, noCatalog
exl-id: 5027d611-916e-492d-9a44-841bdde11c94
---
# Formula fields overview

<!--update the metadata with real information when making this available in TOC and in the left nav - below-->

<!--this article is linked to the UI in the formula box, "Learn more..."-->

<!---
title: Formula fields overview
description: In Adobe Maestro, you can create formula fields that use functions and existing  fields to calculate a new custom value. 
hidefromtoc: yes
hide: yes
author: Alina
feature: (*******************WE NEED A NEW ONE*******************)
role: User, Administrator (************is this right???************)
recommendations: noDisplay, noCatalog
--->

<!--when we release permissions to RECORDS and we release referring lookup fields in a formula field, update considerations to say that lookup fields from linked records depends on the permissions to the record; if they have no permissions to view a linked record, they won't be able to use that records's lookup fields in a formula-->

{{planning-important-intro}}

You can create custom fields in Adobe Workfront Planning by referring to existing fields and connecting them in a Formula-type field.

Formula fields generate a new value using existing values from other fields in a record type and a function that indicates how the existing values should be calculated. 

For information, see the "Formula" section in the article [Create fields](../fields/create-fields.md). 

## Access requirements

You must have the following access to perform the steps in this article: 

<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
    <tr>
<tr>
<td>
   <p> Product</p> </td>
   <td>
   <p> Adobe Workfront</p> </td>
  </tr>  
 <td role="rowheader"><p>Adobe Workfront agreement</p></td>
   <td>
<p>Your organization must be enrolled in the early access stage for Workfront Planning </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront plan</p></td>
   <td>
<p>Any</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront license</p></td>
   <td>
   <p>Any</p> 
  </td>
  </tr>
  
  <tr>
   <td role="rowheader"><p>Access level configuration</p></td>
   <td> <p>There are no access controls for Workfornt planining</p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Permissions</p></td>
   <td> <p>Manage permissions to a workspace</a> </p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p>
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Layout template</p></td>
   <td> <p>Your Workfront or group administrator must add the Planning area in your layout template. For information, see <a href="../access/access-overview.md">Access overview</a>. </p>  
</td>
  </tr>

 </tbody>
</table>

<!-- Notes to add for the table: for the "Workfront plans" row: the above is only for closed beta; when going to GA - activate the following plans:    
<p>Current plan: Prime and Ultimate</p>
<p>Legacy plan: Enterprise</p>-->


## Considerations about formula fields

* Formula fields reference fields that belong to the same record type. You cannot reference fields from other record types when creating a formula field. <!--is this still accurate??-->
* You cannot change the Field type of a Formula field after you save it. 
* You can update the calculation of a formula field after you save it, and the results of the calculation update automatically for all the records of the same type. 
* You must add the fields you reference in formulas as they display in the Workfront Planning interface. 

## Supported formulas

Adobe Workfront Planning formula fields support all expressions from the Workfront calculated fields. For more information, see [Overview of calculated data expressions](/help/quicksilver/reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md).

In addition, we support the following expressions for Workfront Planning formula fields:

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
