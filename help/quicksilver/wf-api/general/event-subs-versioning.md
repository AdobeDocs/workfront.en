---
content-type: api
navigation-topic: general-api
title: Event Subscription Versioning
description: Event Subscription API
author: Becky
feature: Workfront API
role: Developer
---

Event Subscription Versioning

Workfront has two versions of Event Subscriptions. This article describes the differences between them, as well as the process for upgrading or downgrading your event subscription versions.

>[!IMPORTANT]
>
>The following releases will affect event subscription versioning:
>
>* **25.2 Release** (April 10, 2025): All new subscriptions created after the 25.2 release are created as Version 2.
>* **25.3 Release** (July 17, 2025): Subscriptions can no longer be downgraded to Version 1 after the 25.3 release.

## Changes between Version 1 and Version 2

The following changes have been made for Event Subscriptions Version 2


### General changes



<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p><b>Affected fields</b></p> </th> 
   <th> <p><b>Version 1 (Previous behavior)</b></p> </th> 
   <th> <p><b>Version 2 (Change)</b></p> </th> 
   <th> <p><b>Remediation action</b></p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Parameter values</p> </td> 
   <td> <p>For any object created from a template that included a custom form, a <code>CREATE</code> event was sent, then an <code>UPDATE</code> was sent with the parameter values (including calculated fields and their values).    </p> </td> 
   <td> <p>Only a <code>CREATE</code> event is sent, which contains parameter values including calculated fields.</p> </td> 
   <td> <p>If you have a filter on <code>UPDATE</code> events with parameter values (including calculated custom fields) and are expecting to receive it after an object <code>CREATE</code> event that includes parameter values, you no longer receive that <code>UPDATE</code> event. If you want to see parameter values on object creation, you must create an additional <code>CREATE</code> subscription.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Multi-Select type fields</p> </td> 
   <td> <p>For any type of event that contains a change on a multi-select type field, if the field only contained one value it would be converted to and sent as a string. Otherwise it would be sent as an array. </p><p>Examples:</p><ul><li><code>myMultiSelectField: ["oneValue"]</code> is converted and sent as <code>myMultiSelectField: "oneValue"</code>.</li><li><code>myMultiSelectField: ["first", "second"]</code> is sent as <code>myMultiSelectField: ["first", "second"]</code>.</li></ul> </td> 
   <td> <p>Regardless of how many values are in the array, it will be sent as an array. </p><p>Examples:</p><ul><li><code>myMultiSelectField: ["oneValue"]</code> is sent as <code>myMultiSelectField: ["oneValue"]</code>.</li><li><code>myMultiSelectField: ["first", "second"]</code> is sent as <code>myMultiSelectField: ["first", "second"]</code>.</li></ul> </td> 
   <td> <p>If you have a subscription with a filter on a multi-select field, and the value as a string, you must create a new subscription with the same filter that has the value as an array. </p> </td> 
  </tr> 
 </tbody> 
</table>

### Object specific changes

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <b>Object code</b> </th> 
   <th> <b>Affected fields</b> </th> 
   <th> <b>Version 1 (Previous behavior)</b></th> 
   <th> <b>Version 2 (Change)</b> </th> 
   <th> <b>Remediation action</b> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <th rowspan="1">ASSGN</th> 
   <td>
    <ul>
     <li><code>projectID</code></li>
     <li><code>taskID</code></li>
     <li><code>opTaskID</code></li>
     <li><code>customerID</code></li>
    </ul> 
   </td> 
   <td>When this object was updated, the <code>UPDATE</code> event sometimes incorrectly showed the affected fields change from <code>null</code> to <code>ID value</code>.</td> 
   <td>All <code>UPDATE</code> events show the correct value for the affected fields.</td> 
   <td>None. If you have a filter on the affected fields, you receive an <code>UPDATE</code> event only if these fields have actually changed, not if any other value has changed.
   </td> 
  </tr> 
  <tr> 
   <th rowspan="2">DOCU</th> 
   <td>
    <ul>
     <li><code>referenceObjID</code></li>
    </ul> 
   </td> 
   <td>When any parameter value was updated on this object, the <code>UPDATE</code> event incorrectly showed the affected field change from <code>null</code> to <code>object id</code>. </td> 
   <td>All <code>UPDATE</code> events show the correct value for the affected fields.</td> 
   <td>None. If you have a filter on the affected fields, you receive an <code>UPDATE</code> event only if these fields have actually changed, not if any other value has changed.
  </tr> 
  <tr> 
  <td>
    <ul>
     <li><code>groups</code></li>
    </ul> 
   </td> 
   <td>When a document was deleted, the <code>DELETE</code> event incorrectly showed the affected field as an empty array in the before state.    </td> 
   <td>The <code>DELETE</code> event correctly shows the affected field in the before state.</td> 
   <td>None. The <code>DELETE</code> event will still be sent but now show correct data for the affected field. 
