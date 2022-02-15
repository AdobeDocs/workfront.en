---
filename: archive-modules
content-type: reference
product: workfront-fusion
product-area: workfront-integrations
navigation-topic: apps-and-their-modules
---



# Archive modules {#archive-modules}

In a *`Adobe Workfront Fusion`* scenario, you can connect an archive, such as a zipped file, to multiple third-party applications and services.


If you need instructions on creating a scenario, see [Create a scenario](create-a-scenario.md). For information about modules, see [Modules in Adobe Workfront Fusion](_modules.md).


## Archive modules and their fields {#archive-modules-and-their-fields}

When you configure *`Archive`* modules, *`Workfront Fusion`* displays the fields listed below. Along with these, additional *`Archive`* fields might display, depending on factors such as your access level in the app or service. A bolded title in a module indicates a required field.


If you see the map button above a field or function, you can use it to set variables and functions for that field. For more information, see [Map information from one module to another](map-information-between-modules.md).


![](assets/map-toggle-350x74.png)





* [Extract an archive](#extract) 
* [Create an archive](#create) 
* [Inflate](#inflate) 
* [Deflate](#deflate) 




## Extract an archive {#extract-an-archive}

This action module *`extracts a file you identify from an archive`*.


The module returns the ID of the `<MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE">  <span class="mc-variable Snippet_Variables.FusionAction variable varname">extracted</span></MadCap:conditionalText>` *`file`* and any associated fields, along with any custom fields and values that the connection accesses. You can map *`this information`* in subsequent modules in the scenario.

<table style="mc-table-style: url('../../Resources/TableStyles/TableStyle-HeaderRow.css');" class="TableStyle-TableStyle-HeaderRow" cellspacing="15"> 
 <col class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <col class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <tbody> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyB-Column1-LightGray" style="font-weight: bold;">Source file</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyA-Column1-LightGray"> <p> Select the file you want to extract. This file can be mapped from a previous module (such as Dropbox, Gmail, and so on.)</p> <p> <img src="assets/extract-an-archive-350x116.gif" style="width: 350;height: 116;"> </p> </td> 
  </tr> 
 </tbody> 
</table>


` `**Example: **`` Get the ZIP file from the defined Dropbox folder (for example, Archives), extract it using the Archive module and send extracted files to the desired email address as attachments with the Email or Gmail module.


![](assets/example-dropbox-350x134.png)




## Create an archive {#create-an-archive}

This aggregator module adds the desired files to a ZIP or TAR archive.


When you are configuring this module, the following fields display`<MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE"> , along with any other available  <span class="mc-variable Snippet_Variables.Fusion-Apps variable varname">Archive</span> fields, depending on the connection and options you choose</MadCap:conditionalText>`.

<table style="width: 100%;mc-table-style: url('../../Resources/TableStyles/TableStyle-HeaderRow.css');" class="TableStyle-TableStyle-HeaderRow" cellspacing="15"> 
 <col class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <col class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <tbody> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray" style="font-weight: bold;">Source module</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p> Select the module you want to retrieve the files from.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray" style="font-weight: bold;">Type </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> <p>Select whether you want to add files to a ZIP archive or a TAR archive.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray" style="font-weight: bold;">Comment</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray">Enter a comment that you would like to add to the archive.</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray" style="font-weight: bold;">Group by</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> <p>Define an expression that you want to group the aggregated output by. This expression can contain one or more mapped items. The aggregated data will be then separated into groups using this expression's value. Each group outputs as a separate bundle with a key (the evaluated expression) and a value (the aggregated text). You can use the key as a filter in subsequent modules.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray" style="font-weight: bold;">Stop processing after an empty aggregation</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray">Select this option to stop the scenario when there are no results.</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray" style="font-weight: bold;">Archive name</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> <p> Enter a name for the created archive. Do not add an extension.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyB-Column1-LightGray" style="font-weight: bold;">Source file</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyA-Column1-LightGray"> <p>Select a source file from a previous module, or map the source file's name and data.</p> </td> 
  </tr> 
 </tbody> 
</table>


` `**Example: **`` Watch incoming emails using the Gmail > Watch emails module. If an email is received, its attachments are iterated into individual bundles then archived to the ZIP file and saved to the defined Dropbox folder.


![](assets/example-gmail-350x102.png)




## Inflate {#inflate}

This transformer module decompresses binary data using an inflation algorithm.

<table style="width: 100%;mc-table-style: url('../../Resources/TableStyles/TableStyle-HeaderRow.css');" class="TableStyle-TableStyle-HeaderRow" cellspacing="15"> 
 <col class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <col class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <tbody> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyB-Column1-LightGray" style="font-weight: bold;">Data </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyA-Column1-LightGray"> <p>Enter or map the data you want to decompress using the inflate function.</p> </td> 
  </tr> 
 </tbody> 
</table>



## Deflate {#deflate}

This transformer module compresses binary data using a deflation algorithm.

<table style="width: 100%;mc-table-style: url('../../Resources/TableStyles/TableStyle-HeaderRow.css');" class="TableStyle-TableStyle-HeaderRow" cellspacing="15"> 
 <col class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <col class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <tbody> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyB-Column1-LightGray" style="font-weight: bold;">Data </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyA-Column1-LightGray"> <p>Enter or map the data you want to compress using the deflate function.</p> </td> 
  </tr> 
 </tbody> 
</table>

