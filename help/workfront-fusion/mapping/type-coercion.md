---
filename: type-coercion
content-type: reference
product: workfront-fusion
product-area: workfront-integrations
navigation-topic: mapping
title: Type coercion
description: You must have the following access to use the functionality in this article:
---

# Type coercion

## Access requirements

You must have the following access to use the functionality in this article:

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><span>Adobe Workfront</span> plan*</td> 
   <td> <p><span>Pro</span> or higher</p> </td> 
  </tr> Adobe Workfront license* Plan, Work 
  <tr> 
   <td role="rowheader"><span>Adobe Workfront Fusion</span> license**</td> 
   <td> <p><span>Workfront Fusion for Work Automation and Integration</span> </p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>Your organization must purchase <span>Adobe Workfront Fusion</span> as well as <span>Adobe Workfront</span> to use functionality described in this article.</td> 
  </tr> <!--
   Access level configurations* You must be a Workfront Fusion administrator for your organization. You must be a Workfront Fusion administrator for your team.
  --> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your `Workfront administrator`.

&#42;&#42;For information on `Adobe Workfront Fusion` licenses, see [Adobe Workfront Fusion licenses](../../workfront-fusion/get-started/license-automation-vs-integration.md)

### Type coercion

This document describes how `Adobe Workfront Fusion` behaves in situations when it receives values in expected and unexpected data formats.

