---
product-area: documents
navigation-topic: approvals
title: Get started with unified review and approval
description: Learn more about unified review and approval powered by Workfront and Frame.io.
author: Courtney
feature: Work Management, Digital Content and Documents
exl-id: 10962d59-284e-4c41-8523-18ea4ed78362
---
# Get started with unified review and approval


Unified review and approval brings together Adobe Workfront and Adobe Frame.io into a single, deeply connected experience --- closing the gaps between marketing management, creative review, and content delivery. Project coordinators manage work in Workfront while creatives, marketers, and stakeholders review and approve assets in the professional-grade Frame.io viewer, all without moving files between disconnected tools.

For more information about Frame.io, see [Getting Started with Frame.io](https://support.frame.io/en/collections/49298-getting-started).

You must have the Workfront and Frame.io integration set up in your Workfront instance. For more information, see [Unified review and approval overview](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/document-approvals-overview.md#integration-requirements).

## Integration requirements

* Workfront and Frame.io must be deployed to the same Identity Management system (IMS) organization.

* Users can belong to only one Workfront instance within the IMS organization.

* The Workfront instance must be enabled on the Adobe Unified Experience and Adobe enterprise storage.

* The integration must be configured by Adobe Professional Services. 

## Work initiation and planning in Workfront

Project coordinators can create projects and plan work in Workfront. Projects created in an instance with the Frame.io integration enabled utilize Adobe enterprise storage, which allows assets to be stored and managed within the Adobe ecosystem.

If your organization has a Frame.io Enterprise license, projects created in Workfront are also visible in Frame.io, allowing users to interact and upload assets in either product. 

For information about Adobe enterprise storage or projects in Frame.io, see

* [Workspace Overview: Projects](https://help.frame.io/en/articles/9101001-workspace-overview#h_d9f8654895)
* [Adobe enterprise storage overview](/help/quicksilver/review-and-approve-work/esm-overview.md)

## Review and approve assets

Once an asset is finished, the project coordinator can initiate the formal review and approval process in Workfront.

After the approval workflow is created, reviewers and approvers can use the Frame.io viewer to add comments and mark up the asset. They can also make the approval decision in the Frame.io viewer.

For more information about setting up projects, see 

* [Create a project](/help/quicksilver/manage-work/projects/create-projects/create-project.md)

### Initiate formal reviews and approvals in Workfront

Project coordinators can create one-time review and approvals or reusable approval templates. They can assign reviewers, approvers, or a mix of both:

* **Reviewers** can add comments and mark up assets. Once finished, they can mark their review as complete. Marking the review as complete is not required for the asset to move forward in the approval process.
* **Approvers** can add comments and mark up assets. They must make a decision to move the approval process forward. 

#### Create a review and approval workflow

Reviewers and approvers can be added to a single-use approval workflow or a reusable approval template:

* **Single-use approvals**: In the project or task where the asset resides, the project coordinator can assign reviewers and approvers and set a completion deadline. Reviewers and approvers are reminded by email 72 hours before the deadline, 24 hours before the deadline, and then on the deadline itself.

    For more information, see [Create a document approval workflow](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-a-document-approval.md#create-an-approval-workflow-from-the-summary-panel-in-the-new-document-area).

* **Approval templates**: In the Workfront Setup area, project coordinators can create reusable Approval Templates. Within a template, users can add reviewers and approvers and specify a completion timeframe. When the approval template is applied to an asset, the deadline is calculated from the specified timeframe. 

    Once a template is created, it can be applied to an asset to begin the formal review and approval process in Workfront.

    For more information, see [Create an approval workflow template for documents](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-approval-template.md).

### Review and approve assets in the Frame.io viewer

Once the review and approval workflow is initiated in Workfront, reviewers and approvers can access the Frame.io viewer to add comments, mark up the asset, and make a decision. 

For more information, see [Review and approve with the Frame.io viewer](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/review-with-frame.md).

#### Access the Frame.io viewer

Users can access the Frame.io viewer in the following ways:

* Workfront email notifications
* The My approval widget in the Workfront Home area

>[!NOTE]
>
>External Workfront users are notified via email and will be asked to create a Frame.io login to review and approve assets.

![open the frame viewer from Home](assets/open-fio-viewwer.png)

#### Add comments and mark up assets

Comments and asset markup is visible in the Frame.io viewer. For more information on using the Frame.io viewer, see [Commenting on your media](https://help.frame.io/en/articles/9105251-commenting-on-your-media).

#### Make a decision

Once all review activity is complete, approvers must make one of the following decisions:

* **Approve**: The asset does not need changes and is ready for use.
* **Approved with changes**: The asset is mostly complete but needs minor changes before it can be used. Once the specified changes are made, the asset is ready and does not need to go through another round of approvals. 
* **Needs work**: The asset needs changes and is not ready for use. Once the specified changes are made, the asset must be uploaded as a new version and go through another round of approvals. <!--is the same approval workflow automatically applied? Does the coordinator have to do anything to get the approval going? -->

Reviewers can mark their review complete inside of Workfront, but this is not required for the asset to move forward in the approval process. 

For more information about decisions in Workfront, see [Document decision status overview](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/document-approval-status.md). 

![Frame viewer and decision](assets/decision-fio.png)


### Track review and approval metrics

Project coordinators can monitor progress on all in-flight approvals in the Workfront Home area or with customized reports in Canvas Dashboards:

* **Custom dashboard**: Create a report dashboard in the Canvas Dashboards area to display both high-level and detailed information about reviews and approvals with Unified Approvals functionality. For information on how to get started, see [Create a report dashboard for review and approvals](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/create-review-and-approval-dashboard.md).
* **Document approval metrics Home widget**: Displays 2 charts with information about average approval time and decisions as well as list views of pending and overdue approvals.
    ![All approvals](assets/all-approvals.png)

## Send finished assets to Adobe Experience Manager

You can use the [!DNL Experience Manager Assets]​​ to manage and store your digital assets that have gone through the review and approval cycle. This integration allows you to leverage the capabilities of Adobe Experience Manager, Frame.io, and Workfront to streamline your content management and collaboration processes.

For more information, see [Use the Adobe Experience Manager with the Frame.io integration](/help/quicksilver/review-and-approve-work/native-integrations/frame-io/use-aem-with-frame.md).


## Frequently Asked Questions

### Access unified review and approval

+++ Expand to view the frequently asked questions for unified review and approval.

**How do I get access to Unified Review and Approval?**

**What do I need to do to get access?**

To access unified review and approval, your organization must be on a Workfront V2 SKU. If you are not currently on a V2 SKU, this will require a contracting event with Adobe. To get started:

* Contact your Adobe account representative to confirm whether your current Workfront plan supports unified review and approval.

* If a SKU upgrade is needed, your account representative will guide you through the contracting process.

* Once your account is on the correct SKU, Adobe Professional Services will configure the integration for your organization.

     * If you are not sure who your Adobe account representative is, you can reach out through the Adobe support portal or visit Experience League for contact options.

+++

### Getting Started with unified review and approval

+++ Expand to view the frequently asked questions for getting started with unified review and approval.

**What is unified review and approval?**

Unified review and approval is a native integration between Adobe Workfront and Adobe Frame.io that brings work management and creative review together in a single, connected system. Project coordinators plan and track work in Workfront, while reviewers and approvers use the professional-grade Frame.io viewer to provide feedback, mark up assets, and make approval decisions--without toggling between separate tools or manually moving files.

Review and approval sits at the center of every content operation. It is where creative work, stakeholder input, and business decisions converge. When that process is spread across disconnected tools--email threads, chat messages, screenshot markups --- the consequences compound: slower time to market, lost feedback, version confusion, and time spent managing files instead of creating content.

Unified review and approval addresses this by replacing the patchwork of disconnected review tools with one modern system--a single source of truth that lives where work already happens.

**What are the requirements to use this integration?**

To use unified review and approval, the following conditions must be met:

* Workfront and Frame.io must be deployed to the same Adobe Identity Management System (IMS) organization.

* Users can belong to only one Workfront instance within the IMS organization.

* The Workfront instance must be enabled on the Adobe Unified Experience and Adobe enterprise storage.

* The integration must be configured by Adobe Professional Services.

* Workfront customers must be on a V2 SKU (this may require a contracting event--contact your Adobe account representative).

**Do I need a Frame.io license to use this integration?**

No. The Frame.io viewer is automatically included for all Workfront users with a paid license at no additional cost. You do not need a separate Frame.io license to review and approve assets through Workfront.

If your organization wants access to additional Frame.io capabilities --- such as uploading assets directly to projects in Frame.io --- you can purchase a Frame.io Enterprise license. Contact your Adobe account representative to learn more.

**Does this replace Workfront Proof?**

Yes. When unified review and approval is enabled, the Frame.io viewer becomes the primary review surface in Workfront, replacing Workfront Proof. Existing Workfront Proofing functionality is not available within this integration.

+++

### How unified review and approval Works

+++ Expand to view the frequently asked questions for how unified review and approval works.

**How does the review and approval workflow work?**

The workflow follows these general steps:

* A project coordinator creates a project in Workfront and uploads or links assets.

* When an asset is ready for review, the coordinator creates an approval workflow--either a single-use approval or by applying a reusable approval template.

* Assigned reviewers and approvers are notified via email and can open the asset directly in the Frame.io viewer.

* Reviewers can add comments and markup. Approvers must make a formal decision.

* The coordinator tracks status in real time from Workfront.

**What is the difference between a reviewer and an approver?**

Reviewers can add comments and mark up assets, and can mark their review as complete. However, their action is not required for the approval to progress.

Approvers must make one of the following decisions to move the process forward:

* Approve: The asset is ready to use as-is.

* Needs work: The asset requires changes and must be re-submitted as a new version for re-approval.

**What types of approval workflows can I create?**

There are two options:

* Single-use approvals: You can create a single-use approval directly on a document in a project or task. You assign reviewers and approvers, set a deadlines, and configure multiple stages if needed. Automated email reminders are sent 72 hours before, 24 hours before, and on the deadline.

* Approval templates: Reusable templates created in Workfront Setup. A template defines the reviewers, approvers, a relative completion timeframe, and multiple stages if needed. Once applied to an asset, the deadline is calculated automatically.

**How do external users participate in reviews?**

External Workfront users are notified via email when they are assigned to a review or approval. They will be prompted to create a Frame.io login to access the viewer and participate in the review process.

**How do I track review and approval progress?**

Project coordinators can monitor all in-flight approvals in several ways:

* The My Approvals widget in the Workfront Home area provides a real-time summary of pending and overdue approvals.

* The Document Approval Metrics widget displays average approval times and decision breakdowns.

* Custom report dashboards can be built in Canvas Dashboards for deeper visibility into review and approval activity.

+++

### Storage and file management

+++ Expand to view the frequently asked questions for storage and file management.

**What is Adobe enterprise storage and how does it relate to this integration?**

Adobe enterprise storage is the common storage layer that connects Workfront, Frame.io, and Adobe Creative Cloud. Assets live in one place and are accessible across tools without manual file transfers. Creatives can work in place, and reviewers always see the latest version.

Key benefits of Adobe enterprise storage include:

* A single storage layer for all work-in-progress assets across Workfront and Frame.io

* Centralized access control managed through Adobe Identity Management System (IMS)

* End-to-end asset visibility--no version drift, no lost metadata

* Scalable, enterprise-grade storage management

**Are there naming or structure requirements for files and projects?**

Yes. Because the integration uses Adobe enterprise storage, the following conventions apply:

* Object and document names must be unique within the same parent in the folder hierarchy.

* Documents within the same project cannot share a name.

* Document names cannot contain the following special characters: `\\ / : \* ? \" \| \< \>`

* Document names are limited to 255 characters.

Workfront automatically renames objects or documents as needed to prevent conflicts.

**What file types are supported in the Frame.io viewer?**

The Frame.io viewer supports over 40 file formats, including all common video, image, audio, PDF, and Microsoft Office types. Video support includes native playback for professional formats such as ProRes, H.265, and DNxHD, with support for files up to 500 GB.

Frame.io was purpose-built for creative review, which means it handles the full range of asset types that marketing and creative teams work with --- not just static documents. For a complete list of supported formats, see the Frame.io supported file types documentation on Experience League.

+++

### Permissions and access

+++ Expand to view the frequently asked questions for permissions and access.

**How are user permissions managed?**

User permissions are set and controlled in Workfront and automatically flow through to Frame.io. You cannot invite users or modify permissions directly in Frame.io for this integration. All access management must be done using the project share modal in Workfront.

The table below shows how Workfront permissions map to Frame.io permissions:

<table>
  <thead>
    <tr>
      <th>Workfront Permission</th>
      <th>Frame.io Permission</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>Manage</td>
      <td>Edit &amp; Share</td>
    </tr>
    <tr>
      <td>Contribute</td>
      <td>Edit &amp; Share</td>
    </tr>
    <tr>
      <td>View</td>
      <td>Comment Only</td>
    </tr>
  </tbody>
</table>

+++

### Video reviews

+++ Expand to view the frequently asked questions for video reviews.

**Are there any limits on video reviews?**

Yes. There is an annual cap on video proof requests set at 10% of your organization's total paid Workfront user licenses (Standard and Light). This cap applies at the organization level.

Workfront administrators will receive in-app notifications when usage reaches 80% and 100% of the cap.

This limit does not apply to Frame.io Enterprise customers. If your organization regularly reviews large volumes of video content, contact your Adobe account representative to learn about Frame.io Enterprise licensing.

+++

### Integrations and advanced capabilities

+++ Expand to view the frequently asked questions for integrations and advanced capabilities.

**How does this impact existing Creative Cloud plugin integrations with Adobe Express and  GenStudio?**

Integrations supporting the Frame.io viewer experience are currently in development for Adobe Express and GenStudio Performance Marketing. The new integrations will be built on the same unified review and approval system, so they will leverage the Frame.io viewer for a consistent review experience across all three products.

**Is Frame.io integrated within Workfront, or do users navigate to a separate interface?**

Users can launch the Frame.io viewer directly from Workfront, and all review and approval activity takes place within that viewer, and is automatically synced back to Workfront.

**Can I send approved assets to Adobe Experience Manager (AEM)?**

Yes. Once an asset completes the review and approval cycle, you can transfer it to Adobe Experience Manager Assets for final storage and distribution. This connects Workfront for work management, Frame.io for review, and AEM for digital asset management into a unified content supply chain.

For more information, see For more information, see [Use the Adobe Experience Manager with the Frame.io integration](/help/quicksilver/review-and-approve-work/native-integrations/frame-io/use-aem-with-frame.md).

**How does unified review and approval fit into Adobe GenStudio?**

Unified review and approval is a foundational component of Adobe GenStudio--Adobe's broader vision for a connected content supply chain. GenStudio connects Workfront, Frame.io, Creative Cloud, Adobe Express, Adobe Experience Manager Assets, and GenStudio for Performance Marketing into a unified workflow from campaign brief through content delivery.

Within that ecosystem, review and approval serves as the critical handoff point between creation and delivery. It is where creative work meets stakeholder input, quality gets validated, and content is cleared to publish. When that handoff is fast, visible, and reliable, it unlocks velocity across the entire content supply chain--AI can accelerate creation, automation can handle distribution, but a bottleneck in review caps the gains on both sides. Connecting Workfront and Frame.io removes that bottleneck.

**What is the AI Reviewer feature?**

Unified review and approval includes an AI Reviewer capability that automates brand compliance checks as part of the review process. The AI Reviewer can evaluate assets against brand guidelines and flag potential issues before human reviewers are engaged, helping teams catch problems earlier and move faster.

For more information on setting up and using AI Reviewer, see the Workfront documentation on Experience League.

+++

### Contracts, SKUs, and storage

+++ Expand to view the frequently asked questions for contracts, SKUs, and storage.

**When will unified review and approval be available to me?**

Unified review and approval is available now. Access requires an upgrade to a Workfront V2 SKU. If your contract was signed before the V2 SKUs were available, you can gain access in one of two ways:

* Upon renewal: Access will be enabled at your next contract renewal date.

* Early recontract: Your Adobe account team can recontract you early to add the new SKU entitlements while keeping your existing contract end date. There is no price increase when moving to an equivalent package.

Contact your Adobe account representative to determine the best path for your organization.

**Does upgrading to the V2 SKU give me more storage?**

Yes. With the V2 SKU, each licensed user receives 60 GB of storage, up from 30 GB in the previous version.

**How do I choose between Adobe enterprise storage and legacy Workfront storage?**

Enterprise Storage enables the Frame.io viewer experience and is required for unified review and approval. Legacy Storage continues to use the Workfront Proof viewer (ProofHQ) as the default.

If your organization has a mix of simple workflows and more complex proofing workflows, you can prioritize which workflows to migrate first. Enterprise Storage gives you the flexibility to roll out the new experience incrementally, starting with the workflows that will benefit most.

**How are Frame.io licenses managed?**

After signing the V2 SKU, all Workfront users will have access to the Frame.io viewer for review and approval workflows --- no separate Frame.io Enterprise license is required for this.

If your organization needs additional Frame.io Enterprise features such as 

* Advanced watermarking (dynamic and forensic)
* Digital rights management with automatic asset deletion
* Content credentials for AI-generated content
* Custom creative metadata
* Camera to Cloud integrations
* Your own workspace for creative work-in-progress

you can work with your Adobe account team to determine the appropriate number of Frame.io Enterprise licenses. All licenses are managed through the Adobe Admin Console.

+++

### Sandbox and Rollout

+++ Expand to view the frequently asked questions for sandbox and rollout.

**Can I test unified review and approval in a sandbox environment?**

Partially. Approval workflows can be tested in a Workfront sandbox environment. However, the Frame.io viewer experience is not available in sandbox --- testing the review surface itself requires a production environment.

To limit exposure during rollout, you can enable unified review and approval for a specific group within your Workfront production environment. This allows you to run a targeted pilot with a smaller set of users before rolling out more broadly.

+++

### Reviewing and approving assets

+++ Expand to view the frequently asked questions for reviewing and approving assets.

**Can the same user appear in multiple stages of an approval workflow?**

Yes. A user can be assigned to multiple stages within the same approval workflow. This is a significant improvement over the previous proofing experience.

**Can I add stages to create a multi-stage approval workflow?**

Yes. Multi-stage approval workflows are supported, allowing you to route assets through sequential rounds of review and approval with different participants at each stage. Each stage has clear roles --- reviewers provide feedback while approvers make binding decisions --- so approvals reach a conclusion rather than stalling in inboxes. All participants have real-time visibility into exactly where each asset stands in the process.

**Can approval templates include groups or teams, or only individual users?**

Currently, approval templates support individual users. The ability to add groups or teams to approval templates is an area of active development --- check the Workfront release notes on Experience League for updates.

**Are approvers notified by email when they have something to review?**

Yes. Approvers and reviewers receive email notifications when they are assigned to a review or approval. Automated reminder emails are also sent 72 hours before the deadline, 24 hours before, and on the deadline itself.

The ability to customize email notification messages is not currently available, but it is on the product roadmap.

**Can I keep a review stage private from other participants?**

There is currently no native private stage feature. To keep a review private from other participants, the recommended approach is to create a separate copy of the asset specifically for that review group. Comments are not currently segmented by participant group within a single asset.

Note that version history --- including past and current versions --- is always visible to anyone with access to view that asset.

**Can comments be marked as resolved?**

Yes. Comments can be marked as resolved within the Frame.io viewer.

**What markup and annotation tools are available in the Frame.io viewer?**

The Frame.io viewer includes a full set of visual markup tools, including freehand drawing and standard shapes such as circles, arrows, and squares. For video assets, comments are time-stamped with frame-accurate precision, so feedback is always tied to the exact moment in the clip --- not just a general timestamp.

**Will comments made in the Frame.io viewer appear in the Workfront project?**

Comments and annotations remain within the Frame.io viewer so that they retain their full context --- including timestamps and visual markups. This may evolve in future releases.

**Is it possible to add comments to a downloaded version of an asset (e.g., a PDF)?**

This is not currently supported, but it is a commonly requested feature that is under consideration for a future release.

**Can I review multiple assets together as a group?**

Enhanced bulk review options are coming soon. In the meantime, assets of different file types --- such as a video and a Word document --- can be included together in a grouped asset review.

**Is unified review and approval only for video, or does it support other file types?**

Unified review and approval is designed for all asset types, not just video. The Frame.io viewer has been significantly updated to support images, documents, PDFs, and other common file formats in addition to video.

For a full list of supported file types, see the Frame.io supported file types documentation on Experience League.

**Can I share assets externally with stakeholders who don\'t have access to Workfront?**

Yes. Assets can be shared externally. External users are notified via email and will be prompted to create a Frame.io login to access the viewer and participate in the review.

+++

### Interactive Proofs and HTML

+++ Expand to view the frequently asked questions for interactive proofs and HTML.

**Does unified review and approval support interactive proofs or HTML URLs?**

Zip HTML files are currently supported for interactive review. HTML URL support (live web URL review) is on the roadmap and expected in Q3. Check the Workfront release notes on Experience League for updates.

+++

### Fusion and automation

+++ Expand to view the frequently asked questions for Fusion and automation.

**Do I need Workfront Fusion to use unified review and approval?**

No. Unified review and approval is a native product integration and does not require Fusion. The workflow is built directly into Workfront.

**Will Fusion connectors be available for unified review and approval?**

Yes. Fusion actions for unified review and approval are currently in development and are expected to be available in Q3. Check the Workfront release notes on Experience League for updates as they become available.

**Can Fusion be used to automatically trigger a review when a document is uploaded?**

Yes. This type of automation is possible using Workfront webhooks in combination with Fusion.

**How will existing Fusion workflows built on Workfront Proof be affected?**

The impact will vary depending on how each workflow is built. In general:

* Edit or update: Workflows where the existing proof-related action has a direct equivalent in unified approvals can be updated to use the new action.

* Rebuild: Workflows where the underlying steps have changed significantly, or where new capabilities exist, may need to be rebuilt from scratch.

A clearer picture will emerge once the Fusion APIs for unified approvals are available. It is recommended to audit your existing Fusion workflows and evaluate them against the new unified approvals capabilities at that time.

+++


