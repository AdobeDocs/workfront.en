---
filename: sdl-managed-translation-modules
content-type: reference
product: workfront-fusion
product-area: workfront-integrations
keywords: connector
navigation-topic: apps-and-their-modules
---



# SDL Managed Translation modules {#sdl-managed-translation-modules}



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


## SDL&nbsp;Managed Translation Modules {#sdl-managed-translation-modules-1}



>[!NOTE]
>
>The operation timeout for calls to SDL Managed Translation is **120 seconds**.




### Files {#files}



#### Download Translated File {#download-translated-file}

This module retrieves the content of a single translated file, contained within the specified project. If the requested file is not yet in Downland status, the content of the file may not yet be fully translated. If the file is in Download status, and you have successfully retrieved it, be sure to mark the file as complete using the 

```
Cancel or Complete File
```

method.


#### Upload a File {#upload-a-file}

This module allows uploads of files for translation or for inclusion in a translation project as reference material. Uploads must be submitted using multipart/form-data and can contain more than one file. You specify the 

```
ProjectOptionId
```

that should be used to evaluate the uploaded file(s). This determines whether each file you upload is a possible candidate for translation or must be handled as reference material. In the case of archives (

```
zip
```

, 

```
rar
```

, 

```
7z
```

, 

```
tar
```

files) the app examines the contents of the archive and indicates whether the archive as a whole can be translated, or whether it contains a mixture of translatable and non-translatable files.


>[!NOTE]
>
>Uploading more than one file at a time is not recommended, because it can increase the impact of any failure.




#### Add a Reference File {#add-a-reference-file}

This module adds a Reference File.


### Projects  {#projects}



#### Create a project {#create-a-project}

This module creates the specified project.


#### Cancel or Complete a Project {#cancel-or-complete-a-project}

This module cancels or completes the specified project. If the project is awaiting download, the project transitions through any final steps in the workflow, and eventually moves to complete. If the project is awaiting approval or vendor selection is cancelled. If the project is at any other status, the request will fail.


#### Download Project Zip {#download-project-zip}

This module gets the 

```
zip
```

file of translated files for the specified project.


#### Read a Project {#read-a-project}

This module gets the specified project.


#### Get Projects at Status {#get-projects-at-status}

This module gets all available projects in the specified status. This method allows the results to be paged, by specifying 

```
$top
```

, 

```
$skip
```

, and 

```
$orderby
```

query parameters.


#### Get Projects List {#get-projects-list}

Gets a simple list of all projects, providing general information about each project. This method allows the results to be pages, by specifying 

```
$top
```

, 

```
$skip
```

, and 

```
$orderby
```

query parameters.


#### Search Project Creation Options {#search-project-creation-options}

This module gets Project Creation Options.


### Other {#other}



#### Make an API Call {#make-an-api-call}

This module performs an arbitrary authorized API call.
