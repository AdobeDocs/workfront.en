---
filename: create-templates-from-examples
product-area: templates
navigation-topic: templates-navigation-topic
title: Create project templates from examples
description: You can build templates based on the example templates described in this article.
---

# Create project templates from examples

>[!IMPORTANT]
>
>You're currently viewing the Adobe Workfront Classic version of this document. Adobe Workfront Classic is no longer supported. All Adobe Workfront Classic functionality, along with this documentation, will be removed in July 2022. Please transition to the the new Adobe Workfront experienceas soon as possible, and switch to the new Adobe Workfront experience version of this document.

You can build templates based on the example templates described in this article.

This catalog contains a number of .xml project files that you can add to your Adobe Workfront instance by importing them as Microsoft projects. Once you import them, they become Workfront projects which you can save as your own project templates.

If your organization uses the new Adobe Workfront experience, we recommend that you speak with your Workfront administrator and ask them to down templates using Blueprints. For more information, see [Configure a project template blueprint](https://one.workfront.com/s/document-item?bundleId=the-new-workfront-experience&topicId=Content%2FAdministration_and_Setup%2FBlueprints%2Fconfigure-template-package.htm&_LANG=en).

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: link above is hardcoded)</p>
-->

## Access requirements

You must have the following to perform the actions in this article:

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Projects and Templates</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>You have Manage permissions to the templates you create, by default </p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your Workfront administrator.

## Download a template to Workfront from an existing template

