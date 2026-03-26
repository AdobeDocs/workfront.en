---
product-area: documents
navigation-topic: approvals
title: Unified review and approval overview
description: Learn more about unified review and approvals powered by Workfront and Frame.io.
author: Courtney
feature: Work Management, Digital Content and Documents
recommendations: noDisplay, noCatalog
exl-id: 32cb95c2-8d12-492b-ad89-b38e2a337fc5
---

# Unified review and approval overview

Unified review and approvals powered by Workfront and Frame.io allows project coordinators to manage projects and plan work in Workfront while creatives, marketers, and stakeholders can review and approve assets in Frame.io.

## Integration requirements

* Workfront and Frame.io must be deployed to the same Identity Management system (IMS) organization.

* Users can belong to only one Workfront instance within the IMS organization.

* The Workfront instance must be enabled on the Adobe Unified Experience and Adobe enterprise storage.

* The integration must be configured by Adobe Professional Services. 


## Built on Adobe enterprise storage

Unified review and approvals is built on Adobe enterprise storage—-a cloud-based storage solution that serves as the central repository for assets across Adobe enterprise products, including Workfront and Frame.io. <!--, and Creative Cloud.-->

Key benefits of Adobe enterprise storage include:

* Unified storage layer for creative and work management assets
* Centralized permissions via Adobe Identity Management system (IMS) for secure access control
* End-to-end asset visibility across Workfront and Frame.io <!--, and Creative Cloud apps -->
* Scalable storage and quota management for enterprise needs

For more details, see [Adobe enterprise storage overview](/help/quicksilver/review-and-approve-work/esm-overview.md).

## Unified review and approval 

With unified review and approvals, you can:

* Create and manage reviews and approvals directly from Workfront
* Track the status of reviews and approvals in real time
* Centralize feedback and approvals in one place
* Ensure that all stakeholders have access to the latest versions of assets
* Utilize AI Reviewers to automate brand compliance reviews
* and more

For more information, see [Unified document approvals: article index](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/document-reviews-and-approvals.md).


### Use the Frame.io viewer

Use the Frame.io viewer to review and approve assets. The Frame.io viewer provides

* Markup and commenting tools
* Version history and comparison
* Time-stamped comments for video reviews
* Mobile access for on-the-go reviews and approvals

For more information, see [Get started with unified review and approval](/help/quicksilver/review-and-approve-work/native-integrations/frame-io/get-started-with-frame-integration.md).

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

Project coordinators can leverage Workfront's powerful project management capabilities to plan, track, and manage work.

For more information about managing projects in Workfront, see [Projects: article index](/help/quicksilver/manage-work/projects/create-projects/create-project.md).

### Enforced structure and naming conventions

Because unified review and approvals is built using Adobe enterprise storage, there are some enforced structure and naming conventions to be aware of when managing projects and documents.

* Object names must be unique and can't be duplicated
* Adobe enterprise storage requires unique names for peer objects with the same parent in the hierarchy tree
* Documents can't have the same name if they belong to the same project
* Document names can't contain any of the following special characters: \ / : * ? " | < >
* Document names are limited to 255 characters maximum

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

Documents uploaded to Workfront are stored in Adobe enterprise storage and are accessible in both Workfront and Frame.io. When you upload a document to a task or issue in Workfront, a system-generated folder is created in Adobe enterprise storage that inherits permissions from the task or issue. All documents uploaded to that task or issue are stored in that folder and inherit permissions from it. For more information about documents in Workfront, see [The new documents area overview](/help/quicksilver/documents/managing-documents/documents-area.md) and [Object permissions and access level overview for the Adobe enterprise storage model](/help/quicksilver/review-and-approve-work/esm-access-permissions.md).

### Document experience limitations

The following Document capabilities are not be included:

<!--* External document providers-->
* Access to Proofing in Workfront
* Document viewer in Workfront
* Favorite documents
* Request documents










<!--
# Unified Approvals overview

>[!IMPORTANT]
>
>The content of this article refers to updated document approval functionality that is only available for specific accounts. For information on standard approval processes, see the articles listed in [Work approvals](/help/quicksilver/review-and-approve-work/manage-approvals/manage-approvals.md).

Unified Approvals, previously referred to as New Document Approvals, is a holistic redesign of the existing approvals process that is currently in development for Adobe Workfront. Currently available in limited release, it is designed to be a practical and effective solution for businesses requiring comprehensive stakeholder engagement and version-specific document approvals. Its thoughtful design and purposeful new features facilitate collaboration, role clarity, and version control in the approval process, enhancing efficiency and accountability.

## Key differences from Proofing and legacy document approvals

**Differences from Proofing**

* Document approval participants display in the document Summary, not the proofing workflow tab.
* Unified Approvals are not supported in the current reporting tool. 

    You can join the new Canvas Dashboards beta to [Create a report dashboard for review and approvals](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/create-review-and-approval-dashboard.md), or you can use the Document approval metrics widget available in new Home and Canvas Dashboards provides the following details about Unified Approvals:

    * Approvals by decision
    * Average approval time
    * Pending approvals
    * Overdue approvals

**Differences from Legacy document approvals**

With Unified Approvals, you can

* Add reviewers in addition to approvers
* Designate an entire Workfront team as either reviewers or approvers
* Set a deadline for the review or approval
* Create and resuse approval templates
* Utilize new versions 
* View multiple key performance indicators for your approvals in Workfront Home widgets
* Use Canvas Dashboards to view reporting details about Unified Approvals

## Using Unified Approvals

For users looking to create or manage document approvals, see the articles listed in [Set up and manage unified approvals: article index](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/set-up-and-manage-doc-asset-approvals-toc.md)

For users looking to review or approve documents for which they have received a request, see the articles listed in [Approve and review documents: article index](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/review-and-approve-documents/review-documents-toc.md).



-->