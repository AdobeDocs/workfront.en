---
content-type: reference
navigation-topic: betas
title: 'Adobe Workfront and Frame.io native integration alpha: features'
description: Planned features for the Adobe Workfront and Frame.io native integration alpha
author: Nolan
feature: Product Announcements
hide: yes
hidefromtoc: yes
exl-id: a1603a06-957b-4d52-89f3-f0cec1a4e02c
---
# Adobe Workfront and Frame.io native integration alpha: features

## Use cases and feature testing

With this integration, our goal is to allow creatives to stay in their tool of choice (CC or Frame.io) to conduct their content creation and peer reviews, while having project managers coordinate the work and initialize and monitor the formal review process from inside Workfront. This can be achieved by utilizing the best of both solutions: Workfront's new document approvals for managing content approvals, in conjunction with the content review capabilities offered by Frame.io. Collectively, the new document approvals and Frame.io are going to form our new end-to-end content review and approval experience.  
 
To learn more about how the alpha will function and ways you can participate, see [Adobe Workfront and Frame.io integration alpha: overview](/help/quicksilver/product-announcements/betas/frame-io-wf-integration-alpha/frame-io-wf-integration-alpha-overview.md)


>[!NOTE]
>
>In case you came across these pages without your company participating in this alpha program, please make sure to treat the information here with care and reach out to your Workfront or Frame.io administrator for more information.

<!--Initial setup and basic test scenario 

As part of the alpha program, we've provisioned a new test Frame.io account for you and connected it to a new group "Frame.io alpha testing" in your existing Workfront Preview or Sandbox environment. To test the delivered functionality please log in to your Workfront Preview or Sandbox instance and  perform the following steps: 

Coordinators: Within Workfront, create a project with the "Frame.io alpha testing" group assigned as project group 

Coordinators: Within Workfront, assign your creatives to the project or Frame enabled tasks and change the project status to "Current" 

Creatives: Check your emails for an invite to the newly created Frame.io project 

Creatives: Click on the "Join project" button within the invitation email to join the Frame.io project, review the creative brief within the project and start your content creation within your CC tool of choice 

Creatives: Upload your created assets to Frame.io and add them to the linked Workfront project (or assigned Frame enabled tasks)  

Coordinators: Within Workfront, see the linked Frame.io assets in your project and assign reviewers / approvers (new document approvals: More help on this feature) 

Stakeholders: Withing Workfront, view your approval request in Workfront Home or Document Details and review the Frame connected document in the Frame.io Viewer. Leave a comment feedback 

Coordinators: Within Workfront, view the stakeholder created comments within the Updates section of the Frame.io connected document in Workfront 

Stakeholders: Make a decision from within the Frame.io Viewer 

Creatives: Within Frame.io, notice the overall approval decision made for your assets 

Creatives: Within Frame.io, Apply the requested changes by adding the updated version to the version stack of the connected asset 

Coordinators: Within Workfront, assign approvers / reviewers to the new version upload and monitor the progress until it reaches sign-off--> 

## Feature plans

Below is information about the primary use cases we are looking to address and the features we currently have planned to do so. <!--, along with documentation to get you started testing.--> 
 

### Workfront admins can set up a connection between Workfront groups and Frame.io accounts 

* _Within Workfront, you have the ability to connect a Workfront group to a Frame.io account_

* A new Frame.io team will be created within Frame.io representing the connected Workfront group 

**Potential improvements in future releases:** 

* Disconnect a Workfront group from a Frame.io account 

* Connect a Workfront group to an existing Frame.io team 

### Project coordinators can configure which Workfront projects are sent to Frame.io and have the assigned Creatives in Workfront added to it the project in Frame.io 

* Ability to mark Workfront projects as Frame.io enabled by assigning a Frame connected group 

* _Enhancement: Ability to toggle tasks inside Workfront projects as Frame tasks which in turns will create task folders inside Frame.io_

* When a Workfront project status is set to Current, a corresponding connected project is created in Frame, Workfront assigned users are add to the Frame project, and an email notification is sent to them from Frame.io 

    * All Workfront Project members (users and teams) will be added as Collaborators to the Frame.io project (on project creation and later) 

    * _Change: Users and teams assigned to Frame enabled Workfront tasks will be added as Collaborators to the Frame.io project and notified (on project creation and later)_ 

* Documents (Creative Briefs) added to the project and Frame enabled tasks will be pushed to the Frame.io project (within respective work folder) when the project gets created (trigger: project status set to Current) 

    * We recommend you limit the amount of documents added to your project prior to becoming active to your creative briefs only, to avoid send multiple unnecessary documents to Frame.io 

* _Enhancement: Users / teams explicitly unassigned from a frame enabled Workfront task  will be removed from the Frame.io project_

**Potential improvements in future releases:**

* Frame enabled tasks can be configured on project templates 

* New version uploads to creative briefs will be pushed to Frame 

* Optimized project synchronization (disconnecting projects, resyncing projects and documents, etc.) 

### Within Frame.io,Creatives can send created assets to the Workfront project for formal review 

* Ability to connect single Frame.io asset to a WF project or task. An asset reference will be created within Workfront  

* New version uploads inside Frame.io will automatically create new document version within Workfront on connected assets 

* _Enhancement: Ability to mark the referenced Workfront tasks as complete from within Frame.io_

* _Enhancement: In case the connected Workfront document gets deleted it remains within Frame.io and can be reconnected to the same or other project task_

**Potential improvements in future releases:** 

* Ability to send multiple Frame.io assets to Workfront at once 

* Time logging against Workfront project/task from within Frame.io 

### Project coordinators can assign the formal approval process to documents linked from Frame.io 

* Workfront users and teams can be added to new document approvals for Frame.io connected documents 

* _Enhancement: When a user / team is unshared from a Frame enabled document, then they will  also lose their access to the asset in Frame.io Viewer_ 

**Potential improvements in future releases:** 

* Send multiple assets as a single review 

* Bulk assign approvers / reviewers to Workfront documents 

### Stakeholders can conduct their review and approval within Frame.io Viewer 

* Stakeholders will be notified and can view the Frame connected document within the Frame.io Viewer 

* Frame.io Viewer can be accessed from different locations inside Workfront, e.g. Document list, Document details, Workfront Home 

* Ability to harness the existing review & commenting capabilities provided by the Frame.io Viewer which will be synchronised with the Workfront's Update Stream 

* _Ability to make a new document approval decision from within the Frame.io Viewer_ 

### Within Frame.io, Creatives will be informed about the overall decision made on the connected Frame.io asset 

* _Enhancement: Overall document approval status will be displayed on asset inside Frame.io_ 

### Project coordinators can send final assets to AEM  

* _Enhancement: Frame connected documents including metadata can be sent to AEM using the existing Workfront + AEM Asset CS connector_
