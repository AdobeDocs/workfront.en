---
title: Formula fields
description: In Adobe Maestro, you can create formula fields that use functions and existing  fields to calculate a new custom value. 
hidefromtoc: yes
hide: yes
recommendations: noDisplay, noCatalog
---
<!--update the metadata with real information when making this available in TOC and in the left nav - below-->

<!---
title: Formula fields
description: In Adobe Maestro, you can create formula fields that use functions and existing  fields to calculate a new custom value. 
hidefromtoc: yes
hide: yes
author: Alina
feature: (*******************WE NEED A NEW ONE*******************)
role: User, Administrator (************is this right???************)
recommendations: noDisplay, noCatalog
--->

>[!IMPORTANT]
>
>The information in this article refers to Adobe Maestro which is a new offering from Adobe Workfront. 
>
>Currently, Adobe Maestro is part of a beta program which is open to a limited number of customers. You must be a Workfront customer to use Maestro capabilities. 
>
>Contact your account representative for more information about joining the beta program for Maestro.
>
>For information, see [Adobe Maestro overview](../maestro-overview.md). 

You can create calculated fields in Adobe Maestro where the values are calculated automatically, rather than manually, by creating Formula-type fields. For information, see [Create fields](../fields/create-fields.md). 

Formula fields generate a new value using existing values from other fields in a record type and a function that indicates how the existing values should be calculated. 

## Access requirements

You must have the following access to perform the steps in this article: 

<table style="table-layout:auto">
 <col>
 <tbody>
<td>
   <p> Adobe product</p> </td>
   <td>
   <p> Adobe Workfront</p> </td>
  </tr>  
 <td role="rowheader"><p>Adobe Workfront agreement</p></td>
   <td>
<p>Your organization must be enrolled in the Adobe Maestro closed beta program. Contact your account representative to inquire about this new offering. </p>
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
   <td role="rowheader">Access level</td>
   <td> <p>Any</p>  
</td>
  </tr>
<tr>
   <td role="rowheader">Layout template</td>
   <td> <p>Your system administrator must add the Maestro area in your layout template. For information, see <a href="../access/grant-access.md">Grant access to Adobe Maestro</a>. </p>  
</td>
  </tr>
 </tbody>
</table>

<!-- Notes to add for the table: for the "Workfront plans" row: the above is only for closed beta; when going to GA - activate the following plans:    
<p>Current plan: Prime and Ultimate</p>
<p>Legacy plan: Enterprise</p>-->

## Considerations about formula fields

* Formula fields reference fields that belong to the same record type. You cannot reference fields from other record types when creating a formula field. <!--is this still accurate??-->
* You cannot change the Field type of a Formula field after you saved it. 
* You can update the calculation of a formula field after you save it, and the results of the calculation update automatically for all the records of the same type. 


<!--
## The syntax of Maestro formula fields

## Functions supported in Maestro formula fields - I think this should be its own article, but link from here. 

-->