---
product-area: workfront-integrations
keywords: google,doc,document,sheet,slide
navigation-topic: workfront-for-g-suite
title: Privacy and permissions in Workfront for Google Workspace
description: Privacy and permissions in Workfront for Google Workspace
author: Becky
feature: Workfront Integrations and Apps
exl-id: abb8ffa1-1da6-46dd-a929-18b17014839a
---
# Privacy and permissions in Workfront for Google Workspace

Because customer privacy is important, Adobe Workfront does not store or collect any identifying customer data that results from third-party authorization of a Google plug-in app. Workfront for Google Workspace's use and transfer of information received from Google APIs to any other app will adhere with the [Google API Services User Data Policy](https://developers.google.com/terms/api-services-user-data-policy), including the Limited Use requirements.

We require the following permissions so the Workfront for Google Workspace plug-in can deliver its maximum value:

* **View your email messages when the add-on is running**: The Workfront for Google Workspace plug-in can save users countless hours of duplicative work by converting emails to new tasks in Workfront and automatically populating the task's title and description with email's subject and body. The plug-in also allows to post your emails to Workfront as new comments. The plug-in needs to view your email messages when the add-on is running to deliver this value.
* **Run as a Gmail add-on / non-sensitive**: Permissions are needed for the Workfront for Google Workspace add-on to function in Gmail environment. The plug-in requires a Gmail environment to work, so it requires the `Run as a Gmail add-on / non-sensitive` permission.
* **View your email message metadata when the add-on is running**: To improve workflows, the Workfront for Google Workspace plug-in confirms if an email is a Workfront notification, and identifies the type of Workfront notification (new work request, approval request, new comment etc.). The plug-in requires the `View your email message metadata when the add-on is running` permission to deliver this value.
* **Plug-in needs to Run as a Calendar add-on / non-sensitive**: The Workfront for Google Workspace plug-in connects to your calendar, so you can visualize how tasks impact schedules. The plug-in needs the `Run as a Calendar add-on / non-sensitive` permission to do this.
* **Connect to an external service permission:** Ultimately, the plug-in needs to connect to the Workfront API, which is the backbone of the plug-in value. The Workfront API is a service external to Google, so the plug-in requires the `Connect to an external service permission` to make the plug-in work.

For more information on Adobe Workfront's dedication to customer privacy, see [Workfront's Privacy Notice](https://www.adobe.com/content/dam/cc/en/legal/terms/enterprise/pdfs/Privacy-Notice-and-Privacy-Shield-Statement-Adobe-Workfront.pdf).

For more information, see [Google API Services User Data Policy](https://developers.google.com/terms/api-services-user-data-policy).
