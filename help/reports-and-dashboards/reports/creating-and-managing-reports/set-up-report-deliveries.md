---
filename: set-up-report-deliveries
product-area: reporting;setup
navigation-topic: create-and-manage-reports
---



# Report delivery overview {#report-delivery-overview}

You can schedule reports to be automatically delivered to users on a defined schedule, or you can send reports on one-time basis, manually. When you send a report from *`Adobe Workfront`*, the user receives an email with the *`Workfront`* report in a separate attachment.


For information about setting up a report for delivery, see the article [Schedule an automatic report delivery](set-up-automatic-report-delivery.md).


You cannot schedule reports for delivery, nor deliver them manually in the Preview Sandbox environment. For more information about the Preview Sandbox, see the article [The Adobe Workfront Preview Sandbox Environment](wf-preview-sandbox-environment.md).  
For more information about delivering reports in the Preview Sandbox environment, see the article [Send a report in the Preview Sandbox environment](send-report-preview-sandbox-environment.md).


## Report delivery limits {#report-delivery-limits}

Consider the following when scheduling reports for delivery: 



* You can schedule up to 10 repeating report deliveries for any given report.
* You can schedule a report to be delivered only if you are the creator of the report. If you need to send a report that you did not create, you can send it on a manual basis.




## Export limits {#export-limits}

There are several size limits that affect how reports display in *`Workfront`* and how they export through a manual export, a delivered report, or through the API:



* `5MB file size:`&nbsp;File size limit for any exported report scheduled for delivery.&nbsp;If an exported file attached to an email is larger than 5MB, a link where the file can be downloaded is emailed instead of the attached exported report.&nbsp;





*  `50,000 rows:`&nbsp;The number of rows of data allowed in a report export for .pdf and Tab Delimited files.   



  For Excel .xls files, this limit is `65,000 rows`.  



  For Excel .xlsx files, this limit is `100,000 rows`.  



  These limits exclude the column headings, as well as rows for groupings in the report. For instance, if you have 6 groupings in a report, and 50,000&nbsp;rows or data, the exported file will have 50,000&nbsp;rows. 


  If your report has more items than these limits, you receive an error that the export and delivery of the report is not successful. Reduce the number of items you see on the screen to a number less than or equal to these limits to be able to deliver the results.&nbsp;If want to export all the data, we suggest that you use filters to obtain smaller loads&nbsp;of data, then perform multiple exports. For more information, see [Filters overview in Adobe Workfront](filters-overview.md).


  These limits apply to:

*  `<li>A manual export of a report.</li>` `<li>A scheduled report.</li>` `<li>An export through an API integration.&nbsp;</li>` `<li> <p>Data exported through a kick-start.</p> <p>For more information about exporting data via kick-starts, see the article <a href="export-data-from-wf-via-kick-starts.md" class="MCXref xref">Export data from Adobe Workfront via Kick-Starts</a>.</p> <note type="note">  You can export 50,000 rows in a kick-start file, but only to an Excel format file.&nbsp; </note> </li>` `<li> <p>Exporting utilization information for a project.</p> <p>For more information about exporting utilization information for a project, see <a href="resource-utilization-report.md" class="MCXref xref">Overview of the Resource Utilization report</a>.</p> </li>` 

* `65,530 hyperlinks:`&nbsp;This is a limit imposed by Excel on documents that contain more than 65,530 hyperlinks. These documents cannot be opened when they are exported manually, or sent in a delivered report. Note that an Excel document may have just 200 rows of data, but if there are more than 65,530 links inside the document, the document does not open. This limit exists on Excel files only, not on the other supported formats.&nbsp;
* `256 columns`:&nbsp;This is a limit imposed by Excel on documents that contain more than 256 columns. These documents cannot be exported manually, or sent in a delivered report. This limit exists on Excel files only, not on the other supported formats.&nbsp;


If you&nbsp;attempt to export data beyond the limit, you might&nbsp;not receive all of the expected data in the export. Rather, a modified report is produced within the limit.&nbsp;


Additionally, reports that take longer than 60 minutes to run will be halted.


If you have concerns or issues regarding your limit, please contact *`Workfront`* Technical Support.


## Understand time stamps on delivered reports {#understand-time-stamps-on-delivered-reports}

When receiving a report in an email, the time stamp and time format on the report might not match those in *`Workfront`*, if you were to view the report in *`Workfront`* at the same time that it was delivered.&nbsp;


