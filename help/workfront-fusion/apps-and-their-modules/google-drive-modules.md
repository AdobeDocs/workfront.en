---
filename: google-drive-modules
content-type: reference
product: workfront-fusion
product-area: workfront-integrations;documents
keywords: connector
navigation-topic: apps-and-their-modules
---



# Google Drive modules {#google-drive-modules}

The Google Drive modules enable you to monitor, search, create, update, delete, and manage your files, folder, or shared drives in your Google Drive.


In a *`Adobe Workfront Fusion`* scenario, you can connect your Google Drive account to multiple third-party applications and services.


If you need instructions on creating a scenario, see [Create a scenario](create-a-scenario.md). 


For information about modules, see [Modules in Adobe Workfront Fusion](_modules.md).


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
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray"> <p><span class="mc-variable WFVariables.WFFusionIntegration variable varname">Workfront Fusion for Work Automation and Integration</span> </p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-LightGray" role="rowheader">Product</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-LightGray">Your organization must purchase <span class="mc-variable WFVariables.FullProdNameWFF variable varname">Adobe Workfront Fusion</span> as well as <span class="mc-variable WFVariables.FullProdNameWF variable varname">Adobe Workfront</span> to use functionality described in this article.</td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your *`Workfront administrator`*.


&nbsp;


## Connecting Google Drive to *`Workfront Fusion`* {#connecting-google-drive-to-workfront-fusion}

