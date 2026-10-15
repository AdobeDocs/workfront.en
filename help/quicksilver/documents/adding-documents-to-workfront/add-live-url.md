---
product-area: documents
navigation-topic: add-documents-to-workfront
title: Add a web link as a document
description: You can add a website to Adobe Workfront as a web link and request approval on it.
author: Courtney
feature: Digital Content and Documents
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
---
# Add a web link as a document

You can add a website to Adobe Workfront as a web link from the new Documents area. After you add it, you can request approval on the live web page the same way you request approval on an uploaded file.

If your organization uses Adobe cloud storage, you will see the new Documents area when you access documents in Workfront. For more information about Adobe cloud storage, see [Adobe cloud storage overview](/help/quicksilver/review-and-approve-work/esm-overview.md).

## Access requirements

+++ Expand to view access requirements for the functionality in this article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront package</td> 
   <td> <p>Any Workfront package to manage documents using legacy Workfront storage</p>
<p>Any Workflow package to manage documents using Adobe cloud storage</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront licenses</td> 
   <td> 
   <p>Contributor or higher</p> 
   <p>Request or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>Legacy Workfront Storage: Edit access to Documents</p> 
   <p>Adobe cloud storage: Edit access to Documents is enabled by default and cannot be changed</p>
   </td> 
  </tr> 
 </tbody> 
</table>

For information, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md). 

+++

## Add a web link as a document

You can upload an html web page to Workfront as a web link. After you add it, you can request approval on the live web page the same way you request approval on an uploaded file. For more information about how Frame.io handles web links, see [Frame.io web links](https://support.frame.io/hc/en-us/articles/360041187574-Frame-io-Web-Links).

<!--
>[!IMPORTANT]
>
>A web page behind single sign-on or a login page can't be displayed for review.
-->

To add a web link:

1. Go to the project, task, or issue where you want to add the website, then select **Documents** in the left panel.
1. Click **New**, then select **Web link**.
1. Enter a name in the **Document name** field, then enter the website's address in the **URL** field.
1. Click **Add**.
    ![Add a web link as a document](assets/web-url.png)

To request approval on the web link, see [Create a document approval workflow](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-a-document-approval.md).

## Known limitations

* There is a temporary issue with web link documents created in Frame.io. If you create a web link in Frame.io and then create an approval on it in Workfront, the document will not open in Frame.io. Web links created in Workfront are not affected. Until this is resolved, create web link documents in Workfront before starting an approval.
* 