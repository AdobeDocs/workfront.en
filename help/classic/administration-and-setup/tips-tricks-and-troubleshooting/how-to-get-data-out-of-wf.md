---
filename: how-to-get-data-out-of-wf
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: "Retrieving historical data from Adobe Workfront: pros and cons"
description: This article explains the pros and cons of 4 options you can use to retrieve your historical data from Workfront.
---

# Retrieving historical data from Adobe Workfront: pros and cons

>[!IMPORTANT]
>
>You're currently viewing the Adobe Workfront Classic version of this document. Adobe Workfront Classic is no longer supported. All Adobe Workfront Classic functionality, along with this documentation, will be removed in July 2022. Please transition to the the new Adobe Workfront experienceas soon as possible, and switch to the new Adobe Workfront experience version of this document.

This article explains the pros and cons of 4 options you can use to retrieve your historical data from Workfront.

## Use one of our partners

AtAppStore, a Workfront certified partner, has an easy-to-use app that allows you to download your data. This app also includes a viewer that allows you to easily view your data.

* **Pros:**&nbsp;All your Workfront objects are exported, including the custom fields. The interface of the Viewer is easy to use and read, and it’s easily importable in a MS Access Database.  

* **Cons:**&nbsp;Documents are not exported. You will have to download them separately. For more information, go to&nbsp; [http://www.atappstore.com/App/snapshot-to-msaccess/Default.aspx.](http://www.atappstore.com/App/snapshot-to-msaccess/Default.aspx)

## Request an Oracle data dump file from our Database team

Your Account Executive can submit a request to our Database team to export a database dump file (.dmp Oracle file) with your data. An additional request will go to our AOS team to retrieve all of your stored documents.

* **Pros**:&nbsp;You&nbsp;get your entire data load, including custom fields, as well as documents that are stored in the system.  

* **Cons**: The database file is hard to read: there is no way you can read this file unless you upload it to an Oracle database and re-establish the relationships between the tables. The documents&nbsp;are stored on a separate file server and must be extracted separately using a separate process by the AOS team. In doing so, there is no organization to the documents, and they are all referenced by their GUID.
* **Cost**:&nbsp;There is a cost associated with this download, depending on how long it takes the team to create the file. Check with your AE/ CAE for more information or to get this process started.

## Export via Kick-Starts

Whether you have remote consulting hours or not, you can use one of our consultants to export your data in the form of reports or kick-starts, or you can run these reports yourself:

* **Pros**:&nbsp;The reports are easy to read and can be imported in a variety of applications; they can be customized to include any groupings and views you’d like.  

* **Cons**:&nbsp;Documents will have to be downloaded separately.  

* **Cost**:&nbsp;It is free if you can run the reports yourself (all you would need is a system admin login), or if you can use remaining remote consulting hours. If you are interested in purchasing remote consulting for this, please talk with your AE/CAE.

  For more information about using Kick-Starts to export data, see [Export data from Adobe Workfront via Kick-Starts](../../administration-and-setup/manage-workfront/using-kick-starts/export-data-from-wf-via-kick-starts.md).

## Use our open API

if you have the right resources in your organization, they can build a custom API to retrieve all your data from Workfront:

* **Pros**:&nbsp;You are in control of what exports from the system.  

* **Cons**:&nbsp;The time is spent on your side, and you will have to find resources to code the API and perform the export.  

* **Cost**:&nbsp;Internal to your organization.

