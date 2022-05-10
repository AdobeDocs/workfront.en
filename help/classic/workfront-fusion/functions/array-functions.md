---
filename: array-functions
content-type: reference
product: workfront-fusion
product-area: workfront-integrations
navigation-topic: functions
title: Array functions in Adobe Workfront Fusion
description: You must have the following access to use the functionality in this article - EDIT ME.
---

# Array functions in Adobe Workfront Fusion

>[!IMPORTANT]
>
>You're currently viewing the Adobe Workfront Classic version of this document. Adobe Workfront Classic is no longer supported. All Adobe Workfront Classic functionality, along with this documentation, will be removed in July 2022. Please transition to the the new Adobe Workfront experienceas soon as possible, and switch to the new Adobe Workfront experience version of this document.

## Access requirements

You must have the following access to use the functionality in this article:

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Pro or higher</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Plan, Work</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront Fusion license**</td> 
   <td> <p>Workfront Fusion for Work Automation and Integration </p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>Your organization must purchase Adobe Workfront Fusion as well as Adobe Workfront to use functionality described in this article.</td> 
  </tr> <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td role="rowheader">Access level configurations*</td> 
    <td> <!--
      <p data-mc-conditions="QuicksilverOrClassic.Draft mode">You must be a Workfront Fusion administrator for your organization.</p>
     --> <!--
      <p data-mc-conditions="QuicksilverOrClassic.Draft mode">You must be a Workfront Fusion administrator for your team.</p>
     --> </td> 
   </tr>
  --> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your Workfront administrator.

&#42;&#42;For information on Adobe Workfront Fusion licenses, see [Adobe Workfront Fusion licenses](../../workfront-fusion/get-started/license-automation-vs-integration.md)

## add (array; value1; value2; ...)

Adds values specified in parameters to an array and returns that array.

## contains (array; value)

Verifies if an array contains the value.

## distinct (array; [key])

Removes duplicates inside an array. Use the "key" argument to access properties inside complex objects. To access nested properties, use dot notation. The first item in an array is index 1.

**Example:** ```distinct(``` ```Contacts[]``` ```;```

```
name
```

```)``` Removes duplicates inside an array of contacts by comparing the "name" property

## flatten (array)

Creates a new array with all sub-array elements concatenated into it, recursively, up to the specified depth.

More details about the flatten function can be found in the Array.prototype.flat documentation.

## join (array; separator)

Concatenates all of the items of an array into a string, using the specified separator between each item.

## keys (object)

Returns an array of the properties of a given object or array.

## length (array)

Returns the number of items in an array.

## map (complex array; key;[key for filtering];[possible values for filtering])

Returns a primitive array containing values of a complex array. This function allows filtering values. Use raw variable names for keys.

``` ```**Examples: **``````

* ```map(``` ```Emails[]``` ```;```

  ```
  email
  ```

  ```)```

  Returns a primitive array with emails

* ```map(``` ```Emails[]``` ```;```

  ```
  email
  ```

  ```;```

  ```
  label
  ```

  ```;```

  ```
  work
  ```

  ```;```

  ```
  home
  ```

  ```)```

  Returns a primitive array with ```emails``` having a label equal to work or home

For more information, see [Map information from one module to another in Adobe Workfront Fusion](../../workfront-fusion/mapping/map-information-between-modules.md)

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
and our Extract an item and/or its value from an array of collections video tutorial
</MadCap:conditionalText>
-->

.

## merge (array1; array2; ...)

Merges one or more arrays into one array.

## remove (array; value1; value2; ...)

Removes values specified in the parameters of an array. This function is effective only on primitive arrays of text or numbers.

## reverse (array)

The first element of the array becomes the last element. The reverse is also true.

## slice (array; start; [end])

Returns a new array containing only selected items.

## sort (array; [order]; [key])

Sorts values of an array. The valid values of the 

```
order
```

parameter are:

* 

  ```
  asc
  ```

  (default) - ascending order: 1, 2, 3, ... for type Number. A, B, C, a, b, c, ... for type Text

* 

  ```
  desc
  ```

  descending order: ..., 3, 2, 1 for type Number. ..., c, b, a, C, B, A for type Text.

* 

  ```
  asc ci
  ```

  case insensitive ascending order: A, a, B, b, C, c, ... for type Text.

* 

  ```
  desc ci
  ```

  case insensitive descending order: ..., C, c, B, b, A, a for type Text.

Use the 

```
key
```

parameter to access properties inside complex objects.

Use raw variable names for keys.

To access nested properties, use dot notation.

The first item in an array is index 1.

``` ```**Examples: **``````

* ```sort(``` ```Contacts[]``` ```;```

  ```
  name
  ```

  ```)```

  Sorts an array of contacts by the "name" property in default ascending order

* ```sort(``` ```Contacts[]``` ```;```

  ```
  desc
  ```

  ```;```

  ```
  name
  ```

  ```)```

  Sorts an array of contacts by the "name" property in descending order

* ```sort(``` ```Contacts[]``` ```;```

  ```
  asc ci
  ```

  ```;```

  ```
  name
  ```

  

  Sorts an array of contacts by the "name" property in case-insensitive ascending order

* ```sort(``` ```Emails[]``` ```;```

  ```
  sender.name
  ```

  ```)```

  Sorts an array of emails by the "sender.name" property

## arrayDifference [array1, array2, mode]

Returns the difference between two arrays.

Enter one of the following values for the 

```
mode
```

parameter.

* 

  ```
  classic
  ```

  : Returns a new array that contains all elements of 

  ```
  array1
  ```

  that do not exist in 

  ```
  array2
  ```

  .
* 

  ```
  symmetric
  ```

  : Returns an array of elements that are not common to both arrays.

  In other words, the function returns an array that contains all of the elements of 

  ```
  array1
  ```

  that do not exist in 

  ```
  array2
  ```

  , and all of the elements of 

  ```
  array2
  ```

  that do not exist in 

  ```
  array1
  ```

  .

``` ```**Examples: **`````` Given the following arrays:

```
myArray = [1,2,3,4,5]
```

```
yourArray = [3,4,5,6,7]
```

* 

  ```
  arrayDifference [myArray, yourArray, classic]
  ```

  Returns 

  ```
  [1,2]
  ```

* 

  ```
  arrayDifference [yourArray, myArray, classic]
  ```

  Returns 

  ```
  [6,7]
  ```

* 

  ```
  arrayDifference [myArray, yourArray, symmetric]
  ```

  Returns 

  ```
  [1,2,6,7]
  ```