</td> 
  </tr> 
  <tr> 
   <th rowspan="1">DOCV</th> 
  <td>
    <ul>
     <li><code>groups</code></li>
    </ul> 
   </td> 
   <td></td> 
   <td></td> 
   <td></td> 
  </tr> 
  <tr> 
   <th rowspan="1">ASSGN</th> 
  <td>
    <ul>
     <li><code>proofDecision</code></li>
     <li><code>proofName</code></li>
     <li><code>proofProgress</code></li>
    </ul> 
   </td> 
   <td>When this object was updated, two <code>UPDATE</code> events would be sent. The first one did not include the affected fields while the second event did.</td> 
   <td>All field updates including the affected fields are present in only one <code>UPDATE</code> event, and a second unnecessary event is not sent.     </td> 
   <td>None. If you have a filter on the affected fields, the events are delivered in the first event. 
</td> 
  </tr> 
  <tr> 
   <th rowspan="2">EXPNS</th> 
  <td>
    <ul>
     <li><code>topReferenceObjCode</code></li>
     <li><code>referenceObjectName</code></li>
    </ul> 
   </td> 
   <td>When any parameter value was updated on an Expense, the <code>UPDATE</code> event incorrectly showed topReferenceObjCode change from <code>EXPNS</code> to <code>PROJ</code>, and <code>referenceObjectName</code> change from <code>null</code> to <code>string value of project name</code>.      </td> 
   <td>All <code>UPDATE</code> events show the correct value for the affected fields.</td> 
   <td>None. If you have a filter on the affected fields, you receive an <code>UPDATE</code> event only if these fields have actually changed, not if any other value has changed.
  </tr> 
  <tr> 
  <td>
    <ul>
     <li><code>topReferenceObjCode</code></li>
     <li><code>referenceObjectName</code></li>
    </ul> 
   </td> 
   <td>When an Expense object was deleted, an <code>UPDATE</code> event was sent changing the affected fields to null before the <code>DELETE</code> event was sent.    </td> 
   <td>The extra <code>UPDATE</code> event is not  sent. The <code>DELETE</code> event has correct values for the affected fields in the before state. </td> 
   <td>If you have a filter for the affected fields on <code>UPDATE</code> events and are expecting to receive it when the object is deleted, you no longer receive that <code>UPDATE</code> event. If you wish to see these fields when the object is deleted, you must create an additional <code>DELETE</code> subscription.
</td> 
  </tr> 
  <tr> 
   <th rowspan="1">HOUR</th> 
  <td>
    <ul>
     <li><code>projectID </code></li>
     <li><code>taskID </code></li>
     <li><code>roleID</code></li>
     <li><code>timesheetID</code></li>
     <li><code>hourTypeID </code></li>
     <li><code>projectOverheadID</code></li>
     <li><code>referenceObjID</code></li>
     <li><code>referenceObjCode</code></li>
     <li><code>securityRootID</code></li>
    </ul> 
   </td> 
   <td></td> 
   <td></td> 
   <td></td> 
  </tr> 
  <tr> 
   <th rowspan="1">ASSGN</th> 
  <td>
    <ul>
     <li><code>groups</code></li>
    </ul> 
   </td> 
   <td></td> 
   <td></td> 
   <td></td> 
  </tr> 
  <tr> 
   <th rowspan="1">ASSGN</th> 
  <td>
    <ul>
     <li><code>groups</code></li>
    </ul> 
   </td> 
   <td></td> 
   <td></td> 
   <td></td> 
  </tr> 
 </tbody> 
</table>


You can upgrade version 1 event subscriptions to version 2, and temporarily downgrade version 2 event subscriptions to version 1. 



