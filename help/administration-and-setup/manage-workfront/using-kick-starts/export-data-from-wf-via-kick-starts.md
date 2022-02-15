---
filename: export-data-from-wf-via-kick-starts
user-type: administrator
product-area: system-administration
keywords: kickstart,kick-start,kickstarts,kick-starts
navigation-topic: use-kick-starts
---



# Export data from *`Adobe Workfront`* via Kick-Starts {#export-data-from-adobe-workfront-via-kick-starts}

As an *`Adobe Workfront administrator`*, you can use the Kick-Starts data exporter to export data from *`Workfront`*. You can use it in other applications after you export it.


Exporting data through Kick-Starts is also helpful in understanding what fields are associated with each object, how these fields are coded, as well as how the values of these fields&nbsp;are formatted in the database.


## Access requirements {#access-requirements}

You must have the following to perform the steps in this article:

<table style="width: 100%;margin-left: 0;margin-right: auto;mc-table-style: url('../../../Resources/TableStyles/TableStyle-List-options-in-steps.css');" class="TableStyle-TableStyle-List-options-in-steps" cellspacing="0"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2"> 
 <tbody> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader"><span class="mc-variable WFVariables.FullProdNameWF variable varname">Adobe Workfront</span> plan</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p>Any</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader"><span class="mc-variable WFVariables.FullProdNameWF variable varname">Adobe Workfront</span> license</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray"> <p><span class="mc-variable WFVariables.WFLicense-Plan variable varname">Plan</span> </p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-LightGray" role="rowheader">Access level configurations</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-LightGray"> <p>You must be a <span class="mc-variable WFVariables.AdminWF variable varname">Workfront administrator</span>. For more information, see <a href="grant-a-user-full-administrative-access.md" class="MCXref xref">Grant a user full administrative access</a>.</p> <p>Note: If you still don't have access, ask your <span class="mc-variable WFVariables.AdminWF variable varname">Workfront administrator</span> if they set additional restrictions in your access level. For information on how a <span class="mc-variable WFVariables.AdminWF variable varname">Workfront administrator</span> can modify your access level, see <a href="create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>



## Advantages and disadvantages of using kick-starts to export data {#advantages-and-disadvantages-of-using-kick-starts-to-export-data}

There are two ways to export data within *`Workfront`*:



*  Exporting data from a report or a list


  For more information about exporting data from a report or a list, see [Export data](export-data.md).

* Exporting data via kick-starts


The following table shows the advantages and disadvantages of each method:&nbsp;

<table style="mc-table-style: url('../../../Resources/TableStyles/TableStyle-HeaderRow.css');margin-left: 0;margin-right: auto;width: 100%;" class="TableStyle-TableStyle-HeaderRow" cellspacing="15"> 
 <col class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <col class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <col class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <thead> 
  <tr class="TableStyle-TableStyle-HeaderRow-Head-Header1"> 
   <th class="TableStyle-TableStyle-HeaderRow-HeadE-Column1-Header1"> <p>&nbsp;</p> </th> 
   <th class="TableStyle-TableStyle-HeaderRow-HeadE-Column1-Header1"> <p>Exported Data Includes Object and Field Values</p> </th> 
   <th class="TableStyle-TableStyle-HeaderRow-HeadD-Column1-Header1"> <p>Ability to Export Data around Multiple Object Types Simultaneously</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"> <p><span class="bold">Exporting Data from a List View</span> </p> <p>For more information about exporting data from a list, see <a href="export-data.md" class="MCXref xref">Export data</a></p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"> <p>Yes</p> <p>Both <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span> native fields and custom fields associated with the objects are exported.</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p>No</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyB-Column1-MediumGray"> <p><span class="bold">Exporting Data via Kick-Starts</span> </p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyB-Column1-MediumGray"> <p>Yes (limited)</p> <p>Most <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span> native fields associated with objects are exported, but some are not. For example, you cannot export the Schedule, Project Owner, or Project Sponsor fields through a project kick-start export.</p> <p>In a project that has a custom form attached, any data entered in the fields on the form is not exported.</p> <p>But you can export a custom form. The resulting file lists the fields configured in the form, such as text boxes and radio buttons.</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyA-Column1-MediumGray"> <p>Yes</p> <p>Using Kick-Starts to export <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span> data&nbsp;enables you to export data related to multiple object types in a single export. For example, you can include tasks, issues, and projects in a single export.</p> </td> 
  </tr> 
 </tbody> 
