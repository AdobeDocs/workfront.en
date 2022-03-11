---
filename: map-an-array
product: workfront-fusion
product-area: workfront-integrations
navigation-topic: mapping
title: Map an array
description: An array is a special type of item that can contain the following:
---

# Map an array

An array is a special type of item that can contain the following:

* One or more text values (simple array)
* One or more collections of the same type (complex array)

` `**Example: **``The Watch emails module returns an array of attachments for every email. Every attachment represents a collection that may contain a name, content, size, and so on.

For more information, see [Item data types](../../workfront-fusion/mapping/item-data-types.md).

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

## Map an array

<ol> 
 <li value="1"> <p>Click the button located in the target field. <!--
    These steps from the source article are too vague
   --></p> 
  <div class="example" data-mc-autonum="<b>Example: </b>">
   <span class="autonumber"><span><b>Example: </b></span></span> 
   <p>For the example above, you would click the Add an attachment button for an email. </p> 
   <p> <img src="assets/add-an-attachment-button-350x152.jpg" style="width: 350;height: 152;"> </p> 
  </div> </li> 
 <li value="2"> <p>In the box that displays, enter the item. </p> <p>The panel allows you to map fields in the same way as with any other type of item. If you do not want to fill in each item separately, but want to map another array into the target field, use the Map button. In this case, make sure that both arrays (the source array and the target array) have the same structure.</p> <p>You can add any number of items to an array.</p> </li> 
</ol>

You can divide an array into individual bundles using an iterator. Fore more information, see [Iterator module](../../workfront-fusion/modules/iterator-module.md).
