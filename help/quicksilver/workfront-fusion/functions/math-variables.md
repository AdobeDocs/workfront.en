---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: functions
title: Math variables in [!DNL Adobe Workfront Fusion]
description: The following math variables are available in the [!DNL Adobe Workfront Fusion mapping] panel.
author: Becky
feature: Workfront Fusion
exl-id: 2fb561d2-0780-4fd6-87b3-5360a02df177
---
# Math variables in [!DNL Adobe Workfront Fusion]

<!--Audited: 4/2024-->

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

## pi

Represents the mathematical symbol $\pi$.

## [!UICONTROL random]

Returns a floating-point pseudo-random number in the range [`0`,`1`] (inclusive of `0`, but not `1`).

Use the following formula to generate an integer pseudo-random number in the range [`min`,`max`] (inclusive of both `min` and `max`):

![](assets/math-variable-random-350x61.png)

```
floor(random * (1.max - 1.min + 1)) + 1.min
```
