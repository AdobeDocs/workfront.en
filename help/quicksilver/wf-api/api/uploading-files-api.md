---
content-type: api
navigation-topic: api-navigation-topic
title: Uploading files via the API
description: Uploading files via the API
author: Becky
feature: Workfront API
exl-id: 4e0b73b6-0d6d-4971-a87a-dfec85fb031a
---
# Uploading files via the API

You can upload files using WorkFront APIs with API tools, such as Postman, or with simple cURL commands.

To upload documents, see the instructions for **Uploading Documents** in WorkFront [Post Behavior](/help/quicksilver/wf-api/general/api-basics.md#post-behavior). You can also use these same instructions for cURL requests.

**When using API tools to upload files, follow these guidelines:**

* Use your API tool option to upload your file. These is often a **Choose File** button on the request screen. 

* Use the POST HTTP method to make the request to upload the file. 

* Your request should result in a response that includes a value for its handle. 

* Use the handle value, the object type, and the GUID value for the objID in a JSON payload to make a subsequent call. This is for creating the object for your file, as in the following example:

```
}
"name": "TestPDF",
"handle": "7af257e64aba4a22c33ccdfc40bbb87",
"docObjCode": "PROJ",
"objID": "0398450f8345980843445534354",
"currentVersion": {"version": "v1.0", "fileName" : "TestPDF"},
}
```     
        
You should receive an ID for the object in the response.

Refer to the help of the specific API tool you are using for more information.
