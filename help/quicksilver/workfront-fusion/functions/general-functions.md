---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: functions
title: General functions in Adobe Workfront Fusion
description: The following general functions are available in the Adobe Workfront Fusion mapping panel.
author: Becky
feature: Workfront Fusion
exl-id: 74bfda4e-5690-4b8c-ac58-20cf261f188d
---
# General functions in [!DNL Adobe Workfront Fusion]

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

## [!UICONTROL get (object or array; path)]

Returns the value path of an object or array. To access nested objects, use dot notation. The first item in an array is index 1.

>[!INFO]
>
>**Examples:** 
>
>* `get( array ; 1 + 1 )`
>* `get( array ; 5.raw_name )`
>* `get( object ; raw_name )`
>* `get( object ; raw_name.sub_raw_name )`

## [!UICONTROL if (expression; value1; value2)]

Returns the `value1` if the expression is evaluated to true; otherwise it returns the `value2`.

To create an if statement that returns a value only if two or more expressions are evaluated to true, use the `and` keyword. 

To combine `if` statements, use the `and` and `or` operators.

![and operator](/help/quicksilver/workfront-fusion/functions/assets/and-in-if-statement.png)

>[!INFO]
>
>**Examples:** 
>
>* `if( 1 = 1 ; A ; B )`
>
>    Returns A
>
>* `if( 1 = 2 ; A ; B )`
>
>   Returns B
>
>*  `if( 1 = 2 and 1 = 2 ; A ; B )`
>
>    Returns B
>   

## [!UICONTROL ifempty (value1; value2)]

Returns the `value1` if this value is not empty; otherwise it returns the `value2`.

>[!INFO]
>
>**Examples:** 
>
>* `ifempty(` `A` `;` `B` )
>
>   Returns A
>
>* `ifempty(` `unknown` `;` `B` )
>
>   Returns B
>
>* `ifempty(` `""` `;` `B` )
>
>   Returns B

## [!UICONTROL switch (expression; value1; result1; [value2; result2; ...]; [else])]

Evaluates one value (called the expression) against a list of values; returns the result corresponding to the first matching value. To include an  `else` value, add it after the final expression or value.

>[!INFO]
>
>**Examples:** 
>
>* `switch( B ; A ; 1 ; B ; 2 ; C ; 3 )`
>
>   Returns 2
>
>* `switch( C ; A ; 1 ; B ; 2 ; C ; 3 )`
>
>   Returns 3
>
>* `switch( X ; A ; 1 ; B ; 2 ; C ; 3 ; 4 )`
>
>   Returns 4
>   
>   In this function, 4 is the value to be returned if no expressions apply (the `else` value).

## [!UICONTROL omit(object; key1; [key2; ...])]

Omits the given keys of the object and returns the rest.

>[!INFO]
>
>**Example:**
>
>`omit(` User `;` password `)`
>
>Returns a collection of the user's information, excluding the password.

## [!UICONTROL pick(object; key1; [key2; ...])]

Picks only the given keys from the object.

>[!INFO]
>
>**Example:** 
>
>`pick(` User `;` password `;` email `)`
>
>Returns a collection of only the user's password and email address.
