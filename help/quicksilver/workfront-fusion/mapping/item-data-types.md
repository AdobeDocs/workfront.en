---
filename: item-data-types
content-type: reference
product: workfront-fusion
product-area: workfront-integrations
navigation-topic: mapping
title: Item data types in Adobe Workfront Fusion
description: You must have the following access to use the functionality in this article - EDIT ME.
---

# Item data types in Adobe Workfront Fusion

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

## Item data types

You can contain the types of items listed below in a bundle.

For information on which types of items Workfront Fusion allows for conversion between one other, see [Type coercion in Adobe Workfront Fusion](../../workfront-fusion/mapping/type-coercion.md).

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p><a name="Text"></a>Text</p> </td> 
   <td> <p>The most common item type. For some text items, Adobe Workfront Fusion checks whether the maximum or minimum allowed length is met or whether the item performs format validation (email, URL or file name).</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Number</p> </td> 
   <td> <p>For some numerical items, Workfront Fusion may validate the input for a specified range (the minimum or maximum allowed value).</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Boolean (Yes/No)</p> </td> 
   <td> <p>This type is used for items with only two possible values: true or false. </p> <p>When setting modules, the Boolean type can appear in two different forms:</p> 
    <ul> 
     <li> <p>The compulsory check box is shown in case the field is mandatory and must be filled in.</p> <p> <img src="assets/boolean-checkbox-350x158.jpg" style="width: 350;height: 158;"> </p> </li> 
     <li> <p>Optional fields that can be left blank are displayed as a selection box, allowing selection among three values: <code>Yes</code>, <code>No</code>, and <code>Not defined</code> (default).</p> <p> <img src="assets/boolean-convert-file-350x129.jpg" style="width: 350;height: 129;"> </p> </li> 
    </ul> <p>You can click <strong>Map</strong> if you need to map the value to an item from another module.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p><a name="Date"></a>Date</p> </td> 
   <td> <p>Dates are entered in the ISO 8601 date format, for example, <code>2015-09-18T11:58Z</code>. You can change the time zone in your profile settings, as explained in <a href="../../workfront-fusion/workfront-fusion-basics/change-profile-settings.md" class="MCXref xref">Change profile settings in Adobe Workfront Fusion</a>. </p> <p>If you click a field that requires a date, a pop-up calendar displays in the module settings. The time is not required for some items.</p> <p>Values of Date items are formatted using the local and Web timezone selected in your profile. You can display the ISO 8601 version of a date item's value by hovering over the item.</p> <p>Note: If the ISO value does not display, the item is probably text, not a date.</p> <p>The time is entered in the <code>hours:minutes:seconds</code> format, for example,<code>14:03:52</code>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Buffer (binary data)</p> </td> 
   <td> <p>File content is usually sent as Buffer type content (image content, video file, and others). In some cases, text data is included in this type (for example, a text file). Workfront Fusion is able to automatically convert text data in binary code to text and text to text data in binary code. For more information, see <a href="../../workfront-fusion/mapping/about-mapping-files.md" class="MCXref xref">About mapping files in Adobe Workfront Fusion</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Collection</p> </td> 
   <td> <p>A collection is an item consisting of multiple sub-items. The Sender item in an email message is an example of a collection: it contains the sender name (text type) and the sender email address (text type).</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Select (menu)</p> </td> 
   <td> <p>When you configure the module settings as described in <a href="../../workfront-fusion/modules/configure-a-modules-settings.md" class="MCXref xref">Configure a module's settings in Adobe Workfront Fusion</a>, you can select from several items of the same type. An example is the folder select menu in the settings for the Dropbox modules. </p> <p>When setting modules, the select menu can appear in two forms:</p> <p> <p>If multiple selection is possible, several items with check boxes display.</p> <p> <img src="assets/image-kb-type-list-multi-350x232.jpg" style="width: 350;height: 232;"> </p> </p> <p>If only one option is possible, a drop-down menu displays.</p> <p> <img src="assets/select-menu-dropdown-350x130.jpg" style="width: 350;height: 130;"> </p> <p>If you need to map an item from another module, use the <strong>Map</strong> button. This button opens a text field instead of the selection menu. For more information, see <a href="../../workfront-fusion/mapping/map-information-between-modules.md" class="MCXref xref">Map information from one module to another in Adobe Workfront Fusion</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Array</p> </td> 
   <td> <p>You can use the array type to work with several values of the same type, including collections. An example is the Email modules:&nbsp;they return an array of attachments and each attachment contains name, content, size, and so on. For more information, see <a href="../../workfront-fusion/mapping/map-an-array.md" class="MCXref xref">Map an array in Adobe Workfront Fusion</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Validation</p> </td> 
   <td> <p>Workfront Fusion might perform validation on each type of item. If an item does not pass the validation, the module will stop processing because of a data error. For more information, see <a href="../../workfront-fusion/errors/error-processing.md" class="MCXref xref">Error processing in&nbsp;Adobe Workfront Fusion</a>. </p> </td> 
  </tr> 
 </tbody> 
</table>