</table>



## Export limits {#export-limits}

The following limitations exist&nbsp;when exporting data via kick-starts (data is exported in an Excel file format):&nbsp;



* `50,000 rows:`&nbsp;The number of rows allowed in the file.
* `65,530 hyperlinks:`&nbsp;This is a limit imposed by Excel on documents that contain more than 65,530 hyperlinks. These documents cannot be opened after they are exported. Note that an Excel document may have just 200 rows of data, but if there are more than 65,530 links inside the document, the document does not open.




## Export data via kick-starts {#export-data-via-kick-starts}




1. Click `Setup` near the upper-right corner of *`Adobe Workfront`* on the Global Navigation Bar.

1. Click `System` > `Kick-Starts,` then click `Export Data.`

1. Select the object&nbsp;you want to export.
1.  Click `More Options`&nbsp;to see the full list of objects.


   All of the objects listed here can be used to also import data into *`Workfront`*. 


   The only exception is the `Access Levels` object. The Access Levels data sheet that is included in an export is provided for reference purposes only. It allows you to assign an access level to a new user account by ID. 


   For more information about importing data into *`Workfront`* via kick-starts, see [Import data into Adobe Workfront via a Kick-Start template](import-data-via-kickstarts.md)The following is a list of all objects that can be exported through kick-starts:

