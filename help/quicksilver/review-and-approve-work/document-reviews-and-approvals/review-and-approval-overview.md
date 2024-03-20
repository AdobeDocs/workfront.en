---
product-area: documents
navigation-topic: approvals
title: Asset review and approval overview
description: Learn more about the formal review and approval process in Workfront.
author: Courtney
feature: Work Management, Digital Content and Documents

---

# Asset review and approval overview

The new Asset review and approval workflow is built around a tight integration between Workfront and Frame.io. This integration takes the best of what each product has to offer and combines it to create an experience that allows all personas involved in content creation to work in their tools of choice, while having access to comments, files, and status updates synchronized across both systems in real time.

<!-- link to frame docs-->

## Work initiation and planning in Workfront

The project coordinator begins in Workfront. The project is created, tasks are assigned, intructions are sent.

Campaign manager creates WF project, uses synced project folder to send     information and supporting materials to creatives inside Frame.io 

Set up approval workflow from scratch or via templates 

Assign tasks 

Sets project to Current or equal to create frame project and alert creatives 

### Configure a default Frame.io account

Set up default frame account 

<!--add one frame account as default > this will apply to all groups in the sytem

Admins can still add frame accounts to groups 1:1 using the dev token 

^ cover 1:1 in procedure article -->

Workfront administrators can connect a default Frame.io account to a Workfront group. When this group is added to a project, a corresponding project is created in Frame.io. This is the type of project that should be created when review and approval is needed. 

Setup > Review & Approval

In the group area, add the frame.io account the projects will be created in
 <!--questions 
 1. How do we determine which FIO accounts the admin can see?
 2. What does this look like for project set up?
 
 
 -->

### Enable Frame.io users

Workfront users who regularly use Frame.io should be marked as a Frame.io users in their user profile by their Workfront administrator

Workfront administrators can designate Frame.io users in the Workfront User Profile. Users marked as Frame.io users are granted a Frame.io Collaborator license, saving the project coordinator extra coordination steps.

<!-- check list for users who should be marked as frame enabled? use creative persona to create this list

We recommending adding all of your users who work in Creative cloud tools
-->

When a user is marked as a Frame.io user in Workfront and is added to a project: 

* They are added as a Collaborator in Frame.io
<!-- not with GA* Tasks assigned to them appear as a folder inside of Frame.io -->
* They can send assets from Frame.io to Workfront for formal review and approval

![](assets/Frame-enabled-user.png)



### Create a project integrated with Frame.io

Project managers and coordinators can create Workfront projects integrated with Frame.io. When you create an integrated project, you can

* You can add Frame.io enabled users, desinated by the Workfront administrator, to tasks in Workfront. Frame.io enabled users are notified by email when a task is assigned to them and they have work to begin.
 <!--
* Share the project with frame users to give them access -->

* **Share with Frame.io** : Send instructions and materials from Workfront directly to the creative user in Frame.io using a one-way sync project folder. Simply drop the documents into the **Share with Frame.io** folder.

* Track the progress of work as creatives mark tasks complete directly inside of Frame.io.

For more information on created an integrated projects, see [].

<!--Preassign approval templates to asks coming in the future-->


## Content creation and collaboration in Frame.io

Creatives can stay in their tools of choice and have the freedom to create, iterate, and conduct peer reviews inside of Frame.io. 

When a creative is added to an integrated project they can do all of the following without leaving Frame.io, 

* Access instructions from the project coordinator
* Conduct informal peer reviews
* Send finished assets to Workfront for formal review and approval
* Change the status of a task or mark it complete 
<!-- * Notification of decision
* Upload new versions of connected assets marked as needs more work < will automatically connect>-->


## Review and approve assets in Workfront

Once a creative sends a finished asset to Workfront from Frame.io, the project coordinator can kick-off the formal review and approval process in Workfront. All review and approval activity is recorded in Workfront. 

<!--comments from the frame viewer coming to the update stream. update stream comments will not go to frame.io-->

### Initiate formal reviews and approvals

You can create one-time review and approvals, or you can create resuable Approval Templates in the Setup area of workfront. 

You have the option to assign reviewers, approvers, or a mix of both:

* Reviewers can comment and markup assets. Once finished, they can mark their review as complete. <!--example of when to add reviewers-->
* Approvers Can comment, markup assets and must make a decsion.

<!--can also assign teams and set deadline-->

* **Single-use approvals**
Set approval deadlines

* **Approval templates**
    In the Workfront Setup area, users with a Standard license can create resuable Approval Templates. Within a template, users can specifiy a timeframe and add reviewers and approvers. <!--do we want to mention any upcoming plans here? -->

    Once a template is created, it can be applied to assets sent from Frame.io to begin the formal review and approval process in Workfront.
![](assets/assign-template.png)

<!-- can set timreframe which calculates deadline once approval is started. >

    For more information, see [Create and manage Approval Templates](/)<!--don't forget link-->

### Review and approval notifications

Home Awaiting my approval widget
Email - deadline emails 72, 24, and on deadline.

<!-- upload assets directly to workfront to be reviewed in Frame.io/ Will have to send manually at first

Reviewer/approver needs to go through email to get to frame vier
-->
### Review and approval assets

Frame.io connected asset stakeholders can review and approve inside the frame viewer with comments syncing to workfront update stream, decisions, ect

<!-- include screenshot from frame.io-->

External WF users will be asked to create a login for frame 

If the asset is not frame connected, they can view thumbnail in WF and use comment stream. review and approval decisons can be made.

### Track review and approval metrics

Widget in home
Approval velocity report 

<!--
### Published approved assets to Adobe Experience Manager Assets

Use the native integration to send approved assets to AEM.
-->


* Upload an asset from Workfront and send it to frame for review and approval - Coming soon?

## Example campaign asset approval workflow

intro para?

![](assets/example-workflow.png) <!-- probbly need a different version of this but add something similar rather than typing all out?-->