Consider the following:&nbsp;



* When viewing a report in the browser, the time stamp and format on the report matches the&nbsp;locale and the time zone of your browser, as defined in the settings of your browser.
* When the report is delivered in an email, the report is delivered with the time stamp and format that matches the User Locale and Time Zone as they are specified in your *`Workfront`* profile.   
  For more information about the User Locale and Time Zone in *`Workfront`*, see the article [Edit a user's profile](edit-a-users-profile.md).





## Reports with a special view {#reports-with-a-special-view}

When you apply a special view to a report, the special view displays in of the Details tab of the report in  *`Workfront`*.


When you schedule the delivery of a report that has a special view, the default Details tab is delivered in the attachment of the sent email, instead of the special view.


The following are considered special views:



* Milestone view on a Project report
* Gantt View on a Project or Task report
* Reports with a Chart as the default tab




>[!NOTE]
>
>If there is also a Matrix tab on the report in addition to the default tab with a special view, the report is delivered as it displays on the Matrix tab.


For more information about how to apply a special view to a report, see the article [Create a custom report](create-custom-report.md).


## Use the delivered file {#use-the-delivered-file}

When you send a report from *`Workfront`*, the user receives an email with the report in a separate attachment.&nbsp;



* [Subject line, attachment name, and report title](#file-names-and-titles) 
* [Timestamps](#timestamps) 
* [Branding](#branding) 
* [Formatting](#formatting) 
* [Links](#links) 




### Subject line, attachment name, and report title {#subject-line-attachment-name-and-report-title}

For more information about the subject line of the delivered report email, see [Schedule an automatic report delivery](set-up-automatic-report-delivery.md).


The name of the attached report is: *The_Name_Of_The_Report*followed by the exported file format.&nbsp; 


If you scheduled the delivered report to be formatted as a PDF or an HTML file, the title of the report will be:


*The Name of the Report.* 


Reports scheduled to be delivered in an Excel, Excel (.xlsx), or TSV format do not have a title.


>[!NOTE]
>
>If the report has a description, it will be included in the exported file, if the file is formatted as a PDF or an HTML file.




### Timestamps {#timestamps}

A timestamp is displayed on the attached file only if the format of the file is a .pdf. The timestamp is in the footer of the attached file. 


The timestamp includes: 



* Date
* Time
* Time zone when the report was sent




### Branding {#branding}

If your *`Workfront administrator`* has added customized branding to your *`Workfront`* instance, the reports sent in .pdf format also include your personalized logo. 


Reports sent in all other formats cannot be personalized with your logo. 


For more information about branding your *`Workfront`* instance, see the article [Brand your Adobe Workfront instance](brand-your-workfront-instance.md).


### Formatting {#formatting}

You always receive the default tab of a report when a report is sent or scheduled for a delivery, unless the report has a special view. 


If your report has special formatting in the web application, the report should be delivered with the special formatting when the Details and the Matrix tabs are delivered for .pdf and Excel files only. 


The filter, view, or grouping of the report are not included in the delivered file. The description of the report is included only when you send the report as a PDF file. 


For more information about receiving reports with a special view, see the article [Reports with a special view](#sending-reports-with-a-special-view).  
For more information about selecting the default tab of a report and about special formatting, see [Create a custom report](create-custom-report.md).


### Links {#links}

When you send a report from *`Workfront`* to PDF or Excel format, any working links that exist in the original document remain live in the sent file. Links can point to any object in *`Workfront`* that supports linking.


The name of the report in the email message is also a link.


## Report on scheduled reports {#report-on-scheduled-reports}

You can see whether a report has been configured to be delivered by creating the following:



* `A View` for the Report object in a list or a report for reports: Create a view on a list of reports or in a report for reports, and add the following column to the view:  
  *Scheduled Report Name.  
  *The names of all the deliveries scheduled for that report are listed in the column in a bulleted list.  
  ![scheduled_reports_info_in_view.png](assets/scheduled-reports-info-in-view-350x294.png)  

* `A Filter` for the Report object:&nbsp;Create a filter on a list of reports or in a report on reports with the following statement: *Scheduled Report ID Is Not Blank*.  
  This will display only reports that have been scheduled in your list or report.  
  ![](assets/qs-scheduled-report-filter-350x101.png)  
  For more information about creating reports, see [Create a custom report](create-custom-report.md). For information on creating a report on reports, see [Create a report on reporting activities](create-report-reporting-activities.md).



