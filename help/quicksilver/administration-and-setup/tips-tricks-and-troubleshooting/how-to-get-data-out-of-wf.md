---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: 'Export historical data from Adobe Workfront: Pros and cons'
description: This article explains the pros and cons of 4 options you can use to export historical data from Workfront.
author: Courtney
feature: System Setup and Administration
role: Admin
exl-id: ed40984f-602a-46e9-a72b-141936de8fcb
---
# Export historical data from [!DNL Adobe Workfron]t: Pros and cons

This article explains the pros and cons of 4 options you can use to export historical data from [!DNL Workfront].

## Use one of our partners

[!DNL AtAppStore], a [!DNL Workfront] certified partner, has an easy-to-use app that allows you to download your data. This app also includes a viewer that allows you to easily view your data.

* **Pros:** All your [!DNL Workfront] objects are exported, including the custom fields. The interface of the Viewer is easy to use and read, and it's easily importable in a [!DNL MS Access] Database.  

* **Cons:** Documents are not exported. You will have to download them separately. For more information, go to [http://www.atappstore.com/App/snapshot-to-msaccess/Default.aspx.](https://www.atappstore.com/App/snapshot-to-msaccess/Default.aspx)

## Request a [!DNL Postgres] data dump file from our Database team

Your Account Executive can submit a request to our Database team to export a database dump file (.dmp [!DNL Postgres] file) with your data. An additional request will go to our AOS team to retrieve all of your stored documents.

* **Pros**: You get your entire data load, including custom fields, as well as documents that are stored in the system.  

* **Cons**: The database file is hard to read: there is no way you can read this file unless you upload it to a [!DNL Postgres] database and re-establish the relationships between the tables. The documents are stored on a separate file server and must be extracted separately using a separate process by the AOS team. In doing so, there is no organization to the documents, and they are all referenced by their GUID.
* **Cost**: There is a cost associated with this download, depending on how long it takes the team to create the file. Check with your AE/ CAE for more information or to get this process started.

## Export via [!UICONTROL Kick-Starts]

Whether you have remote consulting hours or not, you can use one of our consultants to export your data in the form of reports or [!UICONTROL kick-starts], or you can run these reports yourself:

* **Pros**: The reports are easy to read and can be imported in a variety of applications; they can be customized to include any groupings and views you'd like.  

* **Cons**: Documents will have to be downloaded separately.  

* **Cost**: It is free if you can run the reports yourself (all you would need is a system admin login), or if you can use remaining remote consulting hours. If you are interested in purchasing remote consulting for this, please talk with your AE/CAE.

  For more information about using Kick-Starts to export data, see [Export data from [!DNL Adobe Workfront] via [!UICONTROL Kick-Starts]](../../administration-and-setup/manage-workfront/using-kick-starts/export-data-from-wf-via-kick-starts.md).

## Use our open API

if you have the right resources in your organization, they can build a custom API to retrieve all your data from Workfront:

* **Pros**: You are in control of what exports from the system.  

* **Cons**: The time is spent on your side, and you will have to find resources to code the API and perform the export.  

* **Cost**: Internal to your organization.
