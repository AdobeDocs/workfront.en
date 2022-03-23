

# CloudConvert modules

Adobe Workfront Fusion requires an Adobe Workfront Fusion license in addition to an Adobe Workfront license.
In a Adobe Workfront Fusion scenario, you can connect your CloudConvert account to multiple third-party applications and services. The CloudConvert modules allow you to monitor and manage jobs, tasks, and import and export files in your CloudConvert account.

* [Connect CloudConvert to Workfront Fusion](#connect) 
* [CloudConvert modules and their fields](#cloudcon) 
* [Troubleshooting](#troubles)

## Connect CloudConvert to Workfront Fusion

To connect your CloudConvert account to Workfront Fusion, you need to obtain the API Key from your CloudConvert account.

1. Log in to your CloudConvert account and open your Dashboard.
1. Open the **Authorization > API Keys** section.
1. Click **Create New API key**.
1. Enter the name for the API key, enable the scopes you want to use, then click **Create**.
1. Copy the provided token and store it in a safe place.
1. In Workfront Fusion, start creating a scenario open the CloudConvert module's **Create a connection** dialog.

   For instructions, see [Create a scenario](../../workfront-fusion/scenarios/create-a-scenario.md).

1. Enter the token you saved in step 5, then click **Continue** to establish the connection.

## CloudConvert modules and their fields

When you configure CloudConvert modules, Workfront Fusion displays the fields listed below. Along with these, additional CloudConvert fields might display, depending on factors such as your access level in the app or service. A bolded title in a module indicates a required field.

If you see the map button above a field or function, you can use it to set variables and functions for that field. For more information, see [Map information from one module to another](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [CloudConvert modules](#common2) 
* [Jobs](#jobs) 
* [Tasks](#tasks) 
* [Other](#other)

### Common tasks

* [Capture a Website](#capture) 
* [CloudConvert modules](#convert) 
* [Create an Archive](#create) 
* [Merge Files](#merge) 
* [Optimize a File](#optimize)

#### Capture a Website

This action module captures a specified website and saves it in PDF, JPG, or PNG format.

You specify the URL of the website and other information, such as where you want the information stored.

The module returns the ID of the file and any associated fields, along with any custom fields and values that the connection accesses. You can map this information in subsequent modules in the scenario.

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection</td> 
   <td> <p>For instructions about connecting your CloudConvert account to Workfront Fusion, see <a href="#connect" class="MCXref xref">Connect CloudConvert to Workfront Fusion</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">URL</td> 
   <td>Enter the URL of the website you want to capture. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Output Format </td> 
   <td>Select whether you want to save the captured website in PNG, JPG, or PDF format. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">File Name </td> 
   <td><![CDATA[
]]>Enter a file name (including extension) for the target output file.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Headers </td> 
   <td> <p>(Optional) Define request headers. </p> <p>This is useful, for example, when the specified URL requires authorization. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Conversion and engine specific options </p> </td> 
   <td>Specify conversion and engine specific options. To view available options, see the <a href="https://cloudconvert.com/api/v2/convert#convert-tasks">Cloud Convert API</a> documentation for <code>input_format</code> and <code>output_format</code>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Download a file </td> 
   <td> <p>Enable this option if you also want to include file data in the module's output.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### Convert a file

Converts a file into a selected output format.

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection</td> 
   <td> <p>For instructions about connecting your CloudConvert account to Workfront Fusion, see <a href="#connect" class="MCXref xref">Connect CloudConvert to Workfront Fusion</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Input file</td> 
   <td>Select whether you want to upload a file using Workfront Fusion or provide the URL the file will be uploaded from.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Upload a file</td> 
   <td> <p>Select a source file from a previous module, or map the source file's name and data.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Import a File from URL</td> 
   <td> 
    <ul> 
     <li> <p><strong>URL</strong> </p> <p>Enter the URL of the file you want to convert.</p> </li> 
     <li> <p><![CDATA[

]]><strong>Headers</strong></p> <p>Define request headers (optional). This is useful, for example, when the specified URL requires the authorization.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Format</td> 
   <td>Select whether you want to specify the input format of the file you want to convert. If not specified, the extension of the input file is used as the input format.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Input Format</td> 
   <td>Select the current format of the file.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Output Format</td> 
   <td>Select the target file format you want to convert the file to.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">File Name</td> 
   <td>Choose a filename (including extension) for the target output file.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>Conversion and engine specific options </p> </td> 
   <td>Specify conversion and engine specific options. To view available options, see the <a href="https://cloudconvert.com/api/v2/convert#convert-tasks">Cloud Convert API</a> documentation for <code>input_format</code> and <code>output_format</code>.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Download a file </td> 
   <td> <p>Enable this option if you also want to include file data in the module's output.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### Create an Archive

Enables you to add one or multiple files to the ZIP, RAR, 7Z, TAR, TAR.GZ or TAR.BZ2 archive.

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection</td> 
   <td> <p>For instructions about connecting your CloudConvert account to Workfront Fusion, see <a href="#connect" class="MCXref xref">Connect CloudConvert to Workfront Fusion</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Input Files</p> </td> 
   <td> <p>Specify files you want to add to the archive.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Upload a File</td> 
   <td> <p>Select a source file from a previous module, or map the source file's name and data.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Import a file from URL</p> </td> 
   <td> <p><strong>URL</strong> </p> <p>Enter the URL of the file you want to archive.</p> <p><strong>Headers</strong> </p> <p>Define request headers (optional). This is useful, for example, when the specified URL requires the authorization.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Output Format</td> 
   <td> <p> Select the target format of the archived file.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">File name</td> 
   <td> <p> Enter the file name (including extension) for the target output file.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Conversion and engine specific options </td> 
   <td> <p>Specify conversion and engine specific options. To view available options, see the <a href="https://cloudconvert.com/api/v2/convert#convert-tasks">Cloud Convert API</a> documentation for <code>input_format</code> and <code>output_format</code>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Download a File</td> 
   <td> <p>Enable this option if you also want to include file data in the module's output.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### Merge Files

Merges at least two files into one PDF. If input files are not PDFs, they are automatically converted to PDF.

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection</td> 
   <td> <p>For instructions about connecting your CloudConvert account to Workfront Fusion, see <a href="#connect" class="MCXref xref">Connect CloudConvert to Workfront Fusion</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Input Files</p> </td> 
   <td> <p>Specify files you want to merge.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Upload a File</td> 
   <td> <p>Select a source file from a previous module, or map the source file's name and data.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Import a file from URL</p> </td> 
   <td> <p><strong>URL</strong> </p> <p>Enter the URL of the file you want to archive.</p> <p><strong>Headers</strong> </p> <p>Define request headers (optional). This is useful, for example, when the specified URL requires the authorization.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Output Format</td> 
   <td> <p> Select the target format of the merged file.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">File name</td> 
   <td> <p> Enter the file name (including extension) for the target output file.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Conversion and engine specific options </td> 
   <td> <p>Specify conversion and engine specific options. To view available options, see the <a href="https://cloudconvert.com/api/v2/convert#convert-tasks">Cloud Convert API</a> documentation for <code>input_format</code> and <code>output_format</code>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Download a File</td> 
   <td> <p>Enable this option if you also want to include file data in the module's output.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### Optimize a File

This action module optimizes and compresses a file in PDF, PNG, or JPG format.

You specify the file and the parameters for optimizing and storing it.

The module returns the ID of the  file and any associated fields, along with any custom fields and values that the connection accesses. You can map this information in subsequent modules in the scenario.

When you are configuring this module, the following fields display.

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection</td> 
   <td> <p>For instructions about connecting your CloudConvert account to Workfront Fusion, see <a href="#connect" class="MCXref xref">Connect CloudConvert to Workfront Fusion</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Input File</td> 
   <td>Select whether you want to upload a file using Workfront Fusion or provide the URL from which the file will be uploaded.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Upload a File</p> </td> 
   <td> <p>Select a source file from a previous module, or map the source file's name and data.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Import a file from URL </td> 
   <td> 
    <ul> 
     <li><strong>URL</strong>: Enter the URL of the file you want to convert.</li> 
     <li><strong>Headers</strong>: (Optional) Define request headers. This is useful, for example, when the specified URL requires authorization.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Optimization for </td> 
   <td> <p>Select the optimization profile for specific target needs.</p> 
    <ul> 
     <li> <p><strong>Web</strong>: Optimization for the web (Default)</p> 
      <ul> 
       <li>Remove redundant and unnecessary data for the web</li> 
       <li>Down-sample, clip, and intelligently compress images</li> 
       <li>Merge and subset fonts</li> 
       <li>Convert colors to RGB</li> 
      </ul> </li> 
    </ul> 
    <ul> 
     <li> <p><strong>Print</strong>: Optimization for print</p> 
      <ul> 
       <li> <p>Remove redundant and unnecessary data for printing</p> </li> 
       <li> <p>Down-sample, clip, and intelligently compress images</p> </li> 
       <li> <p>Merge and subset fonts</p> </li> 
       <li> <p>Convert colors to CMYK</p> </li> 
      </ul> </li> 
     <li> <p><strong>Archive</strong>: Optimization for archiving purposes</p> 
      <ul> 
       <li> <p>Remove redundant and unnecessary data for archiving</p> </li> 
       <li> <p>Intelligently compress images</p> </li> 
       <li> <p>Merge and subset fonts</p> </li> 
      </ul> </li> 
     <li> <p><strong>Scanned images</strong>: Optimization for scanned images</p> 
      <ul> 
       <li> <p>Profile optimized for PDFs that mainly consist of raster images</p> </li> 
       <li> <p>Compress the images without significantly reducing the visual quality</p> </li> 
      </ul> </li> 
     <li> <p><strong>maximal size reduction</strong>: Optimization for maximal size reduction</p> 
      <ul> 
       <li> <p>Use the maximal possible compression</p> </li> 
       <li> <p>Might reduce the visual quality</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Input format </td> 
   <td>Select the format of the input file you want to optimize. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">File name</td> 
   <td> <p>Enter a file name (including extension) for the target output file.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Conversion and engine specific options</td> 
   <td> <p>Specify conversion and engine specific options. To view available options, see the <a href="https://cloudconvert.com/api/v2/convert#convert-tasks">Cloud Convert API</a> documentation for <code>input_format</code> and <code>output_format</code>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Download a file</td> 
   <td> <p>Enable this option if you also want to include file data in the module's output.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Jobs

* [Create a Job (advanced)](#create2) 
* [New Job Event](#new) 
* [List Jobs](#list) 
* [Get a Job](#get) 
* [Delete a Job](#delete)

#### Create a Job (advanced)

This module creates a job. A job can be one or multiple tasks that are identified in the Name field and linked between each other using the Input field.

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">For further processing of the finished job created with the Create a Job module, please use the New Job Event (job.finished) module in another scenario.</p>
-->

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection</td> 
   <td> <p>For instructions about connecting your CloudConvert account to Workfront Fusion, see <a href="#connect" class="MCXref xref">Connect CloudConvert to Workfront Fusion</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Input Files</td> 
   <td> <p>Select whether you want to upload a file using Workfront Fusion, or provide the URL from which the file will be uploaded.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Upload a File</td> 
   <td> <p>Select a source file from a previous module, or map the source file's name and data.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Import a File from URL</p> </td> 
   <td> 
    <ul> 
     <li><strong>URL</strong>: Enter the URL of the file you want to process.</li> 
     <li><strong>Headers</strong>: (Optional) Define request headers. This is useful, for example, when the specified URL requires authorization.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Tasks</p> </td> 
   <td> <p>Add tasks that will be performed within the job.</p> <p>Please find the descriptions of the operations' fields in the corresponding section.</p> 
    <ul> 
     <li><a href="#convert" class="MCXref xref">CloudConvert modules</a> </li> 
     <li><a href="#capture" class="MCXref xref">Capture a Website</a> </li> 
     <li><a href="#optimize" class="MCXref xref">Optimize a File</a> </li> 
     <li><a href="#create" class="MCXref xref">Create an Archive</a> </li> 
     <li><a href="#merge" class="MCXref xref">Merge Files</a> </li> 
    </ul> 
    <ul> 
     <li> <p><strong>Execute a Command</strong> </p> <p>For more information on executing a command, see the <a href="https://cloudconvert.com/api/v2/command#command-tasks">CloudConvert API documentation</a>.</p> </li> 
     <li> <p><strong>Export a File to Temporary URL</strong> </p> <p> Specify the task name and input task name (e.g. Conversion).</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Tag </td> 
   <td> <p>Enter a tag. Tags are arbitrary strings to identify the job. They do not have any effect and can be used to associate the job with an ID.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### Delete a Job

This module deletes a job, including all tasks and data.

>[!NOTE]
>
>Jobs are deleted automatically 24 hours after they have ended.

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection</td> 
   <td> <p>For instructions about connecting your CloudConvert account to Workfront Fusion, see <a href="#connect" class="MCXref xref">Connect CloudConvert to Workfront Fusion</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Job ID</td> 
   <td> <p>Enter or map the ID of the job you want to delete.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### Get a Job

This module retrieves job details.

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection</td> 
   <td> <p>For instructions about connecting your CloudConvert account to Workfront Fusion, see <a href="#connect" class="MCXref xref">Connect CloudConvert to Workfront Fusion</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Job ID</td> 
   <td> <p>Enter or map the ID of the job you want to retrieve details about.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### List Jobs

This module retrieves all jobs that have been run in your account.

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection</td> 
   <td> <p>For instructions about connecting your CloudConvert account to Workfront Fusion, see <a href="#connect" class="MCXref xref">Connect CloudConvert to Workfront Fusion</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Status </td> 
   <td> <p>Select the job status to filter returned jobs by.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Limit </td> 
   <td> <p>Set the number of jobs Workfront Fusion 2.0 will return during one execution cycle.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### New Job Event

Triggers when a job in your account or task is created, finishes, or fails.

>[!NOTE]
>
>* The job created by the Create a Job (advanced) module consists of *several* tasks.
>* The New Job Event trigger is also triggered when an *individual* task is created, has finished, or has failed.
>

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Webhhook name</td> 
   <td>Enter the webhook name. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Connection</td> 
   <td> <p>For instructions about connecting your CloudConvert account to Workfront Fusion, see <a href="#connect" class="MCXref xref">Connect CloudConvert to Workfront Fusion</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Output Format </td> 
   <td>Select whether you want to save the captured website in PNG, JPG, or PDF format. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Event</td> 
   <td>Select whether the module is triggered when the job or task is created, finishes, or fails.</td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>* If working with the Array Aggregator (e.g. you have many files in different formats to convert), use the **I don't know the input format** option in the Add a task dialog. Otherwise the error is returned.
>* Linking tasks within the job (name > input, name > input,...):
>
>  ![](assets/linking-name-across-jobs-350x808.png)>

### Tasks

* [Get a Task](#get2) 
* [Download a File](#download) 
* [List Tasks](#list2) 
* [Retry a Task](#retry) 
* [Cancel a Task](#cancel) 
* [Delete a Task](#delete2)

#### Cancel a Task

This module cancels a task that has a status of waiting or processing.

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection</td> 
   <td> <p>For instructions about connecting your CloudConvert account to Workfront Fusion, see <a href="#connect" class="MCXref xref">Connect CloudConvert to Workfront Fusion</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Task ID</td> 
   <td> <p> Enter or map the ID of the task you want to cancel.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### Delete a Task

Delete a task, including all data.

>[!NOTE]
>
>Tasks are deleted automatically 24 hours after they have ended.

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection</td> 
   <td> <p>For instructions about connecting your CloudConvert account to Workfront Fusion, see <a href="#connect" class="MCXref xref">Connect CloudConvert to Workfront Fusion</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Task ID</td> 
   <td> <p> Enter (map) the ID of the task you want to delete.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### Download a File

This module retrieves file name and file data from the specified task.

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection</td> 
   <td> <p>For instructions about connecting your CloudConvert account to Workfront Fusion, see <a href="#connect" class="MCXref xref">Connect CloudConvert to Workfront Fusion</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Task ID</td> 
   <td> <p> Enter or map the ID of the task you want to download the file from.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### Get a Task

This module retrieves task details.

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection</td> 
   <td> <p>For instructions about connecting your CloudConvert account to Workfront Fusion, see <a href="#connect" class="MCXref xref">Connect CloudConvert to Workfront Fusion</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Task ID</td> 
   <td> <p>Enter or map the ID of the task you want to retrieve details about.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### List Tasks

This module retrieves all tasks in your account based on filter settings.

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection</td> 
   <td> <p>For instructions about connecting your CloudConvert account to Workfront Fusion, see <a href="#connect" class="MCXref xref">Connect CloudConvert to Workfront Fusion</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Status </td> 
   <td> <p>Select the task status to filter returned tasks by.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Job ID </td> 
   <td> <p>Enter or map the Job ID to return only tasks within the specified job.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Operation </td> 
   <td> <p>Enter the operation type to return only tasks with the specified operation. </p> <p>Note: Use the List Possible Operations module to retrieve operations.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Limit </td> 
   <td> <p>Enter or map the maximum number of records you want the module to return during each scenario execution cycle.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### Retry a Task

This module creates a new task, based on the settings (payload) of another task.

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection</td> 
   <td> <p>For instructions about connecting your CloudConvert account to Workfront Fusion, see <a href="#connect" class="MCXref xref">Connect CloudConvert to Workfront Fusion</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Task ID</td> 
   <td> <p> Enter or map the ID of the task you want to create a new task from.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Other

* [Get My Info](#get3) 
* [Make an API Call](#make)

#### Get My Info

Retrieves authenticated account details about the current user.

#### Make an API Call

Allows you to perform a custom API call.

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection</td> 
   <td> <p>For instructions about connecting your [Fusion App] account to Workfront Fusion, see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to Workfront Fusion - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">URL</td> 
   <td> <p>Enter a path relative to <code>https://api.cloudconvert.com/</code>. For example: <code>/v2/tasks</code></p> <p>For the list of available endpoints, see the <a href="https://cloudconvert.com/api/v2">CloudConvert API v2 Documentation</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Method</td> 
   <td> <p>Select the HTTP request method you need to configure the API call. For more information, see <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">HTTP request methods</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Headers</td> 
   <td> <p>Add the headers of the request in the form of a standard JSON object.</p> <p>For example, <code>{"Content-type":"application/json"}</code></p> <p>Workfront Fusion 2.0 adds the authorization headers for you.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Query String</td> 
   <td> <p>Add the query for the API call in the form of a standard JSON object.</p> <p>For example: <code>{“name”:“something-urgent”}</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Body</td> 
   <td> <p>Add the body content for the API call in the form of a standard JSON object.When using conditional statements such as <code>if</code> in your JSON, put the quotation marks outside of the conditional statement.<img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"></p> </td> 
  </tr> 
 </tbody> 
</table>

``` ```**Example: **`````` List Tasks

The following API call returns all tasks from your CloudFront account:

URL:
<pre>/v2/tasks</pre>Method:
<pre>GET</pre> ![](assets/cloudconvert-api-example-input.png)

Matches of the search can be found in the module's Output under Bundle > Body > data.

In our example, 6 tasks were returned:

![](assets/cloudconvert-api-example-output.png)

## Troubleshooting

If the CloudConvert > Convert a File throws one of the following errors:

<table cellspacing="0"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p>Error</p> </th> 
   <th>Next steps</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p><span style="font-weight: normal;">The output file size exceeds the limit allowed for your scenario.</span> </p> </td> 
   <td> <p>Please refer to file size limits.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p><span style="font-weight: normal;">You have exceeded the maximum conversion time.</span> </p> </td> 
   <td> <p>The free CloudConvert plan offers 25 conversion minutes daily. If your usage exceeds the limit of the free plan, you may switch to a (prepaid) package or subscription.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p><span style="font-weight: normal;">Failed to read frame size: Could not seek to 1508. �/output/JLIADSA00137P0.mp3: Invalid argument.</span> </p> </td> 
   <td> <p>This error is thrown e.g. when converting files from MP3 to WAV. Make sure that you have selected the correct region because it will find references to files but not only just the correct file.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>RuntimeError: </p> <p><span style="font-weight: normal;">Maximum number of repeats exceeded.</span> </p> </td> 
   <td> <p>Locate the corresponding CloudConvert job in your CloudConvert dashboard's list of jobs and check the job's duration:</p> <p> <img src="assets/cloudconvert-duration-350x177.png" style="width: 350;height: 177;"> </p> <p>The CloudConvert &gt; Convert a File module's timeout is set to 3 minutes. If the job's duration exceeds 3 minutes (possibly due to a temporary overload of the CloudConvert service), the module throws the above mentioned error.</p> <p>In this case consider one of these options:</p> 
    <ul> 
     <li>Enable the <strong>Allow storing of Incomplete Executions</strong> option in the scenario settings to store the incomplete executions for later manual resolution. Optionally you may attach an error handling route to the CloudConvert module with the Break directive to resolve the incomplete executions automatically.</li> 
     <li>Disable the <strong>Download a file option</strong> in the CloudConvert &gt; Convert a file module. In this case the module will not wait for the conversion result. To obtain the conversion result, create a new scenario and use the CloudConvert &gt; New Job Event trigger.</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

``` ```**Example: **`````` Converting a video from MOV to MP4 format

1. Visit [https://cloudconvert.com/video-converter](https://cloudconvert.com/video-converter)
1. Click **Select File** and choose your sample MOV file.
1. Click the dropdown, next to **Convert to** and choose **MP4**.

1. Click the **wrench**icon.
1. Configure the MP4 compression settings as you see fit.
1. Click **Convert**.
1. Once the conversion is complete, click **Download**.
1. Review the converted video.
1. Repeat steps 1 to 8 until you have found the optimal conversion settings for step 5.
1. Visit [https://cloudconvert.com/api/v2/convert#convert-tasks](https://cloudconvert.com/api/v2/convert#convert-tasks)
1. Choose **mov** for the **input_format** field.

1. Choose **mp4**for the **output_format** field.

1. A list of all possible parameters like video_codec, crf, etc. will appear.
1. In Workfront Fusion 2.0, insert the **CloudConvert**> **Convert a File** module in your scenario.

1. Open the module's settings.
1. Configure the module as shown below:

   ![](assets/cloudconvert-mp4-example.png)

1. Make sure to include all the settings in the Conversion and engine specific options field: for each setting from step 5, locate the corresponding parameter from step 13 and its corresponding value.

