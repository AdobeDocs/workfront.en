---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: mapping
title: Type coercion in Adobe Workfront Fusion
description: This document describes how [!DNL Adobe Workfront Fusion] behaves in situations when it receives values in expected and unexpected data formats.
author: Becky
feature: Workfront Fusion
exl-id: 847a17c9-bd67-4132-81a8-2a5fe8d516cb
---
# Type coercion in [!DNL Adobe Workfront Fusion]

## Access requirements

+++ Expand to view access requirements for the functionality in this article.

You must have the following access to use the functionality in this article:

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!DNL Adobe Workfront] plan*</td> 
   <td> <p>[!DNL Pro] or higher</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] license*</td> 
   <td> <p>[!UICONTROL Plan], [!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Adobe Workfront Fusion] license**</td> 
   <td>
   <p>Current license requirement: No [!DNL Workfront Fusion] license requirement.</p>
   <p>Or</p>
   <p>Legacy license requirement: [!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>
   <p>Current product requirement: If you have the [!UICONTROL Select] or [!UICONTROL Prime] [!DNL Adobe Workfront] Plan, your organization must purchase [!DNL Adobe Workfront Fusion] as well as [!DNL Adobe Workfront] to use functionality described in this article. [!DNL Workfront Fusion] is included in the [!UICONTROL Ultimate] [!DNL Workfront] plan.</p>
   <p>Or</p>
   <p>Legacy product requirement: Your organization must purchase [!DNL Adobe Workfront Fusion] as well as [!DNL Adobe Workfront] to use functionality described in this article.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

To find out what plan, license type, or access you have, contact your [!DNL Workfront] administrator.

For information on [!DNL Adobe Workfront Fusion] licenses, see [[!DNL Adobe Workfront Fusion] licenses](../../workfront-fusion/get-started/license-automation-vs-integration.md).

+++

### Type coercion

This document describes how [!DNL Adobe Workfront Fusion] behaves in situations when it receives values in expected and unexpected data formats.

<table style="table-layout:auto">
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
   <td> <p>If the received value is not of the array type, [!DNL Workfront Fusion] will create an array and the first (and the only) element will be the received value.</p> </td> 
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
   <td> <p>The value is handed over unchanged only if the codepage is as expected. If the codepage differs, [!DNL Workfront Fusion] will try to convert the received value to the requested codepage. If this conversion is not supported, [!DNL Workfront Fusion] will return a validation error.</p> </td> 
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
   <td> <p>[!DNL Workfront Fusion] returns a validation error.</p> </td> 
  </tr> 
  <tr> 
   <td>collection </td> 
   <td>collection </td> 
   <td> <p>The value is handed over unchanged.</p> </td> 
  </tr> 
  <tr> 
   <td>collection </td> 
   <td>other </td> 
   <td> <p>[!DNL Workfront Fusion] returns a validation error.</p> </td> 
  </tr> 
  <tr> 
   <td>date </td> 
   <td>date </td> 
   <td> <p>The value is handed over unchanged.</p> </td> 
  </tr> 
  <tr> 
   <td>date </td> 
   <td>text </td> 
   <td> <p>[!DNL Workfront Fusion] will try to convert the text to a date. If the conversion fails, it will return a validation error. Date must contain day, month and year. Date may contain time and time zone. Default time zone is based on your settings. Examples:</p> <p><code>2016-06-20T17:26:44.356Z</code> </p> <p><code>2016-06-20 19:26:44 GMT+02:00</code> </p> <p><code>2016-06-20 19:26+0200</code> </p> <p><code>2016-06-20 17:26:44</code> </p> <p><code>2016-06-20</code> </p> <p><code>2016/06/20 17:26:44</code> </p> <p><code>2016/06/20 19:26:44+02:00</code> </p> <p><code>2016/06/20 17:26</code> </p> <p><code>2016/06/20 5:26 PM</code> </p> <p><code>2016/06/20</code> </p> <p><code>06/20/2016 17:26:44</code> </p> <p><code>06/20/2016 19:26:44+02:00</code> </p> <p><code>06/20/2016 17:26</code> </p> <p><code>06/20/2016 5:26 PM</code> </p> <p><code>06/20/2016</code> </p> <p><code>20.6.2016 17:26:44</code> </p> <p><code>20.6.2016 19:26:44+02:00</code> </p> <p><code>20.6.2016 17:26</code> </p> <p><code>20.6.2016</code> </p> </td> 
  </tr> 
  <tr> 
   <td>date </td> 
   <td>other </td> 
   <td> <p>[!DNL Workfront Fusion] returns a validation error.</p> </td> 
  </tr> 
  <tr> 
   <td>number </td> 
   <td>number </td> 
   <td> <p>The value is handed over unchanged.</p> </td> 
  </tr> 
  <tr> 
   <td>number </td> 
   <td>text </td> 
   <td> <p>[!DNL Workfront Fusion] will try to convert the text to a number. If the conversion fails, it will return a validation error.</p> </td> 
  </tr> 
  <tr> 
   <td>number </td> 
   <td>other </td> 
   <td> <p>[!DNL Workfront Fusion] returns a validation error.</p> </td> 
  </tr> 
  <tr> 
   <td>text </td> 
   <td>text </td> 
   <td> <p>The value is handed over unchanged.</p> </td> 
  </tr> 
  <tr> 
   <td>text </td> 
   <td>array </td> 
   <td> <p>If the given array supports conversion to text, the value will be converted. If not, [!DNL Workfront Fusion] will return a validation error.</p> </td> 
  </tr> 
  <tr> 
   <td>text </td> 
   <td>boolean </td> 
   <td> <p>The value is converted to text (true/false).</p> </td> 
  </tr> 
  <tr> 
   <td>text </td> 
   <td>buffer </td> 
   <td> <p>If text encoding is specified for binary data, the value will be converted to text. If not, [!DNL Workfront Fusion] will return a validation error.</p> </td> 
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
   <td> <p>[!DNL Workfront Fusion] returns a validation error.</p> </td> 
  </tr> 
  <tr> 
   <td>time </td> 
   <td>time </td> 
   <td> <p>The value is handed over unchanged.</p> </td> 
  </tr> 
  <tr> 
   <td>time </td> 
   <td>text </td> 
   <td> <p>[!DNL Workfront Fusion] will try to convert time to the hours:minutes:seconds format. If the conversion fails, it will return a validation error.</p> </td> 
  </tr> 
  <tr> 
   <td>time </td> 
   <td>other </td> 
   <td> <p>[!DNL Workfront Fusion] returns a validation error.</p> </td> 
  </tr> 
 </tbody> 
</table>
