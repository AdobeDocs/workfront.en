---
product-area: documents
navigation-topic: approvals
title: Asset review and approval overview
description: Learn more about the formal review and approval process in Workfront.
author: Courtney
feature: Work Management, Digital Content and Documents
hide: yes
hidefromtoc: yes
recommendations: noDisplay, noCatalog
exl-id: 68b91aad-af76-473f-861d-da846fdfb84c
---
# Asset review and approval overview

The new Asset review and approval workflow is built around a tight integration between Workfront and Frame.io. This integration takes the best of what each product has to offer and combines it to create an experience that allows all personas involved in content creation to work in their tools of choice, while having access to comments, files, and status updates synchronized across both systems in real time.

For more information about Frame.io, see [Getting Started with Frame.io](https://support.frame.io/en/collections/49298-getting-started).

## Work initiation and planning in Workfront

The Workfront administrator enables the integration between Workfront and Frame.io by configuring the default Frame.io account in the Setup area and then designating Frame.io users in Workfront. This allows the coordinator to plan and initiate work using Workfront Projects and formal review and approval workflows. 

### Configure a default Frame.io account

Workfront administrators initiate the Workfront and Frame.io integration by adding a default Frame.io account in the Setup area of Workfront. Once a default Frame.io account is set up, 
any projects created in Workfront have a mirror project created in Frame.io.

For more information, see [].

<!-- in procedure article we need to cover how groups work with projects and how the frame account is associated with a group. And that accounts other than the default can be added on a 1:1 basis using the dev token. -->

### Enable Frame.io users

Workfront users who regularly use Frame.io should be marked as Frame.io users. Workfront administrators can designate Frame.io users in the Workfront User Profile. 

When a user is marked as a Frame.io user in Workfront and is added to a project,

* They are added as a Collaborator in Frame.io
* They can send assets from Frame.io to Workfront for formal review and approval
* They can view information in the one-way sync folder from Workfront

>[!TIP]
>
>We recommend enabling users who regularly work in creative tools and upload assets for review and approval as Frame.io users.

For more information, see [].

![](assets/Frame-enabled-user.png)


### Create a project connected with Frame.io

Once the default Frame.io account is added and Frame.io users are designated, project coordinators can create Workfront projects connected with Frame.io. When you create a connected project, you can

* **Assign Frame.io users to tasks**: Frame.io enabled users are notified by email when they are assigned to a task, signaling there is work to complete. 
* **Share the project with Frame.io users**: Projects shared with Frame.io enabled users grants them access to the project inside Frame.io.
* **Share creative materials with Frame.io**: You can send instructions and materials from Workfront directly to the creative user in Frame.io using a one-way sync project folder. 
* **Track task progress**: Creatives can send finished assets and mark tasks complete without leaving Frame.io.

For more information, see [].

<!--Preassign approval templates to tasks coming in the future-->


## Content creation and collaboration in Frame.io

Creatives can stay in their tools of choice and have the freedom to create, iterate, and conduct peer reviews inside Frame.io. 

When a creative is added to a connected project, they can do the following without leaving Frame.io:

* Access instructions from the project coordinator
* Conduct informal peer reviews
* Send finished assets to Workfront for formal review and approval
* Change the status of a task or mark it complete 
<!-- * Notification of decision
* Upload new versions of connected assets marked as needs more work < will automatically connect>-->

For more information about reviewing assets in Frame.io, see 

## Review and approve assets

Once a creative sends a finished asset to Workfront from Frame.io, the project coordinator can initiate the formal review and approval process in Workfront. 

After the approval is created, users go back to Frame.io to comment on and markup the asset. They can also make a the approval decision in the Frame.io viewer.

### Initiate formal reviews and approvals in Workfront

Project coordinators can create one-time review and approvals or resuable Approval Templates in the Setup area of Workfront. All review and approval activity made in Frame.io is also recorded in Workfront. 

Project coordinators have the option to assign reviewers, approvers, or a mix of both:

* **Reviewers** can comment on and markup assets. Once finished, they can mark their review as complete. <!--example of when to add reviewers-->
* **Approvers** can comment on markup assets. They must make a decision to move the approval process forward. 

Any comments made in Frame.io are reflected in the Updates tab in Workfront. Replies made in Workfront are not reflected in Frame.io.

Comments marked Team only will not appear in the Workfront Updates tab.

Reviewers and approvers can be added to single-use or approval templates:

<!--can also assign teams and set deadline-->

* **Single-use approvals**: Set approval deadlines

* **Approval templates**
    In the Workfront Setup area, users with a Standard license can create resuable Approval Templates. Within a template, users can specify a timeframe and add reviewers and approvers. <!--do we want to mention any upcoming plans here? -->

    Once a template is created, it can be applied to assets sent from Frame.io to begin the formal review and approval process in Workfront.
![](assets/assign-template.png)

<!-- can set timreframe which calculates deadline once approval is started. >

    For more information, see [Create and manage Approval Templates](/)<!--don't forget link-->

* Upload an asset from Workfront and send it to frame for review and approval - Coming soon?

### Approve assets in Frame.io

Frame.io connected asset stakeholders can review and approve inside the Frame.io viewer with comments syncing to Workfront update stream, decisions, etc.

<!-- include screenshot from frame.io-->

If you work exclusively in Frame, you can be notified of a request via email. 

If you work exclusively in Workfront, you can use the approval widget in home.

you can access the Frame.io viewer from whenever you work

**Approve assets from Frame.io**
how they are notified

make a decision - approve, approve with changes, needs work

**Approve assets from Workfront**
how they are notified

Home Awaiting my approval widget

Email - deadline emails 72, 24, and on deadline.

External WF users will be asked to create a login for frame 

If the asset is not frame connected, they can view thumbnail in WF and use comment stream. Review and approval decisions can be made.

<!-- upload assets directly to workfront to be reviewed in Frame.io/ Will have to send manually at first

Reviewer/approver needs to go through email to get to frame vier
-->


### Track review and approval metrics

Widgets in home
Approval velocity report ?

<!--
### Published approved assets to Adobe Experience Manager Assets

Use the native integration to send approved assets to AEM.
-->


## Example campaign asset approval workflow

intro para?

![](assets/example-workflow.png) <!-- probbly need a different version of this but add something similar rather than typing all out?-->