<table style="height: 748px;mc-table-style: url('../../../Resources/TableStyles/TableStyle-HeaderRow.css');width: 100%;margin-left: 0;margin-right: auto;" cellspacing="15" class="TableStyle-TableStyle-HeaderRow"> 
 <col class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <col class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <col class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <thead> 
  <tr class="TableStyle-TableStyle-HeaderRow-Head-Header1"> 
   <th class="TableStyle-TableStyle-HeaderRow-HeadE-Column1-Header1"> <p>Object</p> </th> 
   <th class="TableStyle-TableStyle-HeaderRow-HeadE-Column1-Header1"> <p>Exported Sheets of the Excel File</p> </th> 
   <th class="TableStyle-TableStyle-HeaderRow-HeadD-Column1-Header1"> <p>Export Format</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td scope="col" valign="top" class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">Access Level</td> 
   <td scope="col" valign="top" class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">Access Level<br>Preferences</td> 
   <td scope="col" valign="top" class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray">Exports as Excel file.</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td scope="col" valign="top" class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">Assignment</td> 
   <td scope="col" valign="top" class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">Assignment<br>Preferences</td> 
   <td scope="col" valign="top" class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray">Exports as Excel file.</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td scope="col" valign="top" class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">Company</td> 
   <td scope="col" valign="top" class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"> Company<br>Preferences </td> 
   <td scope="col" valign="top" class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray">Exports as Excel file.</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td scope="col" valign="top" class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">Email Template</td> 
   <td scope="col" valign="top" class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"> Email Template<br>Preferences </td> 
   <td scope="col" valign="top" class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray">Exports as Excel file.</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td scope="col" valign="top" class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">Expense</td> 
   <td valign="top" class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"> Expense<br>Preferences </td> 
   <td scope="col" valign="top" class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray">&nbsp;Exports as Excel file.</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td valign="top" class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">External Page</td> 
   <td valign="top" class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"> External Page<br>Preferences </td> 
   <td scope="col" valign="top" class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray">Exports as Excel file.</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td valign="top" class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">Filter</td> 
   <td valign="top" class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"> Filter<br>Preferences </td> 
   <td valign="top" class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray">Exports as a .zip file.&nbsp;</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td valign="top" class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">Group</td> 
   <td valign="top" class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"> Group<br>Preferences&nbsp; </td> 
   <td valign="top" class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray">Exports as Excel file.</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td valign="top" class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">Grouping</td> 
   <td valign="top" class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"> Grouping<br>Preferences </td> 
   <td valign="top" class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray">Exports as a .zip file.</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td valign="top" class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">Hour</td> 
   <td valign="top" class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"> Hour<br>Preferences </td> 
   <td valign="top" class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray">Exports as Excel file.</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td valign="top" class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">Issue</td> 
   <td valign="top" class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"> Issue<br>Preferences </td> 
   <td valign="top" class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray">Exports as Excel file.</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td valign="top" class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">Job Role</td> 
   <td valign="top" class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"> Job role<br>Preferences </td> 
   <td valign="top" class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray">Exports as Excel file.</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td valign="top" class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">Milestone Path</td> 
   <td valign="top" class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"> Milestone<br>Milestone Path<br>Preferences </td> 
   <td valign="top" class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> Exports as Excel file.&nbsp;</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td valign="top" class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">Note</td> 
   <td valign="top" class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"> Note<br>Preferences </td> 
   <td valign="top" class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray">Exports as Excel file.</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td valign="top" class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">Portfolio</td> 
   <td valign="top" class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"> Portfolio<br>Preferences&nbsp; </td> 
   <td valign="top" class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray">Exports as Excel file.</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td valign="top" class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">Project</td> 
   <td valign="top" class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"> Queue<br>Project<br>Routing Rule<br>Queue Topic<br>Preferences </td> 
   <td valign="top" class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray">&nbsp;Exports as Excel file.</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td valign="top" class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">Resource Estimate</td> 
   <td valign="top" class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"> Resource Estimate<br>Preferences </td> 
   <td valign="top" class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray">Exports as Excel file.</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td valign="top" class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">Resource Pool</td> 
   <td valign="top" class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"> Resource Pool<br>Preferences </td> 
   <td valign="top" class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray">Exports as Excel file.</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td valign="top" class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">Risk</td> 
   <td valign="top" class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"> Risk<br>Preferences&nbsp; </td> 
   <td valign="top" class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray">Exports as Excel file.</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td valign="top" class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">Risk Type</td> 
   <td valign="top" class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"> Risk Type<br>Preferences&nbsp; </td> 
   <td valign="top" class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> Exports as Excel file.&nbsp;</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td valign="top" class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">Scorecard</td> 
   <td valign="top" class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">Scorecard Questions<br>Scorecard Option<br>Scorecard<br>Preferences&nbsp;</td> 
   <td valign="top" class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray">Exports as Excel file.&nbsp;</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td valign="top" class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">Task</td> 
   <td valign="top" class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"> Task<br>Preferences </td> 
   <td valign="top" class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray">Exports as Excel file.&nbsp;</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td valign="top" class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">Template</td> 
   <td valign="top" class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"> Queue<br>Template<br>Routing Rule<br>Queue Topic<br>Preferences </td> 
   <td valign="top" class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> Exports as Excel file.&nbsp;&nbsp;</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td valign="top" class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">Template Assignment</td> 
   <td valign="top" class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"> Template Assignment<br>Preferences </td> 
   <td valign="top" class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray">Exports as Excel file.&nbsp;</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td valign="top" class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">Template Task</td> 
   <td valign="top" class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"> Template Task<br>Preferences </td> 
   <td valign="top" class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray">Exports as Excel file.&nbsp;</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td valign="top" class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">Timesheet</td> 
   <td valign="top" class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"> Timesheet Profile<br>Timesheet<br>Preferences </td> 
   <td valign="top" class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> Exports as Excel file.&nbsp;&nbsp;</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td valign="top" class="TableStyle-TableStyle-HeaderRow-BodyB-Column1-LightGray">&nbsp;View </td> 
   <td valign="top" class="TableStyle-TableStyle-HeaderRow-BodyB-Column1-LightGray"> View<br>Preferences&nbsp; </td> 
   <td valign="top" class="TableStyle-TableStyle-HeaderRow-BodyA-Column1-LightGray">Exports as .zip file.</td> 
  </tr> 
 </tbody> 
</table>


