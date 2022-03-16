---
filename: flow-control
content-type: reference
product: workfront-fusion
product-area: workfront-integrations
navigation-topic: apps-and-their-modules
title: Flow control
description: When you are creating or editing a scenario, you can configure settings to control the way data flows through it.
---

# Flow control

When you are creating or editing a scenario, you can configure settings to control the way data flows through it.

## Access requirements

You must have the following access to use the functionality in this article:

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Pro or higher</p> </td> 
  </tr> Adobe Workfront license* Plan, Work 
  <tr> 
   <td role="rowheader">Adobe Workfront Fusion license**</td> 
   <td> <p>Workfront Fusion for Work Automation and Integration </p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>Your organization must purchase Adobe Workfront Fusion as well as Adobe Workfront to use functionality described in this article.</td> 
  </tr> <!--
   Access level configurations* You must be a Workfront Fusion administrator for your organization. You must be a Workfront Fusion administrator for your team.
  --> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your Workfront administrator.

&#42;&#42;For information on Adobe Workfront Fusion licenses, see [Adobe Workfront Fusion licenses](../../workfront-fusion/get-started/license-automation-vs-integration.md)

## Repeater

You can use a Repeater module to repeat a task a given number of times. A Repeater module generates bundles, one after another.

For example, you could use a Repeater module to send five emails with the subjects "Hello 1," "Hello 2," and so on, by connecting the `Email > Send me an email` module to the Repeater module.

To use a Repeater module:

1. Click the Flow Control icon ![](assets/flow-control-icon.gif) at the bottom of the screen, then click `Repeater` in the menu that displays.
1. Click the Repeater bundle, then click `Connect automatically` in the box that displays.
1. In the Flow Control box that appears, type the number of repetitions (outputted bundles) you want in the `Repeats` box.

   In our email example, you would type 5.

   ![](assets/repeater-2-350x207.png)

   The value of the item increases in each repetition by this value specified in the `Step` field, which you can view by selecting `Show advanced settings`. This number is 1 by default.

1. Click `OK` to close the `Flow Control` box.

1. Click the app or service module connected to the Repeater module.
1. In the box that appears, type the information that you want to repeat.

   In our email example, you would type Hello in the Subject box, then map 

   ```
   i
   ```

   from the repeater module.

   ![](assets/repeater-3-350x207.png)

| Initial value |Enter or map the number that you want the module to set as 

```
i
```

in the first iteration. The default value is 1. |
|---|---|
| Repeats |Enter or map the number of times that you want the module to repeat. This number must be greater than or equal to 0, and less than or equal to 10,000. |
| Step |This is the number by which the module increases the value of 

```
i
```

. The default value is 1. |

>[!NOTE]
>
>The number of repeats is not determined by the value of >
>```>
>i
>```>
>, as it would be in a loop in programming. The module will repeat the number of times indicated in the Repeats field. The value >
>```>
>i
>```>
>changes with each iteration of the repeater module, and can be mapped to later modules. The example above maps the value of >
>```>
>i
>```>
>into the Hello message, resulting in messages that read "Hello 1," Hello 2," and so on.

## Iterator

An Iterator is a special type of module that converts an array into a series of bundles. Each array item will be a separate bundle in the Iterator module output. For more information, see [Iterator module](../../workfront-fusion/modules/iterator-module.md).

## Array aggregator

An array aggregator is a special type of module which allows to merge several bundles into one single bundle. For more information, see [Aggregator module](../../workfront-fusion/modules/aggregator-module.md).

## Router

The Router module allows you to branch your flow into several routes and process the data within each route differently. Once a Router module receives a bundle, it forwards it to each connected route in the order the routes were attached to the Router module. For more information, see [Router module](../../workfront-fusion/modules/router-module.md).

<!--
Directives The error handling directives allow you to control how your scenario reacts to errors. For more information, see Advanced error handling and Directives for error handling.
-->

