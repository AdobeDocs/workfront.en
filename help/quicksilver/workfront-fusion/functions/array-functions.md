---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: functions
title: Array functions in Adobe Workfront Fusion
description: The following array functions are available in the Adobe Workfront Fusion mapping panel.
author: Becky
feature: Workfront Fusion
exl-id: bf065d00-5d84-47e1-8169-bf9e01e2429d
---
# Array functions in Adobe Workfront Fusion

## Access requirements 

You must have the following access to use the functionality in this article: 

<table style="table-layout:auto"> 
 <col>  
 <col>  
 <tbody>  
  <tr>  
   <td role="rowheader">[!DNL Adobe Workfront] plan</td>  
   <td> <p>Any</p> </td>  
  </tr>  
  <tr data-mc-conditions="">  
   <td role="rowheader">[!DNL Adobe Workfront] license</td>  
   <td> <p>New: [!UICONTROL Standard]</p><p>Or</p><p>Current: [!UICONTROL Work] or higher</p> </td>  
  </tr>  
  <tr>  
   <td role="rowheader">[!DNL Adobe Workfront Fusion] license**</td>  
   <td> 
   <p>Current: No [!DNL Workfront Fusion] license requirement.</p> 
   <p>Or</p> 
   <p>Legacy: Any </p> 
   </td>  
  </tr>  
  <tr>  
   <td role="rowheader">Product</td>  
   <td> 
   <p>New:</p> <ul><li>[!UICONTROL Select] or [!UICONTROL Prime] [!DNL Workfront] Plan: Your organization must purchase [!DNL Adobe Workfront Fusion].</li><li>[!UICONTROL Ultimate] [!DNL Workfront] Plan: [!DNL Workfront Fusion] is included.</li></ul> 
   <p>Or</p> 
   <p>Current: Your organization must purchase [!DNL Adobe Workfront Fusion].</p> 
   </td>  
  </tr> 
 </tbody>  
</table>  

For more detail about the information in this table, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md). 

For information on [!DNL Adobe Workfront Fusion] licenses, see [[!DNL Adobe Workfront Fusion] licenses](../../workfront-fusion/get-started/license-automation-vs-integration.md). 

## Functions

* [join](#join-array-separator)
* [length](#length-array)
* [keys](#keys-object)
* [slice](#slice-array-start-end)
* [merge](#merge-array1-array2)
* [contains](#contains-array-value)
* [remove](#remove-array-value1-value2)
* [add](#add-array-value1-value2)
* [map](#map-complex-array-keykey-for-filteringpossible-values-for-filtering)
* [shuffle]
* [sort](#sort-array-order-key)
* [reverse](#reverse-array)
* [flatten](#flatten-array)
* [distinct](#distinct-array-key)
* [toCollection]
* [toArray](#toarray)
* [arrayDifference](#arraydifference-array1-array2-mode)
* [deduplicate]

### [!UICONTROL join (array; separator)]

Concatenates all of the items of an array into a string, using the specified separator between each item.

### [!UICONTROL length (array)]

Returns the number of items in an array.

### [!UICONTROL keys (object)]

Returns an array of the properties of a given object or array.

### [!UICONTROL slice (array; start; [end])]

Returns a new array containing only selected items.

### [!UICONTROL merge (array1; array2; ...)]

Merges one or more arrays into one array.

### [!UICONTROL contains (array; value)]

Verifies if an array contains the value.

### [!UICONTROL remove (array; value1; value2; ...)]

Removes values specified in the parameters of an array. This function is effective only on primitive arrays of text or numbers.

### [!UICONTROL add (array; value1; value2; ...)]

Adds values specified in parameters to an array and returns that array.

### [!UICONTROL map (complex array; key;[key for filtering];[possible values for filtering])]

Returns a primitive array containing values of a complex array. This function allows filtering values. Use raw variable names for keys.

  >[!INFO]
  >
  >**Examples:**
  >
  >* `map(Emails[];email)`
  >
  >  Returns a primitive array with emails
  >
  >* `map(Emails[];email;label;work;home)`
  >
  >  Returns a primitive array with emails having a label equal to work or home

For more information, see [Map information from one module to another in [!UICONTROL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md)

### shuffle

### [!UICONTROL sort (array; [order]; [key])]

Sorts values of an array. The valid values of the `order` parameter are:

* `asc`

    (default) - ascending order: 1, 2, 3, ... for type Number. A, B, C, a, b, c, ... for type Text

* `desc`

    descending order: ..., 3, 2, 1 for type Number. ..., c, b, a, C, B, A for type Text.

* `asc ci`

    case insensitive ascending order: A, a, B, b, C, c, ... for type Text.

* `desc ci`

    case insensitive descending order: ..., C, c, B, b, A, a for type Text.

Use the `key` parameter to access properties inside complex objects.

Use raw variable names for keys.

To access nested properties, use dot notation.

The first item in an array is index 1.

  >[!INFO]
  >
  >**Examples:**
  >
  >* `sort(Contacts[];name)`
  >
  >    Sorts an array of contacts by the "name" property in default ascending order
  >
  >* `sort(Contacts[];desc;name)`
  >
  >   Sorts an array of contacts by the "name" property in descending order
  >
  >* `sort(Contacts[];asc ci;name)`
  >
  >    Sorts an array of contacts by the "name" property in case-insensitive ascending order
  >
  >* `sort(Emails[];sender.name)`
  >
  >    Sorts an array of emails by the "sender.name" property

### [!UICONTROL reverse (array)]

The first element of the array becomes the last element, the second becomes the next-to-last, and so on.

### [!UICONTROL flatten (array)]

Creates a new array with all sub-array elements concatenated into it, recursively, up to the specified depth.

### [!UICONTROL distinct (array; [key])]

Removes duplicates inside an array. Use the "[!UICONTROL key]" argument to access properties inside complex objects. To access nested properties, use dot notation. The first item in an array is index 1.

  >[!INFO]
  >
  >**Example:** `distinct(Contacts[];name)` 
  >
  >Removes duplicates inside an array of contacts by comparing the "name" property

### toCollection

### toArray

This function converts a collection into an array of key-value pairs.

>[!INFO]
>
>**Examples:**
>
>Given the collection 
>
>`{ key1: "value1", key2: "value2:}`
>
>The function
>
>`toArray({ key1: "value1", key2: "value2:})`
>
>Returns the array of key-value pairs
>
>`[{ key1: "value1"}, { key2: "value2"}]`

### [!UICONTROL arrayDifference [array1, array2, mode]]

Returns the difference between two arrays.

Enter one of the following values for the `mode` parameter.

* `classic`: Returns a new array that contains all elements of `array1` that do not exist in `array2`.

* `symmetric`: Returns an array of elements that are not common to both arrays.

   In other words, the function returns an array that contains all of the elements of `array1` that do not exist in `array2`, and all of the elements of `array2` that do not exist in `array1`.

  >[!INFO]
  >
  >**Examples:** 
  >
  >Given the following arrays:
  >
  >```
  >myArray = [1,2,3,4,5]
  >```
  >
  >```
  >yourArray = [3,4,5,6,7]
  >```
  >
  >* `arrayDifference [myArray, yourArray, classic]`
  >
  >    Returns `[1,2]`
  >
  >* `arrayDifference [yourArray, myArray, classic]`
  >
  >    Returns `[6,7]`
  >
  >* `arrayDifference [myArray, yourArray, symmetric]`
  >
  >    Returns `[1,2,6,7]`

### deDuplicate

## Keywords

### emptyarray