1. Download the zipped XML file from the lists below, by clicking the template name that you want to build. See [Available templates](#available-templates).
1. Unzip the file on your desktop.
1. Extract the .xml file from the downloaded .zip file and save it somewhere on your computer. 
1. In Workfront, go to the **Projects** area in the Global Navigation Bar and select the **Projects** tab.  

1. Click the **New** **Project** drop-down menu, and select **Import MS Project**.

1. Browse for the .xml file you extracted from the .zip file and complete the steps of the import wizard.  
   This adds the template to Workfront as a project.
1. Click **Project Actions** on the project you have imported.  
1. Select **Save as Template**.
1. Consider specifying the following information:

   * **Template Name**: Specify the name of the template.  
   
   * **Description**: Add a description of your template.  
   
   * Select a custom form from the **Add Forms** drop-down menu.

1. Click **Next Step**.
1. Select the information that you want to clear in the template.
1. Click **Next Step**.
1. Select the tasks that you want to exclude from the template. The tasks you select here will not be included in the template. 
1. Click **Finish and Save Template.**

## Available templates  {#available-templates}

Various project templates are available, depending on the type of project that you are creating. While the templates in the following sections were created with a specific purpose in mind, a templates can be used for other types of projects.

* [Marketing project templates](#marketing-project-templates) 
* [IT project templates](#it-project-templates) 
* [Other project templates](#other-project-templates) 
* [Workfront implementation templates](#workfront-implementation-templates)

### Marketing project templates {#marketing-project-templates}

The templates in this section include direct mail, events, micro-sites, video, and more. While intended for marketing processes, these templates can be used for other types of projects.

Each template provides industry standard workflow guidelines to get you started and can be customized to fit your organization’s processes.

* [Broadcast Workflow Template](https://cdn.experience.workfront.com/Documentation/Project+template+examples/Marketing+projects+templates/Broadcast_Workflow_Template+(3).zip) 
* [Digital Workflow Template](https://cdn.experience.workfront.com/Documentation/Project+template+examples/Marketing+projects+templates/Digital_Workflow_Template.zip) 
* [Direct Mail Template](https://cdn.experience.workfront.com/Documentation/Project+template+examples/Marketing+projects+templates/Direct_Mail_Template_Template.zip) 
* [Event Workflow Template](https://cdn.experience.workfront.com/Documentation/Project+template+examples/Marketing+projects+templates/Event_Workflow_Template.zip) 
* [Integrated Campaign Workflow Template](https://cdn.experience.workfront.com/Documentation/Project+template+examples/Marketing+projects+templates/Integrated_Campaign_Workflow_Template.zip) 
* [New Microsite Template](https://cdn.experience.workfront.com/Documentation/Project+template+examples/Marketing+projects+templates/New_Microsite_Template.zip) 
* [Print OOH Workflow Template](https://cdn.experience.workfront.com/Documentation/Project+template+examples/Marketing+projects+templates/Print_OOH_Workflow_Template+(1).zip) 
* [Video Workflow Template](https://cdn.experience.workfront.com/Documentation/Project+template+examples/Marketing+projects+templates/Video_Workflow_Template.zip) 
* [Video Commercial Template](https://cdn.experience.workfront.com/Documentation/Project+template+examples/Marketing+projects+templates/Video_Commercial_Template.zip)

### IT project templates {#it-project-templates}

* [IT: Disaster Recovery](https://cdn.experience.workfront.com/Documentation/Project+template+examples/IT+projects+templates/Disaster_Recovery.zip)   
  This template outlines the activities that an IT team would need to complete as part of a Disaster Recovery project.

* [IT: Governance](https://cdn.experience.workfront.com/Documentation/Project+template+examples/IT+projects+templates/IT_Governance.zip)   
  This template provides a generic outline of activities completed by an IT team subscribing to ITG principles.

* [IT: Infrastructure Deployment Plan](https://cdn.experience.workfront.com/Documentation/Project+template+examples/IT+projects+templates/Infrastructure_Deployment_Plan.zip)   
  This template provides a generic outline of activities completed by an IT team to enhance systems/ infrastructure.

* [IT: Security Infrastructure Improvement Plan](https://cdn.experience.workfront.com/Documentation/Project+template+examples/IT+projects+templates/Security_Infrastructure_Improvement_Plan.zip)   
  This template represents an example of a Security Infrastructure Improvement Plan project.

   * In the Initiation Phase, you will find tasks for developing a charter, preliminary technical assessments, business requirements, etc.
   * In the Planning Phase, a more detailed plan is developed and tasks are inserted into place-holder spots within the Construction, Testing, Deploy, and Close phases.
   * In the Planning Phase, a more detailed plan is developed and tasks are inserted into place-holder spots within the Construction, Testing, Deploy, and Close phases.
   * The Construction phase contains a number of tasks that are required for each iteration of the project and place-holders for specific development activities.
   * The Testing phase contains place-holders for Quality Assurance and User Acceptance Test activities, as well as Customer approval.
   * The Deploy phase provides a location where, during the Planning phase, tasks can be added to outline specific steps to go live with the product and pass maintenance off to an operations team.
   * In the Close phase, you will find tasks to finalize the project plan; including, development and presentation of training materials and documentation. It also contains a task representing a post-mortem meeting.

* [Software Development Lifecycle](https://cdn.experience.workfront.com/Documentation/Project+template+examples/IT+projects+templates/Software_Development_Lifecycle.xml_.zip)   
  This Software Development Lifecycle (SDLC) template was created for a customer who followed a traditional waterfall methodology for their development processes.  
  The template features parent tasks that represent the major phases of the project. The names used to describe their phases are: Initiation, Planning, Construction, Testing, Deploy, and Close.

### Other project templates {#other-project-templates}

The templates in this section range from suggested Workfront implementation schedules to software development life cycles to industry-specific workflows across a number of verticals.​

* [ [Finance: Monthly Closeout](https://cdn.experience.workfront.com/Documentation/Project+template+examples/Other+project+templates/Monthly_Closeout.zip)](https://documentation.my.workfront.com/library/a/75891a99-98fb-421b-b0b5-494903aa3d4d)   
  This is an example of the steps a Finance team may complete as a repeated process for Monthly Closeout activities.
* [ [Product Development: Generic](https://cdn.experience.workfront.com/Documentation/Project+template+examples/Other+project+templates/Product_Development+_Generic.zip)](https://documentation.my.workfront.com/library/a/51771358-00fc-47cb-8f14-1801f6cf5bca)   
  This template is a generic outline of activities to be completed for new product development projects.
* [ [Product Development: Pharmaceuticals](https://cdn.experience.workfront.com/Documentation/Project+template+examples/Other+project+templates/Product_Development_Pharmaceuticals.zip)](https://documentation.my.workfront.com/library/a/8fe77243-9555-4010-969e-1c7a5ff9d8d7)   
  This template represents an outline of activities to be completed for new product development projects for pharmaceuticals.
* [Six Sigma: DMAIC Project (In Depth) Version 1](https://cdn.experience.workfront.com/Documentation/Project+template+examples/Other+project+templates/Six_Sigma_DMAIC_Project__In_Depth_v.1_.zip)   
  This template provides an in depth outline of typical activities needed to complete SixSigma's DMAIC approach to project management.
* [Six Sigma: DMAIC Project (In Depth) Version 2](https://cdn.experience.workfront.com/Documentation/Project+template+examples/Other+project+templates/Six_Sigma_DMAIC_Project__In_Depth_v.2_.zip)   
  This template provides an in depth outline of typical activities needed to complete SixSigma's DMAIC approach to project management.
* [ [Six Sigma: DMAIC Project (Simplified)](https://cdn.experience.workfront.com/Documentation/Project+template+examples/Other+project+templates/Six_Sigma_DMAIC_Project__Simplified_v.1_.xml_.zip)](https://documentation.my.workfront.com/library/a/ccdf54f2-2562-4525-9fc0-8377768b9f21)   
  This is a Simplified version of a Six Sigma DMAIC Project.

### Workfront implementation templates {#workfront-implementation-templates}

The following project plans were developed specifically to assist new Workfront customers in understanding the steps they must follow in order to implement Workfront. Each plan corresponds to the activities Workfront is committed to perform as part of each of our standard implementation programs.

* [Workfront Getting Started Template](https://cdn.experience.workfront.com/Documentation/Project+template+examples/Workfront+implementation+templates/Workfront_Getting_Started.xml_.zip)   
  ​If you are just getting started with Workfront, there are several steps you will need to take in order to be successful. The Getting Started Project Template is an outline that will walk you through the steps for an outstanding Workfront implementation.
* [The Basic Business Process Program](https://cdn.experience.workfront.com/Documentation/Project+template+examples/Workfront+implementation+templates/Basic_Business_Process_Program.xml_.zip) 
* [The Preferred Business Process Program](https://cdn.experience.workfront.com/Documentation/Project+template+examples/Workfront+implementation+templates/Preferred_Business_Process_Program.xml_.zip) 
* [The Premium Business Process Program](https://cdn.experience.workfront.com/Documentation/Project+template+examples/Workfront+implementation+templates/Premium_Business_Process_Program.xml_.zip)

