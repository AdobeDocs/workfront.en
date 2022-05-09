---
filename: general-functions
content-type: reference
product: workfront-fusion
product-area: workfront-integrations
navigation-topic: functions
title: General functions in Adobe Workfront Fusion
description: You must have the following access to use the functionality in this article - EDIT ME.
---

# General functions in Adobe Workfront Fusion

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

## get (object or array; path)

Returns the value path of an object or array. To access nested objects, use dot notation. The first item in an array is index 1.

``` ```**Examples: **``````

* ```get(``` ```array``` ```;```

  ```
  1
  ```

  ```+```

  ```
  1
  ```

  ```)``` 

* ```get(``` ```array``` ```;```

  ```
  5.raw_name
  ```

  ```)``` 

* ```get(``` ```object``` ```;```

  ```
  raw_name
  ```

  ```)``` 

* ```get(``` ```object``` ```;```

  ```
  raw_name.sub_raw_name
  ```

  ```)```

## if (expression; value1; value2)

Returns the value 1 if the expression is evaluated to true; otherwise it returns the value 2.

``` ```**Examples: **``````

* ```if(```

  ```
  1
  ```

  ```=```

  ```
  1
  ```

  ```;```

  ```
  A
  ```

  ```;```

  ```
  B
  ```

  ```)```

  Returns A

* ```if(``` ```=```

  ```
  2
  ```

  ```;```

  ```
  A
  ```

  ```;```

  ```
  B
  ```

  ```)```

  Returns B

## ifempty (value1; value2)

Returns the value 1 if this value is not empty; otherwise it returns the value 2.

``` ```**Examples: **``````

* ```ifempty(```

  ```
  A
  ```

  ```;```

  ```
  B
  ```

  )

  Returns A

* ```ifempty(```

  ```
  unknown
  ```

  ```;```

  ```
  B
  ```

  )

  Returns B

* ```ifempty(```

  ```
  ""
  ```

  ```;```

  ```
  B
  ```

  )

  Returns B

## switch (expression; value1; result1; [value2; result2; ...]; [else])

Evaluates one value (called the expression) against a list of values; returns the result corresponding to the first matching value.

``` ```**Examples: **``````

* ```switch(```

  ```
  B
  ```

  ```;```

  ```
  A
  ```

  ```;```

  ```
  1
  ```

  ```;```

  ```
  B
  ```

  ```;```

  ```
  2
  ```

  ```;```

  ```
  C
  ```

  ```;```

  ```
  3
  ```

  ```)```

  Returns 2

* ```switch(```

  ```
  C
  ```

  ```;```

  ```
  A
  ```

  ```;```

  ```
  1
  ```

  ;

  ```
  B
  ```

  ```;```

  ```
  2
  ```

  ```;```

  ```
  C
  ```

  ```;```

  ```
  3
  ```

  ```)```

  Returns 3

* ```switch(```

  ```
  X<span class="function">;</span>A<span class="function">;</span>1<span class="function">;</span>B<span class="function">;</span>2<span class="function">;</span>C<span class="function">;</span>3<span class="function">;</span>4
  ```

  ```)```

  Returns 4

## omit(object; key1; [key2; ...])

Omits the given keys of the object and returns the rest.

**Example:** ```omit(``` ```User``` ```;```password ```)```

Returns a collection of the user's information, excluding the password.

## pick(object; key1; [key2; ...])

Picks only the given keys from the object.

**Example:** ```pick(``` ```User``` ```;```password ```;```email ```)```

Returns a collection of only the user's password and email address.
&nbsp;
