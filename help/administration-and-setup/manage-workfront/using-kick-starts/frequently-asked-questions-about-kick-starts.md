---
filename: frequently-asked-questions-about-kick-starts
user-type: administrator
content-type: faq
product-area: system-administration
keywords: kickstart,kick-start,kickstarts,kick-starts
navigation-topic: use-kick-starts
---



# Frequently asked questions about Kick-Starts {#frequently-asked-questions-about-kick-starts}

The following are frequently asked questions about Kick-Starts:


## Why am I receiving this error when trying to import a Kick-Start file: "Your file was correct, but nothing was imported?" {#why-am-i-receiving-this-error-when-trying-to-import-a-kick-start-file-your-file-was-correct-but-nothing-was-imported}



### Answer {#answer}

One of the following three things might be missing from the Kick-Start file:



1. The `isNew` column must be set to `TRUE` for all the items you want to import. `isNew` must be `TRUE`because you can only import new data with a Kick-Start. You cannot Modify existing data via Kick-Start. You can have other rows in the spreadsheet with  `isNew = FALSE` but, these rows will not import.

1. ​The file needs to have one empty&nbsp;row before the headers of your data start.
1. ​The Excel sheet(s) need(s) to have the correct name(s).


When working with Kick-Starts, we recommend to first download the Kick-start Template, manually populate it with the correct data and then import it back into *`Adobe Workfront`*.


For more information about correctly importing data in *`Workfront`* using Kick-Starts, see [Import data into Adobe Workfront via a Kick-Start template](import-data-via-kickstarts.md).


## Why am I receiving this error when trying to import hours into *`Workfront`* using a Kick-Start file: "User with primary key value(s) "null" not found?" {#why-am-i-receiving-this-error-when-trying-to-import-hours-into-workfront-using-a-kick-start-file-user-with-primary-key-value-s-null-not-found}



### Answer {#answer-1}

The error refers to the GUID of the user that is associated with the hours.&nbsp;


To address this:



1. Export a blank Kick-Start template for the `Hours` object only.  
   For more information about exporting a blank Kick-Start File, see "Exporting the Kick-Start Template" in&nbsp; [Import data into Adobe Workfront via a Kick-Start template](import-data-via-kickstarts.md).

1. Manually copy the data from the original Kick-Start and paste it into the empty file.  
   Do this for each column.
1. Try importing the new file again.  
   The Kick-Start should import successfully.


