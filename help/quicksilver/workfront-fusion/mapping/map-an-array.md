---
filename: map-an-array
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: mapping
title: Map an array in Adobe Workfront Fusion
description: An array is a special type of item that can contain the following - EDIT ME.
---

# Map an array in Adobe Workfront Fusion

An array is a special type of item that can contain the following:

* One or more text values (simple array)
* One or more collections of the same type (complex array)

**Example:** The Watch emails module returns an array of attachments for every email. Every attachment represents a collection that may contain a name, content, size, and so on.

For more information, see [Item data types in Adobe Workfront Fusion](../../workfront-fusion/mapping/item-data-types.md).

## Access requirements

You must have the following access to use the functionality in this article:

<table> 
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

## Map an array

1. Click the button located in the target field. 

   <!--
   <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
   These steps from the source article are too vague
   </MadCap:conditionalText>
   -->

   **Example:** For the example above, you would click the Add an attachment button for an email.

   ![](assets/add-an-attachment-button-350x152.jpg)

1. In the box that displays, enter the item.

   The panel allows you to map fields in the same way as with any other type of item. If you do not want to fill in each item separately, but want to map another array into the target field, use the Map button. In this case, make sure that both arrays (the source array and the target array) have the same structure.

   You can add any number of items to an array.

You can divide an array into individual bundles using an iterator. Fore more information, see [Iterator module in Adobe Workfront Fusion](../../workfront-fusion/modules/iterator-module.md).
