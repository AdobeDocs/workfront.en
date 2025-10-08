---
product-area: documents
navigation-topic: approvals
title: Frame.io integration overview
description: Frame.io integration overview
author: Courtney
feature: Work Management, Digital Content and Documents
recommendations: noDisplay, noCatalog
exl-id: b5f0150b-40b5-4386-98bc-374e7ca65b74
---
# Frame.io integration overview

The Workfront and Frame.io integration allows project coordinators to manage projects and plan work in Workfront while creatives, marketers, and stakeholders can review and approve assets in Frame.io.

## Integration requirements

* Workfront and Frame.io must be deployed to the same Identity Management system (IMS) organization.

* Users can belong to only one Workfront instance within the IMS organization.

* The Workfront instance must be enabled on the Adobe Unified Experience and Adobe enterprise storage.

* The integration must be configured by Adobe Professional Services. 


## Built on Adobe enterprise storage

At the core of this integration is Adobe enterprise storage—-a cloud-based storage solution that serves as the central repository for assets across Adobe enterprise products, including Workfront and Frame.io. <!--, and Creative Cloud.-->

Key benefits of Adobe enterprise storage include:

* Unified storage layer for creative and work management assets
* Centralized permissions via Adobe Identity Management system (IMS) for secure access control
* End-to-end asset visibility across Workfront and Frame.io <!--, and Creative Cloud apps -->
* Scalable storage and quota management for enterprise needs

For more details, see [Adobe enterprise storage overview](/help/quicksilver/review-and-approve-work/esm-overview.md).

## Unified review and approval 

The Workfront and Frame.io integration uses Workfront's unified approval functionality to manage reviews and approvals. With unified approvals, you can:

* Create and manage reviews and approvals directly from Workfront
* Track the status of reviews and approvals in real time
* Centralize feedback and approvals in one place
* Ensure that all stakeholders have access to the latest versions of assets
* Utilize AI Reviewers to automate brand compliance reviews
* and more

For more information, see [Unified document approvals: article index](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/document-reviews-and-approvals.md).


### Use the Frame.io viewer

The integration also connects with the Frame.io viewer. The Frame.io viewer provides

* Markup and commenting tools
* Version history and comparison
* Time-stamped comments for video reviews
* Mobile access for on-the-go reviews and approvals

For more information, see [Get started with the Frame.io integration](/help/quicksilver/review-and-approve-work/native-integrations/frame-io/get-started-with-frame-integration.md).

#### Video review limits

There is an annual cap for video proof requests set at 10% of an organization's total paid Workfront user licenses--Standard and Light. This cap is applied at the organization level. 

Workfront administrators will receive notifications when usage reaches 80% and 100% of the cap.

This limit does not apply to Frame.io Enterprise customers.

#### Supported file types in the Frame.io viewer

The Frame.io viewer supports all common video, image, audio, PDF, and MS&reg; Office types. For a detailed list of supported files, see [Supported File Types on Frame.io](https://help.frame.io/en/articles/9436564-supported-file-types-on-frame-io).

#### Access and licensing for the Frame.io viewer

The Frame.io viewer is the default viewer for all Workfront review and approval workflows. It is is automatically included for all Workfront users with a paid license. No additional Frame.io license is required to use the Frame.io viewer for reviews and approvals.

If your organization wants to take advantage of additional Frame.io functionality available with this integration, such as uploading assets directly to projects in Frame.io, you can purchase a Frame.io enterprise license. Contact your Adobe account representative to schedule a demo and explore the benefits of the full Frame.io solution.

Workfront Proofing functionality is not available with this integration.

## Powerful project management in Workfront

With the Workfront and Frame.io integration, project coordinators can leverage Workfront's powerful project management capabilities to plan, track, and manage work.

For more information about managing projects in Workfront, see [Projects: article index](/help/quicksilver/manage-work/projects/create-projects/create-project.md).

### Enforced structure and naming conventions

Because this integration is built using Adobe Enterprise Storage, there are some enforced structure and naming conventions to be aware of when managing projects and documents.

* Object names must be unique and can't be duplicated
* Adobe Enterprise Storage requires unique names for peer objects with the same parent in the hierarchy tree
* Documents can't have the same name if they belong to the same project
* Document names can't contain special characters, including: \ / : * ? " < > | # % { } $ ! @ + ` & = ^ ~ [ ] ; , .

With these limitations in mind, Workfront automatically renames objects or documents as needed to prevent conflicts.

### Sharing and permissions

As part of the integration, user permissions are controlled in Workfront and flow down to Frame.io. This means you cannot invite a user to a project in Frame.io or modify user permissions in Frame.io. These actions need to be done via the Project Share modal in Workfront.

The following table shows how Workfront permissions map to Frame.io permissions:

<table>
<tr>
<th>Workfront user permission</th>
<th>Frame.io user permission</th>
</tr>
<tr>
<td>Manage</td>
<td>Edit & Share</td>
</tr>
<tr>
<td>Contribute</td>
<td>Edit & Share</td>
</tr>
<tr>
<td>View</td>
<td>Comment Only</td>
</tr>
</table>



### Document management in Workfront

Documents are managed at the project level with this integration and can't be uploaded to tasks or issues at this time. 

Document access is also managed at the project level. If a user has access to a project, they can access all documents associated with that project.

### Document experience limitations

Because this integration is built using Adobe enterprise storage, there are some limitations to the original document experience in Workfront:

#### Limitations

The following capabilities will not be included in this integration:

<!--* External document providers-->
* Access to Proofing in Workfront
* Document viewer in Workfront
* Favorite documents
* Request documents


<!--#### Temporary limitations

For now, the following capabilities are not available:

* Send documents to Adobe Experience Manager Assets
* Multi-stage approvals
* Upload documents to comments or updates in Workfront
* Upload documents to tasks or issues in Workfront-->