1.  Click `Download.`


   The exported kick-start file is downloaded to your computer either as an Excel file, or a . zip file containing multiple Excel and properties files. Each Excel file is a collection of sheets, where each sheet represents a field associated with the object you selected. There is a `Properties` sheet associated with every export.


   The `Dashboard` and `Report`&nbsp;options allow you to select specific dashboards and reports to include in the download. You can export only&nbsp;Dashboards which are shared system-wide.


   You cannot export matrix reports. For more information about matrix reports, see [Create a matrix report](create-matrix-report.md).


   You can select up to 100 Dashboards and 100 Reports in a single export.


   ![](assets/kickstart-export-350x381.png)




   You can export multiple objects at one time.


   By default, the following objects are displayed under the `What to include` label (prior to clicking `More Options`):

<table style="mc-table-style: url('../../../Resources/TableStyles/TableStyle-HeaderRow.css');margin-left: 0;margin-right: auto;width: 100%;" class="TableStyle-TableStyle-HeaderRow" cellspacing="15"> 
 <col class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <col class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <col class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <thead> 
  <tr class="TableStyle-TableStyle-HeaderRow-Head-Header1"> 
   <th class="TableStyle-TableStyle-HeaderRow-HeadE-Column1-Header1"> <p><span class="bold">Object</span> </p> </th> 
   <th class="TableStyle-TableStyle-HeaderRow-HeadE-Column1-Header1"> <p><span class="bold">Exported Sheets of the Excel File</span> </p> </th> 
   <th class="TableStyle-TableStyle-HeaderRow-HeadD-Column1-Header1"> <p>&nbsp;<span class="bold">Export Format</span></p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td scope="col" valign="top" class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"> <p>Dashboard</p> <p>&nbsp;</p> <p>&nbsp;</p> </td> 
   <td scope="col" valign="top" class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"> <p>Parameter<br>Parameter Option<br>Parameter Group<br>Category Parameter<br>Category<br>Report<br>Portal Tab Section<br>Dashboard<br>Preferences<br></p> </td> 
   <td scope="col" valign="top" class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray">&nbsp;Exports as .zip file.</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td scope="col" valign="top" class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"> <p>Report</p> <p>&nbsp;</p> <p>&nbsp;</p> </td> 
   <td scope="col" valign="top" class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">Parameter<br>Parameter Option<br>Parameter Group<br>Category Parameter<br>Category<br>Report<br>Preferences</td> 
   <td scope="col" valign="top" class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray">&nbsp;Exports as .zip file. </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td scope="col" valign="top" class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"> <p>Approval</p> </td> 
   <td scope="col" valign="top" class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"> <p>Step Approver<br>Approval Step<br>Approval<br>Approval Process<br>Preferences</p> </td> 
   <td scope="col" valign="top" class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p>&nbsp;Exports as Excel file.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td scope="col" valign="top" class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"> <p>Custom Data</p> </td> 
   <td scope="col" valign="top" class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"> <p>Parameter<br>Parameter Option<br>Parameter Group<br>Category Parameter<br>Category<br>Preferences</p> </td> 
   <td scope="col" valign="top" class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> <p>&nbsp;Exports as Excel file.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td scope="col" valign="top" class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"> <p>Expense Type</p> </td> 
   <td valign="top" class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"> <p>Expense Type<br>Preferences</p> </td> 
   <td scope="col" valign="top" class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p>Exports as Excel file.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td valign="top" class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"> <p>Hour Type</p> </td> 
   <td valign="top" class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"> <p>Hour Type<br>Preferences</p> </td> 
   <td scope="col" valign="top" class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> <p>Exports as Excel file.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td valign="top" class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"> <p>Team</p> </td> 
   <td valign="top" class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"> Team Member<br>Team<br>Preferences </td> 
   <td scope="col" valign="top" class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p>&nbsp;Exports as Excel file.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td valign="top" class="TableStyle-TableStyle-HeaderRow-BodyB-Column1-MediumGray"> <p>User</p> </td> 
   <td valign="top" class="TableStyle-TableStyle-HeaderRow-BodyB-Column1-MediumGray"> <p>User<br>Preferences</p> </td> 
   <td valign="top" class="TableStyle-TableStyle-HeaderRow-BodyA-Column1-MediumGray"> <p>&nbsp;Exports as Excel file.</p> </td> 
  </tr> 
 </tbody> 