<table cellspacing="15"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Expected</th> 
   <th>Received</th> 
   <th> <p>Description</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>array </td> 
   <td>array </td> 
   <td> <p>The value is handed over unchanged.</p> </td> 
  </tr> 
  <tr> 
   <td>array </td> 
   <td>other </td> 
   <td> <p>If the received value is not of the array type, <span>Workfront Fusion</span> will create an array and the first (and the only) element will be the received value.</p> </td> 
  </tr> 
  <tr> 
   <td>boolean </td> 
   <td>boolean </td> 
   <td> <p>The value is handed over unchanged.</p> </td> 
  </tr> 
  <tr> 
   <td>boolean </td> 
   <td>number </td> 
   <td> <p>The value is converted to logical Yes, even if the value is 0.</p> </td> 
  </tr> 
  <tr> 
   <td>boolean </td> 
   <td>text </td> 
   <td> <p>If the value is equal to false or the value is empty, it is converted to logical No. If not, it is converted to logical Yes.</p> </td> 
  </tr> 
  <tr> 
   <td>boolean </td> 
   <td>other </td> 
   <td> <p>The value is converted to logical Yes whenever the received value exists (is not null).</p> </td> 
  </tr> 
  <tr> 
   <td>buffer </td> 
   <td>buffer </td> 
   <td> <p>The value is handed over unchanged only if the codepage is as expected. If the codepage differs, <span>Workfront Fusion</span> will try to convert the received value to the requested codepage. If this conversion is not supported, <span>Workfront Fusion</span> will return a validation error.</p> </td> 
  </tr> 
  <tr> 
   <td>buffer </td> 
   <td>boolean </td> 
   <td> <p>The value is converted to text (true/false) and then to binary data following the steps mentioned above for converting to text.</p> </td> 
  </tr> 
  <tr> 
   <td>buffer </td> 
   <td>date </td> 
   <td> <p>The value is converted to ISO 8601 text and then to binary data following the steps mentioned for converting to text.</p> </td> 
  </tr> 
  <tr> 
   <td>buffer </td> 
   <td>number </td> 
   <td> <p>The value is converted to text and then to binary data following the steps mentioned above for converting to text.</p> </td> 
  </tr> 
  <tr> 
   <td>buffer </td> 
   <td>text </td> 
   <td> <p>The value is converted to binary data and encoded as expected. If the expected encoding is not specified, utf8 encoding will be used.</p> </td> 
  </tr> 
  <tr> 
   <td>buffer </td> 
   <td>other </td> 
   <td> <p><span>Workfront Fusion</span> returns a validation error.</p> </td> 
  </tr> 
  <tr> 
   <td>collection </td> 
   <td>collection </td> 
   <td> <p>The value is handed over unchanged.</p> </td> 
  </tr> 
  <tr> 
   <td>collection </td> 
   <td>other </td> 
   <td> <p><span>Workfront Fusion</span> returns a validation error.</p> </td> 
  </tr> 
  <tr> 
   <td>date </td> 
   <td>date </td> 
   <td> <p>The value is handed over unchanged.</p> </td> 
  </tr> 
  <tr> 
   <td>date </td> 
   <td>text </td> 
   <td> <p><span>Workfront Fusion</span> will try to convert the text to a date. If the conversion fails, it will return a validation error. Date must contain day, month and year. Date may contain time and time zone. Default time zone is based on your settings. Examples:</p> <p><code>2016-06-20T17:26:44.356Z</code> </p> <p><code>2016-06-20 19:26:44 GMT+02:00</code> </p> <p><code>2016-06-20 19:26+0200</code> </p> <p><code>2016-06-20 17:26:44</code> </p> <p><code>2016-06-20</code> </p> <p><code>2016/06/20 17:26:44</code> </p> <p><code>2016/06/20 19:26:44+02:00</code> </p> <p><code>2016/06/20 17:26</code> </p> <p><code>2016/06/20 5:26 PM</code> </p> <p><code>2016/06/20</code> </p> <p><code>06/20/2016 17:26:44</code> </p> <p><code>06/20/2016 19:26:44+02:00</code> </p> <p><code>06/20/2016 17:26</code> </p> <p><code>06/20/2016 5:26 PM</code> </p> <p><code>06/20/2016</code> </p> <p><code>20.6.2016 17:26:44</code> </p> <p><code>20.6.2016 19:26:44+02:00</code> </p> <p><code>20.6.2016 17:26</code> </p> <p><code>20.6.2016</code> </p> </td> 
  </tr> 
  <tr> 
   <td>date </td> 
   <td>other </td> 
   <td> <p><span>Workfront Fusion</span> returns a validation error.</p> </td> 
  </tr> 
  <tr> 
   <td>number </td> 
   <td>number </td> 
   <td> <p>The value is handed over unchanged.</p> </td> 
  </tr> 
  <tr> 
   <td>number </td> 
   <td>text </td> 
   <td> <p><span>Workfront Fusion</span> will try to convert the text to a number. If the conversion fails, it will return a validation error.</p> </td> 
  </tr> 
  <tr> 
   <td>number </td> 
   <td>other </td> 
   <td> <p><span>Workfront Fusion</span> returns a validation error.</p> </td> 
  </tr> 
  <tr> 
   <td>text </td> 
   <td>text </td> 
   <td> <p>The value is handed over unchanged.</p> </td> 
  </tr> 
  <tr> 
   <td>text </td> 
   <td>array </td> 
   <td> <p>If the given array supports conversion to text, the value will be converted. If not, <span>Workfront Fusion</span> will return a validation error.</p> </td> 
  </tr> 
  <tr> 
   <td>text </td> 
   <td>boolean </td> 
   <td> <p>The value is converted to text (true/false).</p> </td> 
  </tr> 
  <tr> 
   <td>text </td> 
   <td>buffer </td> 
   <td> <p>If text encoding is specified for binary data, the value will be converted to text. If not, <span>Workfront Fusion</span> will return a validation error.</p> </td> 
  </tr> 
  <tr> 
   <td>text </td> 
   <td>date </td> 
   <td> <p>The value is converted to ISO 8601 text.</p> </td> 
  </tr> 
  <tr> 
   <td>text </td> 
   <td>number </td> 
   <td> <p>The value is converted to text.</p> </td> 
  </tr> 
  <tr> 
   <td>text </td> 
   <td>other </td> 
   <td> <p><span>Workfront Fusion</span> returns a validation error.</p> </td> 
  </tr> 
  <tr> 
   <td>time </td> 
   <td>time </td> 
   <td> <p>The value is handed over unchanged.</p> </td> 
  </tr> 
  <tr> 
   <td>time </td> 
   <td>text </td> 
   <td> <p><span>Workfront Fusion</span> will try to convert time to the hours:minutes:seconds format. If the conversion fails, it will return a validation error.</p> </td> 
  </tr> 
  <tr> 
   <td>time </td> 
   <td>other </td> 
   <td> <p><span>Workfront Fusion</span> returns a validation error.</p> </td> 
  </tr> 
 </tbody> 
</table>

