---
title: Use the Project Coordinator collaborator
content-type: reference
description: Learn how to use the Project Coordinator, an out-of-the-box AI Collaborator that monitors project status and follows up on overdue tasks.
author: Becky
feature: Work Management, Projects

---
# Use the Project Coordinator collaborator

{{highlighted-preview-article-level}}

The Project Coordinator is an out-of-the-box AI Collaborator that monitors your project and notifies stakeholders about important status information.

Using a Project Coordinator does not require you to configure an agent outside of Workfront.

For instructions on configuring a Project Coordinator, see [Configure a Project Coordinator](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/configure-ai-collaborators.md#configure-a-project-coordinator) in the article Configure AI Collaborators.

For information about AI Collaborators generally, see [Configure AI Collaborators](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/configure-ai-collaborators.md).

## Access requirements

+++ Expand to view access requirements for the functionality in this article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Adobe Workfront] package</td> 
   <td><p>Select, Prime, or Ultimate</p></td> 
  </tr> 
  <tr> 
   <td>[!DNL Adobe Workfront] license</td> 
   <td><p>[!UICONTROL Standard]</p></td>
  </tr> 
  <tr> 
   <td>Object permissions</td> 
   <td>You must have Manage permission to projects to assign a Project Coordinator.</td> 
  </tr>
  </tbody> 
</table>

For information, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Project Coordinator overview

The Project Coordinator monitors your project and helps keep work on track. When assigned to a project, it sends project updates on a schedule that your administrator configures. Updates can include:

* A summary of progress
* Project health
* Overdue or at-risk tasks or approvals
* Missing fields or assignments

The Project Coordinator can also comment on the project and its tasks.

Your administrator configures how often updates are sent, the time they are sent, and who receives them.

You can also run the Project Coordinator on demand by mentioning it in an update on the project. The Project Coordinator runs when it is mentioned, even if it is not scheduled to run at that time.

>[!NOTE]
>
>Project Coordinator behavior may change before general availability.

## Add the Project Coordinator to a project

An administrator must first create the Project Coordinator and add the **Project Coordinator** field to the project header in your layout template. Then the field appears in the project header.

For more information, see [Customize object headers using a layout template](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-object-headers.md).

To assign a Project Coordinator to a project:

1. Go to the project for which you want to assign a Project Coordinator.
1. In the project header, Click the **Project Coordinator** field.
1. Select the Project Coordinator you want to assign.

   The window displays a description of the selected Project Coordinator, as well as the actions that the Project Coordinator performs.
1. Click **Apply**.

## Run the Project Coordinator by mentioning it

In addition to its scheduled updates, you can trigger the Project Coordinator at any time by @mentioning it in an update on the project. The Project Coordinator runs as soon as it is mentioned, even if it is not scheduled to run at that time.

To mention the Project Coordinator:

1. Go to the project that has the Project Coordinator assigned.
1. Open the **Updates** area of the project.
1. In the update field, type **@** and select the Project Coordinator.
1. Add your message, then post the update.

   The Project Coordinator runs and posts its response.

>[!NOTE]
>
>The Project Coordinator must be assigned to the project before you can trigger it with an @mention.

## Configure the Project Coordinator

For instructions on configuring the Project Coordinator, see [Configure the Project Coordinator](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/configure-ai-collaborators.md#configure-a-project-coordinator) in the article Configure AI Collaborators.