</table>


<table style="mc-table-style: url('../../../Resources/TableStyles/TableStyle-HeaderRow.css');margin-left: 0;margin-right: auto;width: 100%;" class="TableStyle-TableStyle-HeaderRow" cellspacing="15"> 
 <col class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <col class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <col class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <thead> 
  <tr class="TableStyle-TableStyle-HeaderRow-Head-Header1"> 
   <th class="TableStyle-TableStyle-HeaderRow-HeadE-Column1-Header1"> <p><span class="bold">&nbsp;</span> </p> </th> 
   <th class="TableStyle-TableStyle-HeaderRow-HeadE-Column1-Header1"> <p><span class="bold">Exported Sheets of the Excel File</span> </p> </th> 
   <th class="TableStyle-TableStyle-HeaderRow-HeadD-Column1-Header1"> <p>&nbsp;<span class="bold">Export Format</span></p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td scope="col" valign="top" class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"> <p>Dashboard</p> <p>&nbsp;</p> <p>&nbsp;</p> </td> 
   <td scope="col" valign="top" class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"> <p>Parameter<br>Parameter Option<br>Parameter Group<br>Category Parameter<br>Category<br>Report<br>Portal Tab Section<br>Dashboard<br>Preferences<br></p> </td> 
   <td scope="col" valign="top" class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray">&nbsp;Exports as .zip file.</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td scope="col" valign="top" class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"> <p>Report</p> <p>&nbsp;</p> <p>&nbsp;</p> </td> 
   <td scope="col" valign="top" class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">Parameter<br>Parameter Option<br>Parameter Group<br>Category Parameter<br>Category<br>Report<br>Preferences</td> 
   <td scope="col" valign="top" class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray">&nbsp;Exports as .zip file. </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td scope="col" valign="top" class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"> <p>Approval</p> </td> 
   <td scope="col" valign="top" class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"> <p>Step Approver<br>Approval Step<br>Approval<br>Approval Process<br>Preferences</p> </td> 
   <td scope="col" valign="top" class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p>&nbsp;Exports as Excel file.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td scope="col" valign="top" class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"> <p>Custom Data</p> </td> 
   <td scope="col" valign="top" class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"> <p>Parameter<br>Parameter Option<br>Parameter Group<br>Category Parameter<br>Category<br>Preferences</p> </td> 
   <td scope="col" valign="top" class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> <p>&nbsp;Exports as Excel file.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td scope="col" valign="top" class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"> <p>Expense Type</p> </td> 
   <td valign="top" class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"> <p>Expense Type<br>Preferences</p> </td> 
   <td scope="col" valign="top" class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p>Exports as Excel file.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td valign="top" class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"> <p>Hour Type</p> </td> 
   <td valign="top" class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"> <p>Hour Type<br>Preferences</p> </td> 
   <td scope="col" valign="top" class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> <p>Exports as Excel file.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td valign="top" class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"> <p>Team</p> </td> 
   <td valign="top" class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"> Team Member<br>Team<br>Preferences </td> 
   <td scope="col" valign="top" class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> <p>&nbsp;Exports as Excel file.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td valign="top" class="TableStyle-TableStyle-HeaderRow-BodyB-Column1-MediumGray"> <p>User</p> </td> 
   <td valign="top" class="TableStyle-TableStyle-HeaderRow-BodyB-Column1-MediumGray"> <p>User<br>Preferences</p> </td> 
   <td valign="top" class="TableStyle-TableStyle-HeaderRow-BodyA-Column1-MediumGray"> <p>&nbsp;Exports as Excel file.</p> </td> 
  </tr> 
 </tbody> 
</table>


1.  (Recommended) Analyze the exported data to ensure that all the information you expect to see was exported.&nbsp;


   For large exports, *`Workfront`* works in the background to produce the Excel file and gives you a warning message about the delay. The kick-start file is emailed to you, when the download finishes.


   ![](assets/large-kick-start-file-warning-350x65.png)





