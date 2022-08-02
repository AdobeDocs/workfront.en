---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: apps-and-their-modules
title: Image modules
description: Adobe Workfront Fusion Image modules allow you get information about a specific image (dimensions, type, and so on), convert an image to another file format, and directly change the size of the image.
author: Becky
feature: Workfront Fusion, Digital Content and Documents
exl-id: 89efa9d5-00c9-4bb5-97b3-2b2f9d73721d
---
# Image modules

Adobe Workfront Fusion Image modules allow you get information about a specific image (dimensions, type, and so on), convert an image to another file format, and directly change the size of the image.

## Access requirements

You must have the following access to use the functionality in this article:

<table style="table-layout:auto"> 
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
   <td> <p>Workfront Fusion for Work Automation and Integration </p>  <p>Workfront Fusion for Work Automation</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>Your organization must purchase Adobe Workfront Fusion as well as Adobe Workfront to use functionality described in this article.</td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your Workfront administrator.

&#42;&#42;For information on Adobe Workfront Fusion licenses, see [Adobe Workfront Fusion licenses](../../workfront-fusion/get-started/license-automation-vs-integration.md)

## Image modules and their fields

When you are configuring this module, the following fields display. A bolded title in a module indicates a required field.

* [Resize](#resize) 
* [Convert a format](#convert-a-format) 
* [Extract metadata](#extract-metadata)

### Resize {#resize}

This transformer module changes an image's height and width according to criteria you specify.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader">Source file</td> 
   <td> <p>Select the source of the image you want to convert. You can select output from a previous module or map the data file and filename. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Data</td> 
   <td>Map the file that you want to convert. This field is available if you selected Map in the Source file field.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">File name</td> 
   <td>Enter a name for the converted file. This field is available if you selected Map in the Source file field.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">I want to</td> 
   <td>Select whether you want to maintain the height-width ratio or change the dimensions to a specified height and width.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">According to</td> 
   <td> <p>Select how you want the module to determine the new size of the image. This field appears if you selected to maintain height-width ration in the I&nbsp;want to field. Other fields appear based on the selection in this field.</p> 
    <ul> 
     <li> <p>Maximum width</p> <p>Reduces an image to a width you specify. Height is calculated automatically.</p> </li> 
     <li> <p>Maximum height</p> <p>Reduces an image to a height you specify. Width is calculated automatically.</p> </li> 
     <li> <p>Maximum height or width</p> <p>Reduces an image in a way that its height and width do not exceed the values you specify. Because this option maintains height-width ratio, one of the dimensions may be smaller than specified. For example, if height and width are both specified as 40, a 400x300 image will be reduced to 40X30.</p> </li> 
     <li> <p>Minimum width</p> <p>Enlarges an image to a width you specify. Height is calculated automatically.</p> </li> 
     <li> <p>Minimum height</p> <p>Enlarges an image to a height you specify. Width is calculated automatically.</p> </li> 
     <li> <p>Minimum height or width</p> <p>Enlarges an image in a way that its height and width are not smaller than the values you specify. Because this option maintains height-width ratio, one of the dimensions may be larger than specified. For example, if height and width are both specified as 300, a 40x30 image will be enlarged to 400X300.</p> </li> 
     <li> <p>Percent</p> <p>Changes the image size by a percentage based on the value you specify. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Width</td> 
   <td>Enter or map the desired width of the resized image in pixels.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Height</td> 
   <td>Enter or map the desired height of the resized image in pixels.</td> 
  </tr> 
 </tbody> 
</table>

### Convert a format {#convert-a-format}

This transformer module changes the format of an image file. This module is compatible the following formats:

* PNG
* JPG
* GIF
* BMP

Both the source file and the output must be in one of these formats. For example, the Image > Convert a format module can transform a PNG file into a BMP file, or a BMP&nbsp;into a JPG.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader">Source file</td> 
   <td> <p>Select the source of the image you want to convert. You can select output from a previous module or map the data file and filename. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Data</td> 
   <td>Map the file that you want to convert. This field is available if you selected Map in the Source file field.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">File name</td> 
   <td>Enter a name for the converted file. This field is available if you selected Map in the Source file field.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Output format</td> 
   <td>Select the format that you want the module to convert the source file to. </td> 
  </tr> 
 </tbody> 
</table>

### Extract metadata {#extract-metadata}

This transformer module returns basic information about a module.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader">Source file</td> 
   <td> <p>Select the source of the image you want to convert. You can select output from a previous module or map the data file and filename. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Data</td> 
   <td>Map the file that you want to convert. This field is available if you selected Map in the Source file field.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">File name</td> 
   <td>Enter a name for the converted file. This field is available if you selected Map in the Source file field.</td> 
  </tr> 
 </tbody> 
</table>

## Possible problems

### Action terminated with an error

There are three cases when an action can terminate with an error:

* Received data was not in the JPG/GIF/PNG/BMP format
* The maximum width/height limit had been exceeded while changing the image dimensions. The image size must not exceed 3840 px width and 2160 px height
* The maximum allowable size of an image had been exceeded while changing the dimensions or format of the image.
