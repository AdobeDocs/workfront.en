

# Export report information in the `Reporting Canvas`

You can export an entire report from `Adobe Workfront`, or you can export only the table or visualization you need from a report.

You can export to:

* CSV
* PDF

  <!--
  PNG
  -->

* XLSX

## Access requirements

You must have the following access to perform the steps in this article:

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><span>Adobe Workfront</span> plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><span>Workfront</span> license*</td> 
   <td> <p>Plan</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to create reports, calendars, and dashboards</p> <p>Note: If you still don't have access, ask your <span>Workfront administrator</span> if they set additional restrictions in your access level. For information on how a <span>Workfront administrator</span> can modify your access level, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> Object permissions Manage access to the report For information on requesting additional access, see Request access to objects in Adobe Workfront. 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your `Workfront administrator`.

<!--
Find out if the Object permissions info is correct here ^
-->

## Prerequisites

Before you begin, you must enroll in the `Reporting Canvas` beta program.

<!--
For more information, see [link to Beta enrollment info].
-->

## Export a report

<ol> 
 <li value="1"> <p>Go to the report that you want to export.</p> </li> 
 <li value="2"> <p>In the report header, click the <span class="bold">More</span> icon <img src="assets/more-icon.png">, select <span class="bold">Export</span>, then select the file format you want.</p> </li> 
 <li value="3"> <p>(Conditional) If you selected <span class="bold">PDF</span>, configure the fields below to format the exported file, then click <span class="bold">Download PDF</span>.</p> 
  <table cellspacing="0"> 
   <col> 
   <col> 
   <tbody> 
    <tr> 
     <td role="rowheader">Document size</td> 
     <td> <p>Select the document size for the exported file.</p> </td> 
    </tr> 
    <tr> 
     <td role="rowheader">Orientation</td> 
     <td> <p>Select <span class="bold">Portrait</span> or <span class="bold">Landscape</span>.</p> </td> 
    </tr> 
    <tr> 
     <td role="rowheader">Scaling options</td> 
     <td> <p>Select the scaling option for the exported file:</p> 
      <ul> 
       <li> <p><span class="bold">Normal</span> (default option)</p> </li> 
       <li> <p><span class="bold">Fit to width</span> </p> </li> 
       <li> <p><span class="bold">Fit to height</span> </p> </li> 
      </ul> </td> 
    </tr> 
    <tr> 
     <td role="rowheader">Heading settings</td> 
     <td> <p>Select what you want to display in the header.</p> </td> 
    </tr> 
    <tr> 
     <td role="rowheader">Footer settings</td> 
     <td> <p>Select what you want to display in the footer.</p> <p>If you select <span class="bold">Footer message</span>, type the <span class="bold">Footer text</span> that you want to display. You can type up to 255 characters.</p> </td> 
    </tr> 
    <tr> 
     <td role="rowheader">Watermark</td> 
     <td> <p>If you select <span class="bold">Include watermark</span>, do any of the following:</p> 
      <ul> 
       <li>Type the <span class="bold">Watermark text</span> that you want to display. You can type up to 20 characters.</li> 
       <li>Slide the <span class="bold">Opacity</span> to the percentage that you want for the text.</li> 
       <li>Enter the degree of <span class="bold">Rotation</span> that you want for the text.</li> 
      </ul> </td> 
    </tr> 
   </tbody> 
  </table> <p>The PDF preview in the right pane updates as you configure each field.</p> <p>The exported file downloads in the following format: REPORT_TITLE_YYYY-MM-DDTHH_MM_SS.</p> <note type="note"> 
   <p>Consider the following for your exported file:</p> 
   <ul> 
    <li> <p>If you export a report that contains multiple tables to an XLSX format, the exported file has a separate sheet for each table.</p> </li> 
    <li> <p>If you export a report that contains multiple tables to a CSV format, the exported file is a zipped file that contains a separate file for each table.</p> </li> 
    <li> <p>If you export a table that contains grouped rows to a CSV format, the CSV file includes all of the rows, but they are not displayed in groups.</p> </li> 
   </ul> 
  </note> </li> 
</ol>

