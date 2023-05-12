---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: functions
title: Math functions in Adobe Workfront Fusion
description: The following math functions are available in the Adobe Workfront Fusion mapping panel.
author: Becky
feature: Workfront Fusion
exl-id: 8a3c7a89-62b5-45e9-b857-8beedd0e5af4
---
# Math functions in [!DNL Adobe Workfront Fusion]

## Access requirements

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

## [!UICONTROL average ([array of values]) average(value1; [value2], ...)]

Returns the average value of the numeric values in a specific array, or the average value of numerical values entered individually.

## [!UICONTROL ceil (number)]

Returns the smallest integer greater than or equal to a specified number.

>[!INFO]
>
>**Examples:** 
>
>* `ceil(` `1.2` `)`
>
>   Returns 2
>
>* `ceil(` `4` `)`
>
>   Returns 4

## [!UICONTROL floor (number)]

Returns the largest integer less than or equal to a specified number.

>[!INFO]
>
>**Examples:** 
>
>* `floor(` `1.2` `)`
>
>   Returns 1
>
>* `floor(` `1.9` `)`
>
>   Returns 1
>
>* `floor(` `4` `)`
>
>   Returns 4

## [!UICONTROL formatNumber (number; decimalPOINTS; [decimalSeparator]; [thousandsSeparator])]

Returns a number in requested format. By default, the decimal point is a comma (,) and the thousands separator is a period (.).

>[!INFO]
>
>**Example:** 
>
>`formatNumber( 123456789 ; 3 ; , ; . )`
>
>Returns 123.456.789,000

## [!UICONTROL max ([array of values]), max(value1;value2; ...)]

Returns the largest number in a specified array or the largest number among numbers entered individually.

## [!UICONTROL min ([array of values]), min(value1; value2; ...)]

Returns the smallest number in a specified array or the smallest number among numbers entered individually.

## [!UICONTROL parseNumber (number; decimal separator)]

Parses a string with a number and returns the number. For example, parseNumber(1 756,456;,)

## [!UICONTROL round (number)]

Rounds a numeric value to the nearest integer.

>[!INFO]
>
>**Examples:** 
>
>* `round(` `1.2` `)`
>
>   Returns 1
>
>* `round(` `1.5` `)`
>
>   Returns 2
>
>* `round(` `1.7` `)`
>
>   Returns 2
> 
>* `round(` `2` `)`
>
>   Returns 2

## [!UICONTROL sum ([array of values]), sum(value1; value2; ...)]

Returns the sum of the values in a specified array or the sum of numbers entered individually.
