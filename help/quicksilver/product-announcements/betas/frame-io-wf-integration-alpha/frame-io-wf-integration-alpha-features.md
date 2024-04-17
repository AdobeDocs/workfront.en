---
content-type: reference
navigation-topic: betas
title: 'Adobe Workfront and Frame.io native integration beta: features'
description: Planned features for the Adobe Workfront and Frame.io native integration beta
author: Nolan
feature: Product Announcements
hide: yes
hidefromtoc: yes
exl-id: a1603a06-957b-4d52-89f3-f0cec1a4e02c
---
# Adobe Workfront and Frame.io native integration beta: features and testing

With this integration, our goal is to allow creatives to stay in their tool of choice (CC or Frame.io) to conduct their content creation and peer reviews, while having project managers coordinate the work and initialize and monitor the formal review process from inside Workfront. This can be achieved by utilizing the best of both solutions: Workfront's new document approvals for managing content approvals, in conjunction with the content review capabilities offered by Frame.io. Collectively, the new document approvals and Frame.io are going to form our new end-to-end content review and approval experience.  
 
To learn more about how the beta will function and ways you can participate, see [Adobe Workfront and Frame.io integration beta: overview](/help/quicksilver/product-announcements/betas/frame-io-wf-integration-alpha/frame-io-wf-integration-alpha-overview.md).

>[!NOTE]
>
>In case you came across these pages without your company participating in this beta program, please make sure to treat the information here with care and reach out to your Workfront or Frame.io administrator for more information.
>

## Demo Video