If you are @gmail.com or @googlemail.com user you need to create an OAuth client on the [Google Cloud Platform](https://console.developers.google.com/projectselector2/apis/dashboard?supportedpurview=project) in order to obtain Client ID and Client Secret.


For step-by-step instructions on how to create the OAuth client (and obtain Client ID and Client Secret), see [Connect Adobe Workfront Fusion to Google Services using a custom OAuth client](connect-fusion-to-google-using-oauth.md).


For instructions about connecting your *`Google Drive`* account to *`Workfront Fusion`*, see [Create a connection to Workfront Fusion - Basic instructions](connect-to-fusion-general.md)


## Google Drive modules and their fields {#google-drive-modules-and-their-fields}

When you configure *`Google Drive`* modules, *`Workfront Fusion`* displays the fields listed below. Along with these, additional *`Google Drive`* fields might display, depending on factors such as your access level in the app or service. A bolded title in a module indicates a required field.


If you see the map button above a field or function, you can use it to set variables and functions for that field. For more information, see [Map information from one module to another](map-information-between-modules.md).


![](assets/map-toggle-350x74.png)






* [Triggers](#triggers) 
* [Actions](#actions) 




### Triggers {#triggers}




* [Watch Files In Folder](#watch) 
* [Watch All Files](#watch2) 
* [Watch shared files](#watch3) 
* [Watch Comments](#watch4) 




#### Watch Files In Folder {#watch-files-in-folder}

Retrieves file details when a file is added or modified in the specified folder.

<table style="width: 100%;mc-table-style: url('../../Resources/TableStyles/TableStyle-HeaderRow.css');" class="TableStyle-TableStyle-HeaderRow" cellspacing="15"> 
 <col style="width: 200px;" class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <col style="width: 50%;" class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <tbody> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray" style="font-weight: bold;" data-mc-conditions="QuicksilverOrClassic.Draft mode">Connection </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p>For instructions about connecting your Google Drive account to <span class="mc-variable WFVariables.ProdNameWFF variable varname">Workfront Fusion</span>, see <a href="#connecti" class="MCXref xref">Connecting Google Drive to Workfront Fusion</a></p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray" style="font-weight: bold;" data-mc-conditions="QuicksilverOrClassic.Draft mode">Select the folder to be watched</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray" data-mc-conditions="QuicksilverOrClassic.Draft mode">Select the folder on your drive that you want to watch the files in.</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray" style="font-weight: bold;" data-mc-conditions="QuicksilverOrClassic.Draft mode">What files to watch</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p>Select which type of files you want to watch.</p> 
    <ul> 
     <li>All</li> 
     <li>Google Documents</li> 
     <li>Google Spreadsheets</li> 
     <li>Google Slides</li> 
     <li>Google Drawings</li> 
    </ul> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray" style="font-weight: bold;" data-mc-conditions="QuicksilverOrClassic.Draft mode">Convert Google Documents files to format</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray" data-mc-conditions="QuicksilverOrClassic.Draft mode">Select the file format that you want to convert Google Documents to.</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray" style="font-weight: bold;" data-mc-conditions="QuicksilverOrClassic.Draft mode">Convert Google Spreadsheets files to format</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray" data-mc-conditions="QuicksilverOrClassic.Draft mode">Select the file format that you want to convert Google Spreadsheets to.</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray" style="font-weight: bold;" data-mc-conditions="QuicksilverOrClassic.Draft mode">Convert Google Slides files to format</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray" data-mc-conditions="QuicksilverOrClassic.Draft mode">Select the file format that you want to convert Google Documents to.</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray" style="font-weight: bold;" data-mc-conditions="QuicksilverOrClassic.Draft mode">Convert Google Drawings files to format</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray" data-mc-conditions="QuicksilverOrClassic.Draft mode">Select the file format that you want to convert Google Documents to.</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray" style="font-weight: bold;" data-mc-conditions="QuicksilverOrClassic.Draft mode">Watch</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray" data-mc-conditions="QuicksilverOrClassic.Draft mode">Select whether you want to watch new files and all changes, or only new files.</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyB-Column1-LightGray" style="font-weight: bold;" data-mc-conditions="QuicksilverOrClassic.Draft mode">Maximum number of downloaded files</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyA-Column1-LightGray" data-mc-conditions="QuicksilverOrClassic.Draft mode">Set the maximum number of results that Workfront Fusion will download during one cycle (the number of repetitions per scenario run).</td> 
  </tr> 
 </tbody> 
</table>



#### Watch All Files {#watch-all-files}

Retrieves file details when a file in your Google Drive is added or modified.

<table style="width: 100%;mc-table-style: url('../../Resources/TableStyles/TableStyle-HeaderRow.css');" class="TableStyle-TableStyle-HeaderRow" cellspacing="15"> 
 <col style="width: 200px;" class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <col style="width: 50%;" class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <tbody> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray" style="font-weight: bold;">Connection </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p>For instructions about connecting your Google Drive account to <span class="mc-variable WFVariables.ProdNameWFF variable varname">Workfront Fusion</span>, see <a href="#connecti" class="MCXref xref">Connecting Google Drive to Workfront Fusion</a></p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray" style="font-weight: bold;">What files to watch</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> <p>Select which type of files you want to watch.</p> 
    <ul> 
     <li>All</li> 
     <li>Google Documents</li> 
     <li>Google Spreadsheets</li> 
     <li>Google Slides</li> 
     <li>Google Drawings</li> 
    </ul> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray" style="font-weight: bold;">Convert Google Documents files to format</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray">Select the file format that you want to convert Google Documents to.</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray" style="font-weight: bold;">Convert Google Spreadsheets files to format</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray">Select the file format that you want to convert Google Spreadsheets to.</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray" style="font-weight: bold;">Convert Google Slides files to format</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray">Select the file format that you want to convert Google Documents to.</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray" style="font-weight: bold;">Convert Google Drawings files to format</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray">Select the file format that you want to convert Google Documents to.</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray" style="font-weight: bold;">Watch</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray">Select whether you want to watch new files and all changes, or only new files.</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyB-Column1-MediumGray" style="font-weight: bold;">Maximum number of downloaded files</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyA-Column1-MediumGray">Set the maximum number of results that Workfront Fusion will download during one cycle (the number of repetitions per scenario run).</td> 
  </tr> 
 </tbody> 
</table>



#### Watch shared files {#watch-shared-files}

Triggers when a new file is shared to you, or an existing shared file is updated.

<table style="width: 100%;mc-table-style: url('../../Resources/TableStyles/TableStyle-HeaderRow.css');" class="TableStyle-TableStyle-HeaderRow" cellspacing="15"> 
 <col style="width: 200px;" class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <col style="width: 50%;" class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <tbody> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray" style="font-weight: bold;">Connection </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p>For instructions about connecting your Google Drive account to <span class="mc-variable WFVariables.ProdNameWFF variable varname">Workfront Fusion</span>, see <a href="#connecti" class="MCXref xref">Connecting Google Drive to Workfront Fusion</a></p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray" style="font-weight: bold;">Select the folder to be watched</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray">Select the shared folder that you want to watch the files in.</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray" style="font-weight: bold;">What files to watch</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p>Select which type of files you want to watch.</p> 
    <ul> 
     <li>All</li> 
     <li>Google Documents</li> 
     <li>Google Spreadsheets</li> 
     <li>Google Slides</li> 
     <li>Google Drawings</li> 
    </ul> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray" style="font-weight: bold;">Convert Google Documents files to format</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray">Select the file format that you want to convert Google Documents to.</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray" style="font-weight: bold;">Convert Google Spreadsheets files to format</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray">Select the file format that you want to convert Google Spreadsheets to.</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray" style="font-weight: bold;">Convert Google Slides files to format</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray">Select the file format that you want to convert Google Documents to.</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray" style="font-weight: bold;">Convert Google Drawings files to format</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray">Select the file format that you want to convert Google Documents to.</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray" style="font-weight: bold;">Watch</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray">Select whether you want to watch new files and all changes, or only new files.</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyB-Column1-LightGray" style="font-weight: bold;">Maximum number of downloaded files</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyA-Column1-LightGray">Set the maximum number of results that Workfront Fusion will download during one cycle (the number of repetitions per scenario run).</td> 
  </tr> 
 </tbody> 
</table>



#### Watch Comments {#watch-comments}

Triggers when a comment is added or modified on the selected file.

<table style="width: 100%;mc-table-style: url('../../Resources/TableStyles/TableStyle-HeaderRow.css');" class="TableStyle-TableStyle-HeaderRow" cellspacing="15"> 
 <col style="width: 200px;" class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <col style="width: 50%;" class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <tbody> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray" style="font-weight: bold;">Connection </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p>For instructions about connecting your Google Drive account to <span class="mc-variable WFVariables.ProdNameWFF variable varname">Workfront Fusion</span>, see <a href="#connecti" class="MCXref xref">Connecting Google Drive to Workfront Fusion</a></p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray" style="font-weight: bold;">File</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray">Select the file that you want to watch for comments.</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray" style="font-weight: bold;">Watch</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray">Select whether you want to watch for all changes or for new comments only</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyB-Column1-MediumGray" style="font-weight: bold;">Maximum number of returned comments</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyA-Column1-MediumGray">Set the maximum number of comments that Workfront Fusion will return during one cycle (the number of repetitions per scenario run).</td> 
  </tr> 
 </tbody> 
</table>



### Actions {#actions}




* [Upload a File](#upload) 
* [Update a File](#update) 
* [Copy a File](#copy) 
* [Delete a File](#delete) 
* [Move a File/Folder to Trash](#move) 
* [Get a file](#get) 
* [Search for Files/Folders](#search2) 
* [Create a Folder](#create) 
* [Get a share link](#get2) 




#### Upload a File {#upload-a-file}

Uploads a file to your Google Drive.

<table style="width: 100%;mc-table-style: url('../../Resources/TableStyles/TableStyle-HeaderRow.css');" class="TableStyle-TableStyle-HeaderRow" cellspacing="15"> 
 <col style="width: 200px;" class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <col style="width: 50%;" class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <tbody> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray" style="font-weight: bold;">Connection </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p>For instructions about connecting your Google Drive account to <span class="mc-variable WFVariables.ProdNameWFF variable varname">Workfront Fusion</span>, see <a href="#connecti" class="MCXref xref">Connecting Google Drive to Workfront Fusion</a></p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray" style="font-weight: bold;">Destination</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> <p>Select the destination that you want to upload a file to.</p> 
    <ul> 
     <li>My Drive</li> 
     <li>Shared with Me</li> 
    </ul> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray" style="font-weight: bold;">Target folder</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray">Select the folder that you want to upload a file to. </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray" style="font-weight: bold;">Source file</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray">Select whether you want to use a file passed in from a previous module, or if you want to map the file manually.</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray" style="font-weight: bold;">File name</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray">Select the file name. This option is available if you select "Map" in the source file field.</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray" style="font-weight: bold;">Data</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray">Select the data file that you want to upload. This option is available if you select "Map" in the source file field.</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray" style="font-weight: bold;">Title</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray">Enter a title for the new file.</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyB-Column1-MediumGray" style="font-weight: bold;">Convert a file</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyA-Column1-MediumGray">Enabling this option allows the module to convert files to the corresponding Google format.</td> 
  </tr> 
 </tbody> 
</table>



#### Update a File {#update-a-file}

Updates a file's metadata or content.

<table style="width: 100%;mc-table-style: url('../../Resources/TableStyles/TableStyle-HeaderRow.css');" class="TableStyle-TableStyle-HeaderRow" cellspacing="15"> 
 <col style="width: 200px;" class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <col style="width: 50%;" class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <tbody> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray" style="font-weight: bold;">Connection </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p>For instructions about connecting your Google Drive account to <span class="mc-variable WFVariables.ProdNameWFF variable varname">Workfront Fusion</span>, see <a href="#connecti" class="MCXref xref">Connecting Google Drive to Workfront Fusion</a></p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray" style="font-weight: bold;">Destination</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> <p>Select the destination that you want to upload a file to.</p> 
    <ul> 
     <li>My Drive</li> 
     <li>Shared with Me</li> 
    </ul> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray" style="font-weight: bold;">Move to a folder</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray">If you want to move the file to a different folder, select the folder that you want to move the file into.</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray" style="font-weight: bold;">File ID</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray">Map the ID&nbsp;of the file that you want to update.</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray" style="font-weight: bold;">Title</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray">Enter a title for the updated file.</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray" style="font-weight: bold;">Change a file content</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray">Select whether you want to replace the content of the file.</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray" style="font-weight: bold;">Source file</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray">Select whether you want to use a file passed in from a previous module, or if you want to map the file manually. This field is available if you selected to change the file's content in the previous field.</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray" style="font-weight: bold;">File name</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray">Select the file name. This option is available if you select "Map" in the source file field.</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyB-Column1-LightGray" style="font-weight: bold;">Data</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyA-Column1-LightGray">Select the data file that you want to upload. This option is available if you select "Map" in the source file field.</td> 
  </tr> 
 </tbody> 
</table>



#### Copy a File {#copy-a-file}

Copies a file to the new location.

<table style="width: 100%;mc-table-style: url('../../Resources/TableStyles/TableStyle-HeaderRow.css');" class="TableStyle-TableStyle-HeaderRow" cellspacing="15"> 
 <col style="width: 200px;" class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <col style="width: 50%;" class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <tbody> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray" style="font-weight: bold;">Connection </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p>For instructions about connecting your Google Drive account to <span class="mc-variable WFVariables.ProdNameWFF variable varname">Workfront Fusion</span>, see <a href="#connecti" class="MCXref xref">Connecting Google Drive to Workfront Fusion</a></p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray" style="font-weight: bold;">Destination</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> <p>Select the destination that you want to upload a file to.</p> 
    <ul> 
     <li>My Drive</li> 
     <li>Shared with Me</li> 
    </ul> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray" style="font-weight: bold;">Target folder</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray">Select the folder where the file you want to copy is located/</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray" style="font-weight: bold;">File ID</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray">Map the ID&nbsp;of the file that you want to update.</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyB-Column1-LightGray" style="font-weight: bold;">The name of the copy</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyA-Column1-LightGray">Enter a title for the new file. Leave this field blank if you do not want to change the original file name.</td> 
  </tr> 
 </tbody> 
</table>



#### Delete a File {#delete-a-file}

Permanently deletes a file or folder.

<table style="width: 100%;mc-table-style: url('../../Resources/TableStyles/TableStyle-HeaderRow.css');" class="TableStyle-TableStyle-HeaderRow" cellspacing="15"> 
 <col style="width: 200px;" class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <col style="width: 50%;" class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <tbody> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray" style="font-weight: bold;">Connection </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p>For instructions about connecting your Google Drive account to <span class="mc-variable WFVariables.ProdNameWFF variable varname">Workfront Fusion</span>, see <a href="#connecti" class="MCXref xref">Connecting Google Drive to Workfront Fusion</a></p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyB-Column1-MediumGray" style="font-weight: bold;">File ID</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyA-Column1-MediumGray">Map the ID&nbsp;of the file that you want to delete.</td> 
  </tr> 
 </tbody> 
</table>



#### Move a File/Folder to Trash {#move-a-file-folder-to-trash}

Moves a file or folder to the trash.

<table style="width: 100%;mc-table-style: url('../../Resources/TableStyles/TableStyle-HeaderRow.css');" class="TableStyle-TableStyle-HeaderRow" cellspacing="15"> 
 <col style="width: 200px;" class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <col style="width: 50%;" class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <tbody> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray" style="font-weight: bold;">Connection </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p>For instructions about connecting your Google Drive account to <span class="mc-variable WFVariables.ProdNameWFF variable varname">Workfront Fusion</span>, see <a href="#connecti" class="MCXref xref">Connecting Google Drive to Workfront Fusion</a></p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyB-Column1-MediumGray" style="font-weight: bold;">File ID</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyA-Column1-MediumGray">Map the ID&nbsp;of the file that you want to move to the trash.</td> 
  </tr> 
 </tbody> 
</table>



#### Get a file {#get-a-file}

Retrieves the file with the ID specified.

<table style="width: 100%;mc-table-style: url('../../Resources/TableStyles/TableStyle-HeaderRow.css');" class="TableStyle-TableStyle-HeaderRow" cellspacing="15"> 
 <col style="width: 200px;" class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <col style="width: 50%;" class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <tbody> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray" style="font-weight: bold;">Connection </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p>For instructions about connecting your Google Drive account to <span class="mc-variable WFVariables.ProdNameWFF variable varname">Workfront Fusion</span>, see <a href="#connecti" class="MCXref xref">Connecting Google Drive to Workfront Fusion</a></p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray" style="font-weight: bold;">Convert Google Documents files to format</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray">Select the file format that you want to convert Google Documents to.</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray" style="font-weight: bold;">Convert Google Spreadsheets files to format</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray">Select the file format that you want to convert Google Spreadsheets to.</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray" style="font-weight: bold;">Convert Google Slides files to format</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray">Select the file format that you want to convert Google Documents to.</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray" style="font-weight: bold;">Convert Google Drawings files to format</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray">Select the file format that you want to convert Google Documents to.</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyB-Column1-MediumGray" style="font-weight: bold;">File ID</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyA-Column1-MediumGray">Map the ID&nbsp;of the file that you want to retrieve.</td> 
  </tr> 
 </tbody> 
</table>



#### Search for Files/Folders {#search-for-files-folders}

Searches for files or folders based on search criteria.

<table style="width: 100%;mc-table-style: url('../../Resources/TableStyles/TableStyle-HeaderRow.css');" class="TableStyle-TableStyle-HeaderRow" cellspacing="15"> 
 <col style="width: 200px;" class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <col style="width: 50%;" class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <tbody> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray" style="font-weight: bold;">Connection </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p>For instructions about connecting your Google Drive account to <span class="mc-variable WFVariables.ProdNameWFF variable varname">Workfront Fusion</span>, see <a href="#connecti" class="MCXref xref">Connecting Google Drive to Workfront Fusion</a></p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray" style="font-weight: bold;">Destination</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> <p>Select the destination that you want to search.</p> 
    <ul> 
     <li>My Drive</li> 
     <li>Shared with Me</li> 
    </ul> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray" style="font-weight: bold;">List a folder</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray">Navigate to the folder you want to search for the files or folders.</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray" style="font-weight: bold;">Retrieve</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> <p> Select whether you want to search for files, folders, or both.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray" style="font-weight: bold;"> <p>Search</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p>Select the type of the search you want to perform.</p> 
    <ul> 
     <li> <p><span class="bold">Search within file/folder names</span> </p> 
      <ul> 
       <li> <p><span class="bold">Query</span> </p> <p>Enter a part of the file name or full file name (including the suffix) you want to search.</p> </li> 
       <li> <p><span class="bold">Search Options</span> </p> <p>Select whether you want to search for the exact term, or if you want to search for names containing the search term.</p> </li> 
      </ul> </li> 
     <li> <p><span class="bold">Fulltext search</span> </p> 
      <ul> 
       <li> <p><span class="bold">Query</span> </p> <p>Enter any search term you want search in your Google Drive.</p> </li> 
      </ul> </li> 
     <li> <p><span class="bold">Enter custom search query</span> </p> 
      <ul> 
       <li> <p><span class="bold">Query</span> </p> <p>Enter the custom search query. For more details, please refer to the Search for Files section of this article.</p> </li> 
       <li> <p><span class="bold">Add the folder selected above to the query</span> </p> <p>Searches for the folder n the parents collection. This finds all files and folders located directly in the folder selected above.</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray" style="font-weight: bold;">Maximum number of returned results</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray">Set the maximum number of files or folders Workfront Fusion will return during one execution cycle.</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyB-Column1-LightGray" style="font-weight: bold;">Continue the execution of the route even if the module returns no results</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyA-Column1-LightGray">Enable this option to ensure that the scenario is not stopped if the module returns no results.</td> 
  </tr> 
 </tbody> 
</table>



#### Create a Folder {#create-a-folder}

Creates a folder in the specified location.

<table style="width: 100%;mc-table-style: url('../../Resources/TableStyles/TableStyle-HeaderRow.css');" class="TableStyle-TableStyle-HeaderRow" cellspacing="15"> 
 <col style="width: 200px;" class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <col style="width: 50%;" class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <tbody> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray" style="font-weight: bold;">Connection </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p>For instructions about connecting your Google Drive account to <span class="mc-variable WFVariables.ProdNameWFF variable varname">Workfront Fusion</span>, see <a href="#connecti" class="MCXref xref">Connecting Google Drive to Workfront Fusion</a></p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray" style="font-weight: bold;">Destination</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> <p>Select the destination that you want to upload a file to.</p> 
    <ul> 
     <li>My Drive</li> 
     <li>Shared with Me</li> 
    </ul> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray" style="font-weight: bold;">New folder location</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray">Navigate to the location where you want to create a new folder.</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray" style="font-weight: bold;">The name of the new folder</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray">Enter a name for the folder that you are creating.</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyB-Column1-LightGray" style="font-weight: bold;">Share folder</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyA-Column1-LightGray">Select this option if you want to share the folder with anyone with the Share link. Otherwise, the share link is for the owner only.</td> 
  </tr> 
 </tbody> 
</table>



#### Get a share link {#get-a-share-link}

Retrieves the share link for a file in Google Drive.

<table style="width: 100%;mc-table-style: url('../../Resources/TableStyles/TableStyle-HeaderRow.css');" class="TableStyle-TableStyle-HeaderRow" cellspacing="15"> 
 <col style="width: 200px;" class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <col style="width: 50%;" class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <tbody> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray" style="font-weight: bold;">Connection </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p>For instructions about connecting your Google Drive account to <span class="mc-variable WFVariables.ProdNameWFF variable varname">Workfront Fusion</span>, see <a href="#connecti" class="MCXref xref">Connecting Google Drive to Workfront Fusion</a></p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyB-Column1-MediumGray" style="font-weight: bold;">File ID</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyA-Column1-MediumGray">Map the ID&nbsp;of the file that you want to get the share link for.</td> 
  </tr> 
 </tbody> 
</table>



## Troubleshooting {#troubleshooting}



### Unable to upload or update a file {#unable-to-upload-or-update-a-file}

There are several situations when uploading or updating a file fails:



* The uploaded file is too big and exceeds the maximum file size limit allowed for your Google Drive plan or you have exceeded your Google Drive storage limit. You can either upgrade your storage plan or delete existing files from the Google Drive service.
* The selected folder where the file was to be uploaded to no longer exists. The scenario stops and it is then necessary to select a target folder again.




## Search for files {#search-for-files}

In the module List files in a folder you can use your own query which consists of these parts:



* `Field` - Attribute of the file that is being searched, for example, the attribute 

  ```
  name
  ```

  of the file.

* `Operator` - Test that is performed on the data to provide a match, for example, 

  ```
  contains
  ```

  .

* `Value` - The content of the attribute that is tested, for example, the name of the file 

  ```
  My cool document
  ```

  .



Combine clauses with the conjunctions 

```
and
```

or 

```
or
```

, and negate the query with 

```
not
```

.



* [Fields](#fields) 
* [Value types](#value) 
* [Operators](#operator) 
* [Examples](#examples) 




### Fields {#fields}


<table style="width: 100%;mc-table-style: url('../../Resources/TableStyles/TableStyle-HeaderRow.css');" class="TableStyle-TableStyle-HeaderRow" cellspacing="15"> 
 <col style="width: 200px;" class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <col style="width: 150px;" class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <col style="width: 200px;" class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <col style="width: 25%;" class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <thead> 
  <tr class="TableStyle-TableStyle-HeaderRow-Head-Header1"> 
   <th class="TableStyle-TableStyle-HeaderRow-HeadE-Column1-Header1">Field </th> 
   <th class="TableStyle-TableStyle-HeaderRow-HeadE-Column1-Header1">Value Type </th> 
   <th class="TableStyle-TableStyle-HeaderRow-HeadE-Column1-Header1">Operators</th> 
   <th class="TableStyle-TableStyle-HeaderRow-HeadD-Column1-Header1"> <p> Description</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"><code>title</code><![CDATA[	]]></td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">string</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"><code>contains</code><sup>1</sup>, <code>=</code>, <code>!=</code></td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p> Name of the file.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"><code>fullText</code> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">string </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"><code>contains</code><sup>2, 3</sup> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> <p> Full text of the file including name, description, content, and indexable text.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"><code>mimeType</code> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"> string</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"><![CDATA[	]]><code>contains</code>, <code>=</code>, <code>!=</code></td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p> MIME type of the file.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"><code>modifiedDate</code> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"> date<sup>4</sup></td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"><code> &lt;=</code>, <code>&lt;</code>, <code>=</code>, <code>!=</code>, <code>&gt;</code>, <code>&gt;=</code></td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> <p> Date of the last modification to the file.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"><code>lastViewedByMeDate</code> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"> date<sup>4</sup></td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"><code>&lt;=</code>, <code>&lt;</code>, <code>=</code>, <code>!=</code>, <code>&gt;</code>, <code>&gt;=</code></td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p> Date that the user last viewed a file.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"><code>trashed</code><![CDATA[	]]></td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">boolean </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"><code>=</code>, <code>!=</code></td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> <p> Whether the file is in the trash or not.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"><code>starred</code><![CDATA[	]]></td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">boolean </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"><code>=</code>, <code>!=</code><![CDATA[	]]></td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p>Whether the file is starred or not.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"><code>parents</code><![CDATA[	]]></td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">collection </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"><code>in </code> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> <p>Whether the parents collection contains the specified ID.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"><code>owners</code><![CDATA[	]]></td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">collection </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"><code>in </code> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p>Users who own the file.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"><code>writers</code><![CDATA[	]]></td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">collection </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"><code>in </code> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> <p>Users who have permission to modify the file.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"><code>readers </code> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">collection </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"><code>in </code> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p>Users who have permission to read the file.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"><code>sharedWithMe</code> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">boolean </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"><![CDATA[	]]><code>=</code>, <code>!=</code></td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> <p> Files that are in the user's "Shared with me" collection.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyB-Column1-LightGray"><code>properties </code> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyB-Column1-LightGray">collection</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyB-Column1-LightGray"><code>has </code> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyA-Column1-LightGray"> <p> Public custom file properties.</p> </td> 
  </tr> 
 </tbody> 
</table>

Consider the following about operators in these fields:



*  The 

  ```
  contains
  ```

  operator only performs prefix matching for a 

  ```
  title
  ```

  .


  For example, the title "HelloWorld" matches for 

  ```
  title contains 'Hello'
  ```

  but not for 

  ```
  title contains 'World'
  ```

  .

*  The 

  ```
  contains
  ```

  operator only performs matching on entire string tokens for 

  ```
  fullText
  ```

  .


  For example, if the full text of a doc contains the string "HelloWorld" only the query 

  ```
  fullText contains 'HelloWorld'
  ```

  returns a result. Queries such as fullText contains 'Hello' would not return results in this scenario.

*  The 

  ```
  contains
  ```

  operator matches on an exact alphanumeric phrase if it is surrounded by double quotes.


  For example, if the 

  ```
  fullText
  ```

  of a doc contains the string "Hello there world", then the query 

  ```
  fullText contains '"Hello there"'
  ```

  returns a result, but the query 

  ```
  fullText contains '"Hello world"'
  ```

  does not.


  Furthermore, because the search is alphanumeric, if the 

  ```
  fullText
  ```

  of a doc contains the string "Hello_world", then the query 

  ```
  fullText contains '"Hello world"'
  ```

  returns a result.

* Fields of 

  ```
  type
  ```

  date are currently not comparable to each other, only to constant dates.




### Value types {#value-types}


<table style="width: 100%;mc-table-style: url('../../Resources/TableStyles/TableStyle-HeaderRow.css');" class="TableStyle-TableStyle-HeaderRow" cellspacing="15"> 
 <col style="width: 200px;" class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <col style="width: 50%;" class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <thead> 
  <tr class="TableStyle-TableStyle-HeaderRow-Head-Header1"> 
   <th class="TableStyle-TableStyle-HeaderRow-HeadE-Column1-Header1">Value Type</th> 
   <th class="TableStyle-TableStyle-HeaderRow-HeadD-Column1-Header1"> <p> Notes</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">String </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p>Surround with single quotes '. Escape single quotes in queries with <code>\'</code>, e.g.,<code> 'Valentine\'s Day'</code>.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">Boolean </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> <p><code>true </code>or <code>false</code>.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyB-Column1-LightGray">Date </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyA-Column1-LightGray"> <p>RFC 3339 format, default timezone is UTC, e.g., <code>2012-06-04T12:00:00-08:00</code>.</p> </td> 
  </tr> 
 </tbody> 
</table>



### Operators {#operators}


<table style="width: 100%;mc-table-style: url('../../Resources/TableStyles/TableStyle-HeaderRow.css');" class="TableStyle-TableStyle-HeaderRow" cellspacing="15"> 
 <col style="width: 200px;" class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <col style="width: 50%;" class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <thead> 
  <tr class="TableStyle-TableStyle-HeaderRow-Head-Header1"> 
   <th class="TableStyle-TableStyle-HeaderRow-HeadE-Column1-Header1">Operator </th> 
   <th class="TableStyle-TableStyle-HeaderRow-HeadD-Column1-Header1"> <p>Notes</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"><code>contains</code><![CDATA[	]]></td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p>The content of one string is present in the other.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"><code>=</code> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> <p> The content of a string or boolean is equal to the other.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"><code>!=</code> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p> The content of a string or boolean is not equal to the other.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"><code>&lt;</code> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> <p> A date is earlier than another.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"><code>&lt;=</code> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p> A date is earlier than or equal to another.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"><code>&gt;</code> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> <p> A date is later than another.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"><code>&gt;=</code> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p> A date is later than or equal to another.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"><code>in </code> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> <p>An element is contained within a collection.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"><code>and </code> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p>Return files that match both clauses.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"><code>or </code> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> <p>Return files that match either clause.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"><code>not </code> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p>Negates a search clause.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyB-Column1-MediumGray"><code>has </code> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyA-Column1-MediumGray"> <p>A collection contains an element matching the parameters.</p> </td> 
  </tr> 
 </tbody> 
</table>

For compound clauses, you can use parentheses to group clauses together. For example:
`<pre>modifiedDate > '2012-06-04T12:00:00' and (mimeType contains 'image/' or mimeType contains 'video/')</pre>` This search returns all files with an image or video MIME type that their last modification was after June 4, 2012. Because 

```
and
```

and 

```
or
```

operators are evaluated from left to right, without parentheses, the above example would return only images modified after June 4, 2012, but would return all videos, even those before June 4, 2012.


### Examples {#examples}

All examples on this page show the unencoded `<q>q</q>` parameter, where 

```
title = 'hello'
```

is encoded as




```
title+%3d+%27hello%27
```

. Client libraries handle this encoding automatically.


Search for files with the name "hello"
`<pre>title = 'hello'</pre>` Search for folders using the folder-specific MIME type
`<pre>mimeType = 'application/vnd.google-apps.folder'</pre>` Search for files that are not folders
`<pre>mimeType != 'application/vnd.google-apps.folder'</pre>` Search for files with a name containing the words "hello" and "goodbye"
`<pre>title contains 'hello' and name contains 'goodbye'</pre>` Search for files with a name that does not contain the word "hello"
`<pre>not title contains 'hello'</pre>` Search for files containing the word "hello" in the content
`<pre>fullText contains 'hello'</pre>` Search for files not containing the word "hello" in the content
`<pre>not fullText contains 'hello'</pre>` Search for files containing the exact phrase "hello world" in the content
`<pre>fullText contains '"hello world"'fullText contains '"hello_world"'</pre>` Search for files with a query containing the "\" character (e.g., "\authors")
`<pre>fullText contains '\\authors'</pre>` Search for files writeable by the user "test@example.org"
`<pre>'test@example.org' in writers</pre>` Search for the ID 

```
1234567
```

in the 

```
parents
```

collection. This finds all files and folders located directly in the folder whose ID is 

```
1234567
```

.
`<pre>'1234567' in parents</pre>` Search for the alias ID 

```
appDataFolder
```

in the 

```
parents
```

collection. This finds all files and folders located directly under the [Application Data folder](https://developers.google.com/drive/api/v2/appdata).
`<pre>'appDataFolder' in parents</pre>` Search for files writeable by the users "test@example.org" and "test2@example.org"
`<pre>'test@example.org' in writers and 'test2@example.org' in writers</pre>` Search for files containing the text "important" which are in the trash
`<pre>fullText contains 'important' and trashed = true</pre>` Search for files modified after June 4th 2012
`<pre>modifiedDate > '2012-06-04T12:00:00' // default time zone is UTC</pre>``<pre>modifiedDate > '2012-06-04T12:00:00-08:00'</pre>` Search for files shared with the authorized user with "hello" in the name
`<pre>sharedWithMe and title contains 'hello'</pre>` Search for files with a [custom file property](https://developers.google.com/drive/api/v2/properties) named 

```
additionalID
```

with the value 

```
8e8aceg2af2ge72e78
```

.
`<pre>properties has { key='additionalID' and value='8e8aceg2af2ge72e78' and visibility='PRIVATE' }</pre>` Source of this guide is [Google Drive documentation](https://developers.google.com/drive/api/v2/search-shareddrives).
