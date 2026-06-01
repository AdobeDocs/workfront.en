---
product-area: documents
navigation-topic: manage-documents
title: Check document storage limits
description: As an Adobe Workfront administrator, you view document storage usage and quota on the Customer Info page. How storage appears depends on whether your organization uses legacy Workfront storage or Adobe cloud storage.
author: Courtney
feature: Digital Content and Documents
exl-id: f5d1963e-b205-44b9-b2b6-b7de465c6977
last-update: 2026-04-29T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/vOjgBLxX5rFIGHBCHB2a6Q3Bs3KE5x-opXUMvANjI1E
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
    internal-label: Administration
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
---
# Check document storage limits

{{highlighted-preview}}

While there are no restrictions on the types and sizes of individual files that users can upload to your Workfront instance, your Workfront plan includes a total storage quota. As a Workfront administrator, you monitor usage and quota from the Setup area on the Customer Info page.

How storage appears depends on whether your organization uses legacy Workfront storage or Adobe cloud storage:

* If you use legacy Workfront storage, see [Legacy Workfront storage](#legacy-workfront-storage) in this article.
* If you use Adobe cloud storage, see [Adobe cloud storage](#adobe-cloud-storage) in this article.

   For more information about Adobe cloud storage, see [Adobe cloud storage overview](/help/quicksilver/review-and-approve-work/esm-overview.md).

## Access requirements

+++ Expand to view access requirements for the functionality in this article.


<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Workfront plan</td> 
   <td> <p>Any Workfront package to manage documents using legacy storage</p>
      <p>Any Workflow package to manage documents using Adobe cloud storage</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license</td> 
   <td> <p>You must be a Workfront administrator.</p> </td> 
  </tr> 
 </tbody> 
</table>

For more detail about the information in this table, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md). 

+++

## Legacy Workfront storage

If your organization uses legacy Workfront storage, the Customer Info page shows a single storage quota for documents uploaded directly to Workfront.

To check legacy Workfront document storage:

{{step-1-to-setup}}

1. In the left panel, click **System** > **Customer Info**.
1. In the **Basic Info** section, find **Storage Quota**. Here, you can view how much storage you're currently using as well as the total amount of storage your Workfront plan includes.

The storage quota is refreshed daily to show the most up-to-date count.

>[!NOTE]
>
>This limit does not apply to documents you link to Workfront from any other third-party service provider (SharePoint, Google Drive, Webdam, Box, Dropbox, or any other document asset management provider).

<div class="preview">

## Adobe cloud storage


If your organization uses Adobe cloud storage, your storage quota is reported as a single pooled allocation that combines storage provisioned through your Workfront license and any storage provisioned through a Frame.io Enterprise add-on. There's no hard cap on storage usage; users can continue uploading documents even when usage exceeds your quota.

### View storage usage on Customer Info

To check Adobe cloud storage for documents:

{{step-1-to-setup}}

1. In the left panel, click **System** > **Customer Info**.
1. Go to the **Storage Overview** section.
1. Review your usage. The Storage Overview shows your pooled storage quota and breaks usage into:

    * Workfront legacy projects and Adobe cloud storage projects display in the blue bar.
    * Frame standalone projects display in the green bar. These projects are separate from Workfront and only available if you have a Frame.io Enterprise license. 


![Adobe cloud storage usage on Customer Info](assets/storage-usage.png)

Usage figures refresh regularly so you see an up-to-date count. 

### Email notifications for administrators

When usage crosses 75%, 90%, or 100% of your storage quota, Workfront sends an email notification to System Administrators. 

</div>