>[!VIDEO](https://video.tv.adobe.com/v/3426406/)

## Basic test scenario 

To allow you to easily test the new features of the beta program, we've created a new test Frame.io account and connected it to a new group called `Frame.io testing` in your existing Workfront Preview or Sandbox environment.

To test the functionality, please log in to your Workfront Preview or Sandbox instance and perform the following steps: 

1. **Coordinators:** Within Workfront, create a project with the `Frame.io testing` group assigned as the project group. 

1. **Coordinators:** Within Workfront, mark the tasks that require creative work as frame-enabled (in task details) and assign your creatives to it (assign yourself as well if you would like to test the whole workflow). 

>[!NOTE]
>
>Subtasks cannot be marked as Frame enabled.
>

1. **Coordinators:** Upload your creative brief and change the project status to "Current".

1. **Creatives:** Check your emails for an invite to the newly created Frame.io project 

1. **Creatives:** Click the "Join project" button within the invitation email to join the Frame.io project, review the creative brief within the project and start your content creation within your Creative Cloud tool of choice. 

1. **Creatives:** Upload your created assets to Frame.io and add them to the linked Workfront project by selecting one of the assigned Frame-enabled tasks. Select the option to mark the task as complete. 

1. **Coordinators:** Within Workfront, find the linked Frame.io assets in the frame-enabled task and check that the task's status was changed to "complete".

1. **Coordinators:** Assign reviewers/approvers to the linked Frame.io asset. Assign yourself as an approver as well if you would like to test the entire workflow. (For more information on assigning reviews/approvers, see [Add additional approvers or reviewers to a document](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/add-additional-reviewers-or-approvers.md)). 

1. **Stakeholders:** Within Workfront, view your approval request in Home, Document Details, or in the received email notification. Open the asset in the Frame.io Viewer, leave a comment containing feedback, and make a decision.

1. **Coordinators:** Within Workfront, view the stakeholder created comments within the Updates section of the Frame.io connected document, as well as the decision within the Approval section or document summary pane.

1. **Creatives:** Within Frame.io, notice the overall approval decision made for your assets. 

1. **Creatives:** Within Frame.io, apply the requested changes by adding the updated version to the version stack of the connected asset. 

1. **Coordinators:** Within Workfront, assign approvers/reviewers to the newly uploaded version and monitor the progress until it reaches sign-off. 

## Detailed test scenario

For participants looking to test additional functionality, we've created a more involved test scenario. A guide for this detailed test scenario can be downloaded here: [WF + Frame.io Detailed Test Scenario Walkthrough](/help/quicksilver/product-announcements/betas/assets/MVP-WF-Frame-Detailed-Walk-Through.pdf).



## Feature plans

Below is information about the primary use cases we are looking to address and the features we currently have planned to do so. <!--, along with documentation to get you started testing.--> 

>[!NOTE]
>
>Bullets under a **"Potential improvements in future releases"** header may or may not be included in a future release, depending on beta feedback and our evolving development plans. 
>

### Workfront admins can set up a connection between Workfront groups and Frame.io accounts 

* Within Workfront, you have the ability to connect a Workfront group to a Frame.io account

* A new Frame.io team will be created within Frame.io representing the connected Workfront group (Please note that this feature has only been enabled for customers using the integration on Production. Customers still testing on Sandbox or Preview will have the connection configured by the Adobe team.)

**Potential improvements in future releases:** 

* Disconnect a Workfront group from a Frame.io account 

* Connect a Workfront group to an existing Frame.io team 

### Project coordinators can configure which Workfront projects are sent to Frame.io and have the assigned Creatives in Workfront added to it the project in Frame.io 

* Ability to mark Workfront projects as Frame.io enabled by assigning a Frame connected group 

* Ability to toggle tasks inside Workfront projects as Frame tasks which in turns will create task folders inside Frame.io

* Given a Workfront project has a Frame-connected group assigned and at least one Frame-enabled task, when the Workfront project status is set to Current, a corresponding connected project is created in Frame, Workfront assigned users are add to the Frame project, and an email notification is sent to them from Frame.io 

    * Users and teams assigned to Frame enabled Workfront tasks will be added as Collaborators to the Frame.io project and notified (on project creation and later) 

* Documents (Creative Briefs) added to the project and Frame enabled tasks will be pushed to the Frame.io project (within respective work folder) when the project gets created (trigger: project status set to Current) 

    * We recommend you limit the amount of documents added to your project prior to becoming active to your creative briefs only, to avoid send multiple unnecessary documents to Frame.io 

    * Documents/tasks added after the initial project synchronization won't be pushed to Frame.io, only users/teams

**Potential improvements in future releases:**

* Frame enabled tasks can be configured on project templates 

* New version uploads to creative briefs will be pushed to Frame 

* Optimized project synchronization (disconnecting projects, resyncing projects and documents, etc.) 

### Within Frame.io,Creatives can send created assets to the Workfront project for formal review 

* Ability to connect single Frame.io asset to a WF project or task. An asset reference will be created within Workfront  

* New version uploads inside Frame.io will automatically create new document version within Workfront on connected assets 

* Ability to mark the referenced Workfront tasks as complete from within Frame.io

* In case the connected Workfront document gets deleted it remains within Frame.io and can be reconnected to the same or other project task

**Potential improvements in future releases:** 

* Ability to send multiple Frame.io assets to Workfront at once 

* Time logging against Workfront project/task from within Frame.io 

### Project coordinators can assign the formal approval process to documents linked from Frame.io 

* Workfront users and teams can be added to new document approvals for Frame.io connected documents 

* When a user/team is unshared from a Frame enabled document, then they will  also lose their access to the asset in Frame.io Viewer 

**Potential improvements in future releases:** 

* Send multiple assets as a single review 

* Bulk assign approvers/reviewers to Workfront documents 

### Stakeholders can conduct their review and approval within Frame.io Viewer 

* Stakeholders will be notified and can view the Frame connected document within the Frame.io Viewer 

* Frame.io Viewer can be accessed from different locations inside Workfront, e.g. Document list, Document details, Workfront Home 

* Ability to harness the existing review & commenting capabilities provided by the Frame.io Viewer which will be synchronised with the Workfront's Update Stream 

* Ability to make a new document approval decision from within the Frame.io Viewer 
