---
filename: array-functions
content-type: reference
product: workfront-fusion
product-area: workfront-integrations
navigation-topic: functions
---



# Array functions {#array-functions}



## Access requirements {#access-requirements}

You must have the following access to use the functionality in this article:

<table style="width: 100%;margin-left: 0;margin-right: auto;mc-table-style: url('../../Resources/TableStyles/TableStyle-List-options-in-steps.css');" class="TableStyle-TableStyle-List-options-in-steps" cellspacing="0"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2"> 
 <tbody> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader"><span class="mc-variable WFVariables.FullProdNameWF variable varname">Adobe Workfront</span> plan*</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p><span class="mc-variable WFVariables.WFPlan-Pro variable varname">Pro</span> or higher</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader"><span class="mc-variable WFVariables.FullProdNameWFF variable varname">Adobe Workfront Fusion</span> license**</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray"> <p><span class="mc-variable WFVariables.WFFusionIntegration variable varname">Workfront Fusion for Work Automation and Integration</span> </p> <p data-mc-conditions="SnippetConditions.HIDE"><span class="mc-variable WFVariables.WFFusionAutomation variable varname">Workfront Fusion for Work Automation</span> </p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-LightGray" role="rowheader">Product</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-LightGray">Your organization must purchase <span class="mc-variable WFVariables.FullProdNameWFF variable varname">Adobe Workfront Fusion</span> as well as <span class="mc-variable WFVariables.FullProdNameWF variable varname">Adobe Workfront</span> to use functionality described in this article.</td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your *`Workfront administrator`*.


## add (array; value1; value2; ...) {#add-array-value-value}

Adds values specified in parameters to an array and returns that array.


## contains (array; value) {#contains-array-value}

Verifies if an array contains the value.


## distinct (array; [key]) {#distinct-array-key}

Removes duplicates inside an array. Use the "key" argument to access properties inside complex objects. To access nested properties, use dot notation. The first item in an array is index 1.

` `**Example: **`` `distinct(` `Contacts[]` `;`

```
name
```

`)` Removes duplicates inside an array of contacts by comparing the "name" property


## flatten (array) {#flatten-array}

Creates a new array with all sub-array elements concatenated into it, recursively, up to the specified depth.


More details about the flatten function can be found in the Array.prototype.flat documentation.


## join (array; separator) {#join-array-separator}

Concatenates all of the items of an array into a string, using the specified separator between each item.


## keys (object) {#keys-object}

Returns an array of the properties of a given object or array.


## length (array) {#length-array}

Returns the number of items in an array.


## map (complex array; key;[key for filtering];[possible values for filtering]) {#map-complex-array-key-key-for-filtering-possible-values-for-filtering}

Returns a primitive array containing values of a complex array. This function allows filtering values. Use raw variable names for keys.

` `**Examples: **`` 


*  `map(` `Emails[]` `;`

  ```
  email
  ```

  `)` 


  Returns a primitive array with emails

*  `map(` `Emails[]` `;`

  ```
  email
  ```

  `;`

  ```
  label
  ```

  `;`

  ```
  work
  ```

  `;`

  ```
  home
  ```

  `)` 


  Returns a primitive array with `emails`having a label equal to work or home



For more information, see [Map information from one module to another](map-information-between-modules.md).


## merge (array1; array2; ...) {#merge-array-array}

Merges one or more arrays into one array.


## remove (array; value1; value2; ...) {#remove-array-value-value}

Removes values specified in the parameters of an array. This function is effective only on primitive arrays of text or numbers.


## reverse (array) {#reverse-array}

The first element of the array becomes the last element. The reverse is also true.


## slice (array; start; [end]) {#slice-array-start-end}

Returns a new array containing only selected items.


## sort (array; [order]; [key]) {#sort-array-order-key}

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

` `**Examples: **`` 


*  `sort(` `Contacts[]` `;`

  ```
  name
  ```

  `)` 


  Sorts an array of contacts by the "name" property in default ascending order

*  `sort(` `Contacts[]` `;`

  ```
  desc
  ```

  `;`

  ```
  name
  ```

  `)` 


  Sorts an array of contacts by the "name" property in descending order

*  `sort(` `Contacts[]` `;`

  ```
  asc ci
  ```

  `;`

  ```
  name
  ```

  <![CDATA[ ]]>


  Sorts an array of contacts by the "name" property in case-insensitive ascending order

*  `sort(` `Emails[]` `;`

  ```
  sender.name
  ```

  `)` 


  Sorts an array of emails by the "sender.name" property






## arrayDifference [array1, array2, mode] {#arraydifference-array-array-mode}

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




` `**Examples: **`` Given the following arrays:




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





