---
content-type: tips-tricks-troubleshooting
product-area: timesheets
navigation-topic: tips-tricks-and-troubleshooting-timesheets
title: Track Hour Records with the Adobe Workfront API
description: If your organization uses Adobe Workfront to enter hours worked, but uses another tool as the system of record for that data, you can use the Workfront API to synchronize data between the two systems.
author: Lisa
feature: Timesheets
exl-id: b26f8156-f9dc-43e7-8e0d-8c0905dc7a12
---
# Track Hour Records with the Adobe Workfront API

If your organization uses Adobe Workfront to enter hours worked,&nbsp;but uses another tool as the system of record for that data, you can use the Workfront API to synchronize data between the two systems.

Simply tracking the hour record is not feasible because, if the hour entry is removed, the entire record is deleted, requiring you to pull the entire dataset and compare it to the old dataset. Fortunately, all hour transactions are recorded in Workfront Journal Entries.

After retrieving an initial set of all the current hours in the system, you can track any and all changes through the Journal Entries.
<pre>GET /attask/api/v5.0/JRNLE/search?subObjCode=HOUR&fields=changeType,aux2,newNumberVal,oldNumberVal,subObjCode,subObjID</pre><pre>{<br>"data": [<br>{<br>"ID": "5785406d008d93dd35665f14d90d4929",<br>"objCode": "JRNLE",<br>"changeType": "A",<br>"aux2": "Brad Littler",<br>"newNumberVal": 1,<br>"oldNumberVal": null,<br>"subObjCode": "HOUR",<br>"subObjID": "5785406d008d93dce3f7f2e0e8eda4ea"<br>},<br>{<br>"ID": "57854124008da2b9f372c01f8b9054bf",<br>"objCode": "JRNLE",<br>"changeType": "D",<br>"aux2": "Brad Littler",<br>"newNumberVal": null,<br>"oldNumberVal": 1,<br>"subObjCode": "HOUR",<br>"subObjID": "5785406d008d93dce3f7f2e0e8eda4ea"<br>},<br>{<br>"ID": "5785416f008db05ecee934663a968366",<br>"objCode": "JRNLE",<br>"changeType": "A",<br>"aux2": "Brad Littler",<br>"newNumberVal": 1,<br>"oldNumberVal": null,<br>"subObjCode": "HOUR",<br>"subObjID": "5785416f008db05d9d2925c12b10f521"<br>},<br>{<br>"ID": "57854176008db22fe974b7c67feea6b2",<br>"objCode": "JRNLE",<br>"changeType": "E",<br>"aux2": "Brad Littler",<br>"newNumberVal": 2,<br>"oldNumberVal": 1,<br>"subObjCode": "HOUR",<br>"subObjID": "5785416f008db05d9d2925c12b10f521"<br>}<br>]<br>}</pre>Following is a description of the included fields:

* **changeType:** The type of change being made to the object:

   * **A:** Add  
   
   * **E:** Edit  
   
   * **D:** Delete

* **aux2:** The name of the user the hour record is for.  

* **newNumberVal:** New value of the hour record (This will be null if the changeType is D).  

* **oldNumberVal:** Previous value of the hour record.  

* **subObjCode:** Type of record being modified (Should always be HOUR).  

* **subObjID:** ID of the Hour record.

You can use this information to discover what hour records have been changed, edited, or deleted. You can then use the subObjID to retrieve more information from the hour records if necessary.
