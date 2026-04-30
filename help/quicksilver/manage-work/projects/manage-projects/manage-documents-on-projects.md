---
product-area: projects
navigation-topic: manage-projects
title: Document Management Overview for Projects and Related Objects
description: Depending on whether your Workfront administrator chooses for your storage preference default, you can store documents on either legacy Workfront storage or Adobe enterprise storage. This article describes how you can manage documents for projects, portfolios, programs, templates, tasks, and issues.
author: Alina
feature: Work Management
exl-id: 5623157e-946e-4475-9df3-b1888a2a0934
---
# Document management overview for projects and related objects

Your Adobe Workfront administrator can define the default for your organization's storage preference to indicate where documents should be stored in Workfront. 

The Workfront administrator can choose one of the following options: 

* Workfront storage
* Adobe Enterprise storage

This preference allows you to automatically store documents attached to Workfront objects on one of the storage locations available. 

>[!IMPORTANT]
>
>Not all customers have access to both Workfront as well as Adobe storage. Some customers have access only to Workfront which others have access only to Adobe Enterprise storage by default. No configuration is needed for customers without access to Workfront storage.

The Workfront administrator can do one of the following:

* Choose one of the two storage options as the default for your organization
* Allow you to choose which storage you prefer to use when you create one of the following objects: 

    * Projects
    * Portfolios
    * Templates

For information about setting storage preferences for Workfront, see [Enable Adobe enterprise storage for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-esm.md).

This article describes how you can manage documents for projects, portfolios, programs, tasks, issues, templates, and template tasks.

<!--

Not sure we need these since this became an overview article: 

## Access requirements

+++ Expand to view access requirements for the functionality in this article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront package</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license</td> 
   <td> <p>Light or higher</p>
   <p>Review or higher</p>
   
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>View or higher access to the objects you want to add documents to:</p>
   <ul><li>Projects</li>
   <li>Portfolios</li>
<li>Programs</li>
<li>Templates</li> 
<li>Tasks</li> 
<li>Issues</li> </ul>  
   
</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p> View or higher permissions to the objects you want to add documents to:</p>

<ul><li>A project</li>
   <li>A portfolio</li>
<li>A program</li>
<li>A template</li> 
<li>A task</li> 
<li>An issue</li> </ul>    
   
</td> 
  </tr> 
 </tbody> 
</table>

*For more detail about the information in this table, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

-->

## Document storage overview

Customers might have access to one of the following document storage capabilities:

* Only Workfront storage. The Storage Preferences area in System Preferences does not exist. 
* Only Adobe Enterprise storage. The Storage Preferences area in System Preferences does not exist.
* Both Workfront Storage and Adobe Enterprise storage. The Workfront administrator can choose between the following: 

    * Selects a default storage environment for how documents are handled in the future.
    * Allows users to choose which storage they choose when they create the following objects: 

        * Projects
        * Portfolios
        * Templates

    >[!NOTE]
    >
    >* Tasks and issues inherit the type of storage from the project. 
    >* Template tasks inherit the type of storage from the template
    >* Programs inherit the type of storage from the portfolio. 


Documents stored on objects in Workfront storage are managed differently than those stores in Adobe enterprise storage. 

For more information, see [Adobe enterprise storage overview](/help/quicksilver/review-and-approve-work/esm-overview.md). 

The following sections document how document storage works for Workfront objects when both Workfront and Adobe enterprise storage options are in place. 

### Document management for projects

Consider the following when working with projects: 

* When you create an Adobe enterprise-storage project, Workfront creates a folder in the Documents section of the project where documents are saved. The folder name is the same name as the project. You cannot delete or manually rename the folder. The folder is renamed if you change the name of the project to match the project's new name.
* When you create or move an Adobe-enterprise storage project to a legacy Workfront-storage portfolio or program, the portfolio or program is automatically converted to an Adobe enterprise-storage object. 
* You cannot create a Workfront-storage project for an Adobe enterprise-storage portfolio or program. 

### Document management for portfolios

Consider the following when working with portfolios: 

