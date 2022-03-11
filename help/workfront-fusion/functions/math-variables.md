---
filename: math-variables
content-type: reference
product: workfront-fusion
product-area: workfront-integrations
navigation-topic: functions
title: Math variables
description: You must have the following access to use the functionality in this article:
---

# Math variables

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

## random

Returns a floating-point pseudo-random number in the range [

```
0
```

, 

```
1
```

] (inclusive of 

```
0
```

, but not 

```
1
```

).

Use the following formula to generate an integer pseudo-random number in the range [

```
min
```

, 

```
max
```

] (inclusive of both 

```
min
```

and 

```
max
```

):

![](assets/math-variable-random-350x61.png)

You can copy and paste the formula's code into a field:
<pre>{{floor(random * (1.max - 1.min + 1)) + 1.min}}</pre>