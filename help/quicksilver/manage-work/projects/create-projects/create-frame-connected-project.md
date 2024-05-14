---
product-area: projects
navigation-topic: create-projects
title: Create a project connected with Frame.io
description: A project is a large unit of work in Adobe Workfront. You can create projects from scratch, use a template, or convert issues or tasks to projects.
author: Courtney
feature: Work Management

---

# Create a project connected with Frame.io

The Workfront and Frame.io integration allows you to create projects in Workfront that are mirrored in Frame.io, providing a seamless review and approval experience. 

When a Workfront project is connected with Frame.io, you can 

* **Assign Frame.io users to tasks**: Frame.io enabled users are notified by email when they are assigned to a Workfront task, signaling there is work to complete. 
* **Share the project with Frame.io users**: When a project is shared with Frame.io enabled users, they have access to the project inside both Workfront and Frame.io.
* **Share creative materials with Frame.io**: Project coordinators can send instructions and materials from Workfront directly to the creative user in Frame.io using a one-way sync project folder. [!BADGE Coming soon]{type=Informative}
* **Track task progress**: Creatives can send finished assets and mark tasks complete--all without leaving Frame.io.

## Access requirements

>[!IMPORTANT]
>
>This functionality is available only to organization that have been onboarded to the [!DNL Adobe Admin Console].

You must have the following:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license</td> 
   <td> <p>Standard</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>Edit access to Projects</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>When you create a project, you automatically receive Manage permissions to the project.</p> </td> 
  </tr> 
 </tbody> 
</table>

For more detail about the information in this table, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Prerequisites

* Set up the default Frame.io account in the Workfront setup area 
* Enable Frame.io users in the Workfront user profile

For more information about the prerequisites above, see [Configure the [!DNL Workfront] and [!DNL Frame.io] integration](/help/quicksilver/administration-and-setup/configure-integrations/configure-wf-and-frame.md).


## Create a new project template

When building a new template, you can enter the information for all tasks and for your future project settings. This information will then transfer to any project that you create from the template.

Projects in Frame.io are organized by team, and 

Workfront groups are associated with Frame.io teams. 

To organize projects by team inside of Frame.io, you have to assign the correct Workfront group to the project before it's created.  

We recommend using a project template to create connected projects because you can set the project group before.

If you choose to create the project from scratch, Workfront automatically adds the Default project group and the mirror Frame.io project is created under that default team in frame.io. Updating the group after project creation does not change the Frame.io team. 

### Create the template and specify the project group

{{step1-to-templates}}

1. Click **New Template**. 
1. Type a name for your template. Press Enter to save the name.
1. In the left panel, click **Template Details**.
1. In the **Template association** section, make sure to specify a group. If you do not add a group, the default project group is added and the project in Frame.io is created under that corresponding frame.io team.

Continue to the next section.

![](assets/template-group.png)

### Add tasks and assign Frame.io enabled users

1. In the left panel, click **Template Tasks**.
1. Click **Start Adding Template Tasks** to quickly add tasks to your template. You can configure additional settings later. 

   Or

   Click **New Template Task** to add one task at a time and configure additional settings.
   ![](assets/add-tasks-to-template.png)
1. Add a task name.
1. In the **Assignments** area, assign users or teams. If you assign a Frame.io enabled user, either individually or in a team, they are granted collaborator access to the Frame.io project and notified about the task in the Frame.io project via email. From that email, they can join the Frame.io project and begin work. 
1. Repeat steps 1 and 2 as needed.

Continue to the next section.

### Configure additional template details 

Workfront has robust project management capabilities. We recommend using the [Edit project templates](/help/quicksilver/manage-work/projects/create-and-manage-templates/edit-templates.md) article to configure the following areas of the template:

   * Overview
   * Finance
   * Custom Forms
   * Project Settings
   * Tasks Settings
   * Issue Settings
   * Access

### Create a project from the template

Once you create a template, you can use it to create projects. 

{{step1-to-projects}}

1. Click **New Project from Template**. 
1. Using the search box, begin typing the name of the template you need. 
1. Select the template name, then click **Use template**. 
   ![](assets/find-your-template.png)
1. Adjust any project settings as needed, then click **Create project**. 
1. In the left panel, click **Documents**. 
1. Use the one-way sync folder to automatically share creative materials with Frame.io. [!BADGE Coming soon]{type=Informative}

   >[!NOTE]
   >
   >This feature is currently in development. To share information with users in Frame.io, upload the files to the Document tab. When the status of the project is set to current, those files automatically push to Frame.io

1. In the project header, change the project from **Planning** to **Current**. 

After the project is created and creatives upload finished assets, you can assign a review and approval workflow to the asset in Workfront. For more information, see [Create a document review or approval request](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-a-document-approval.md). <!-- name may need to change -->

## Create a new project from scratch

You can create a new project from scratch as needed. 

>[!IMPORTANT]
>
>Projects in Frame.io are organized by team, and Workfront groups are associated with Frame.io teams. To organize projects by team inside of Frame.io, you have to assign the correct Workfront group to the project before it's created.  
>
>If you choose to create the project from scratch, Workfront automatically adds the Default project group and the mirror Frame.io project is created under that default team in frame.io. Updating the group after project creation does not change the Frame.io team. 

### Create the project

{{step1-to-projects}}

1. Click **New Project**. 
1. Type a name for your project. Press Enter to save the name.

Continue to the next section.

### Add tasks and assign Frame.io enabled users

1. In the left panel, click **Tasks**.
1. Click **Start Adding Tasks** to quickly add tasks to your project. You can configure additional settings later. 

   Or

   Click **New Task** to add one task at a time and configure additional settings.
   ![](assets/add-project-tasks.png)
1. Add a task name.
1. In the **Assignments** area, assign users or teams. If you assign a Frame.io enabled user, either individually or in a team, they are granted collaborator access to the Frame.io project and notified about the task in the Frame.io project via email. From that email, they can join the Frame.io project and begin work. 
1. Repeat steps 1 and 2 as needed.

Continue to the next section.

### Upload creative materials

1. In the left panel, click **Documents**. 
1. Use the one-way sync folder to automatically share creative materials with Frame.io. [!BADGE Coming soon]{type=Informative}

   >[!NOTE]
   >
   >   This feature is currently in development. To share information with users in Frame.io, upload the files to the Document tab. When the status of the project is set to current, those files automatically push to Frame.io

Continue to the next section.

### Configure additional project details 

Workfront has robust project management capabilities. We recommend using the [Edit projects](/help/quicksilver/manage-work/projects/manage-projects/edit-projects.md) article to configure the following areas of the project:

   * Overview
   * Finance
   * Custom Forms
   * Project Settings
   * Tasks Settings
   * Issue Settings
   * Access

### Set the project to current

1. In the project header, change the project from Planning to Current. 
After the project is created and creatives upload finished assets, you can assign a review and approval workflow to the asset in Workfront. 

After the project is created and creatives upload finished assets, you can assign a review and approval workflow to the asset in Workfront.

For more information, see [Create a document review or approval request](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-a-document-approval.md). <!-- name may need to change -->