* When you create an Adobe enterprise-storage portfolio, Workfront creates a folder in the Documents section of the portfolio where documents are saved. The folder name is the same name as the portfolio. You cannot delete or manually rename the folder. The folder is renamed if you change the name of the portfolio to match the portfolio's new name.
* When you create or move an Adobe-enterprise storage project to a legacy Workfront-storage portfolio, the portfolio is automatically converted to an Adobe enterprise-storage object.
* If the converted portfolio previously had documents attached, they continue to remain stored in Workfront storage. New documents are also stored in Workfront storage. 
* If the converted portfolio had no documents attached in Workfront storage, new documents are stored in Adobe enterprise storage.

### Document management for programs

Consider the following when working with programs: 

* When you create an Adobe enterprise-storage program, Workfront creates a folder in the Documents section of the program where documents are saved. The folder name is the same name as the program. You cannot delete or manually rename the folder. The folder is renamed if you change the name of the program, to match the program's new name.
* When you create or move an Adobe-enterprise storage project to a legacy Workfront-storage portfolio, the portfolio is automatically converted to an Adobe enterprise-storage object.
* If the converted program previously had documents attached, they continue to remain stored in Workfront storage. New documents are also stored in Workfront storage. 
* If the converted program had no documents attached in Workfront storage, new documents are stored in Adobe enterprise storage.

### Document management for tasks

Consider the following when working with tasks:

* Tasks inherit the storage type from projects. 
* When you upload a document to a task on an Adobe-storage project, Workfront automatically creates a folder in the Documents section of the task. The folder name is the same as the task. 
* You can rename and delete the document folder from the Adobe enterprise-storage task which also deletes the documents in the folder. After you add new documents to the task, the folder is automatically recreated. Deleted documents are not placed back in the folder. 
* For Adobe enterprise-storage projects, the document folder on a task displays as a subfolder on the documents folder automatically created for the project.
* You cannot copy or move a task from a Workfront-storage project to an Adobe-storage one. The reverse is also not possible. 

### Document management for issues

Consider the following when working with issues:

* Issues inherit the storage type from projects. 
* When you upload a document to an issue on an Adobe-storage project, Workfront automatically creates a folder in the Documents section of the issue. The folder name is the same as the issue. 
* You can rename and delete the document folder from the Adobe enterprise-storage issue which also deletes the documents in the folder. After you add new documents to the issue, the folder is automatically recreated. Deleted documents are not placed back in the folder. 
* For Adobe enterprise-storage projects, the document folder on an issue displays as a subfolder on the documents folder automatically created for the project.
* You cannot copy or move an issue from a Workfront-storage project to an Adobe-storage one. The reverse is also not possible. 

### Document management for project templates

Consider the following when working with templates: 

* When you create an Adobe enterprise-storage template, Workfront creates a folder in the Documents section of the template where documents are saved. The folder name is the same name as the program. You cannot delete or manually rename the folder. The folder is renamed if you change the name of the template, to match the template's new name.
* You can use a Workfront-storage template to create Workfront-storage projects; you can use an Adobe-storage template to create an Adobe-storage project. 
* You can attach a Workfront-storage template to an Adobe-storage project and this does not change the storage location of the project. 
* You can attach an Adobe-storage template to a Workfront-storage project and this does not change the storage location for the project. 

### Document management for template tasks

Consider the following when working with template tasks:

* Template tasks inherit the storage type from templates. 
* When you upload a document to a template task on an Adobe-storage template, Workfront automatically creates a folder in the Documents section of the template task. The folder name is the same as the template task. 
* You can rename and delete the document folder from the Adobe enterprise-storage template task which also deletes the documents in the folder. After you add new documents to the template task, the folder is automatically recreated. Deleted documents are not placed back in the folder.
* For Adobe enterprise-storage templates, the document folder on a template task displays as a subfolder on the documents folder automatically created for the template. 
* You cannot copy or move a template task from a Workfront-storage template to an Adobe-storage one. The reverse is also not possible.
* When you attach a document to an issue you submit to a request queue associated with Adobe storage, a folder is created for each submitted issue where the documents are stored. The folder is also added as a subfolder to the automatically created project folder on the request queue.
