



# Restore data {#restore-data}

This document describes the process for recovering objects that have been deleted from your `Workfront` Production or Preview&nbsp;environments. 


Projects, tasks, issues, and documents can be restored by a  `Workfront administrator` of each `Workfront` instance, while separate hours, notes, and custom forms can be restored only by the `Workfront` Database Team. 


>[!NOTE]
>
>`Workfront` keeps the deleted information for up to 30 days from the date it was deleted, both for the purpose of restoring it by the `Workfront administrator`&nbsp;or by the Database Team. Anything deleted longer than 30 days before the restore is requested is no longer available.&nbsp;




## Restore deleted projects, tasks, issues, and documents {#restore-deleted-projects-tasks-issues-and-documents}

As a `Workfront administrator` for your `Workfront` instance, you can restore projects, tasks, issues, and documents that have been deleted from your `Workfront` Production or Preview environments up to 30 days after the object was deleted.&nbsp; 


Objects and fields attached to the object deleted will also be restored. For example, if you restore a project, all tasks, issues, documents, hours, notes, assignments, and custom data are also restored.&nbsp; 


For information about how to restore projects, tasks, issues, and documents, see [Restore deleted items](restore-deleted-items.md).


## Restore individual&nbsp;items {#restore-individual-items}

Only the `Workfront` Database Team can restore individual&nbsp;items.


The following are examples of individual&nbsp;items that might need to be restored independently of the parent that was deleted with them:



* Tasks
* Issues
* Documents
* Custom Forms
* Hours
* Notes


The following sections describe the process of restoring documents and custom forms:



* [Take immediate action](#immediate-action-items) 
* [Information needed for a data restore](#information-needed-for-a-data-restore) 
* [Data restore process](#data-restore-process) 




### Take immediate action {#take-immediate-action}

Data from your live environment is available in the Preview Sandbox for up to 7&nbsp;days. This means you can export the standalone data from the Preview Sandbox environment using the following methods: 



*  Kick-Starts 
*  Building a report and exporting the results  


For more information about exporting data from `Workfront`, see [Export data](export-data.md).


You can import the exported data in the following ways: 



*  Manually, if you are using exported reports 
*  In bulk, if you are using Kick-Starts  
  For more information about importing data into `Workfront` using Kick-Starts, see [Import data into Workfront via Kick-Starts](import-data-via-kickstarts.md).



The Preview Sandbox environment is refreshed during our maintenance windows over the weekend.   
For more information about the windows of maintenance for the Preview Sandbox environment, see [trust.workfront.com](https://trust.workfront.com/).


>[!IMPORTANT] {type="important"}
>
>Documents are an exception to these methods of restoration. You can manually download them from the Preview Environment, and re-upload them into the Production environment. If you want to download and upload documents in bulk, you will need to request a data restore from `Workfront`.&nbsp;




### Information needed for a data restore {#information-needed-for-a-data-restore}

Once you have determined a deleted object needs restoring by our Database Team, you will want to gather as much information as you have about it. The following information is required for our database administrators to find the object and initiate a restore: 



*  Object name 
*  Object Type (Task, Issue, Project, etc) 
*  Estimated Date and Time of deletion 
*  Object GUID (if possible)  
  Refer to the following information when locating the GUID of an object: 
*  `<li value="1"> The GUID can be found by referencing e-mail notifications triggered by interacting with the object (assignments to, comments on, etc.) </li>` `<li value="2"> Example of a GUID found at the end of a URL: yourdomain.my.workfront.com/issue/view?ID=568bfa96011220154c8ca4c4e691556b </li>` 



Once you have gathered this information or if you require assistance, please call our Customer Support Team&nbsp;at 844-306-HELP(4357) or submit a ticket online. 


### Data restore process {#data-restore-process}




1.  After our Customer Support Team receives your information, they will escalate it to our Customer Support Team. 
1.  Our Customer Support Team will contact our&nbsp;Database Team.
1.  Once the Database Team has had a chance to review the data being restored, a more accurate estimate for the ETA can be provided. A restore will generally take three days but can take longer depending on the type and volume of data being restored. 
1.  The Database Team will restore the information to your Preview Sandbox environment where you will have the chance to review the restored data. Our Customer Support Team will let you know when the data can be found&nbsp;in the Preview Sandbox. 
1.  Once you are satisfied with the restore in the sandbox, let our Customer Support Team know &nbsp;and they will contact our&nbsp;Database Team to notify them that they can restore the data to your production environment. 
1.  You will have a chance to review the restored data before the request is closed. 


