---
title: Configure the [!DNL Workfront] and [!DNL Frame.io] integration
user-type: administrator
product-area: system-administration;workfront-integrations;setup
navigation-topic: administrator-integrations
description: As an [!DNL Adobe Workfront] administrator, you can integrate [!DNL Workfront] with [!DNL Frame.io] and provide your organization with a seamless way to review and approve assets.
author: Courtney
feature: System Setup and Administration, Workfront Integrations and Apps
role: Admin

---

# Configure the [!DNL Workfront] and [!DNL Frame.io] integration

The Workfront administrator enables the integration between Workfront and Frame.io by configuring the default Frame.io account in the Setup area and then designating Frame.io users in Workfront. This allows the coordinator to plan and initiate work using Workfront Projects and formal review and approval workflows. 

## Configure a default Frame.io account

Workfront administrators initiate the Workfront and Frame.io integration by adding a default Frame.io account in the Setup area of Workfront. Once a default Frame.io account is set up, 
any projects created in Workfront have a mirror project created in Frame.io.

For more information, see [].

<!-- in procedure article we need to cover how groups work with projects and how the frame account is associated with a group. And that accounts other than the default can be added on a 1:1 basis using the dev token. -->

## Configure a single frame account with a workfront grouop

You can connect a workfront group with a frame.io account that is differnet from the default account. You can do this on a 1:1 basis.

1. go to groups
1. get dev token

## Enable Frame.io users

Workfront users who regularly use Frame.io should be marked as Frame.io users. Workfront administrators can designate Frame.io users in the Workfront User Profile.

When a user is marked as a Frame.io user in Workfront and is added to a project,

* They are added as a Collaborator in Frame.io
* They can send assets from Frame.io to Workfront for formal review and approval
* They can view information in the one-way sync folder from Workfront

To enable Frame.io users:

1. go to the user profile
1. 

>[!TIP]
>
>We recommend enabling users who regularly work in creative tools and upload assets for review and approval as Frame.io users.

For more information, see [].

![](assets/Frame-enabled-user.png)