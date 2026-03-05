---
product-area: documents
navigation-topic: approvals
title: Object permissions and access level overview for the Adobe enterprise storage model
description: Adobe enterprise storage permissions and access overview
author: Courtney
feature: Work Management, Digital Content and Documents
recommendations: noDisplay, noCatalog
hide: yes
hidefromtoc: yes
exl-id: 758d17e6-f31f-42b7-a9e6-6bd1821f5c15
---
# Object permissions and access level overview for the Adobe enterprise storage model

<!--linked in UI -->

Adobe enterprise storage is a cloud-based storage solution that serves as the central storage repository for assets across Adobe enterprise products. Workfront environments that use Adobe enterprise storage have slightly different object permissions and access level behaviors than those using legacy Workfront document storage. 

## Access levels

Workfront access levels apply only within Workfront. Project and Document restrictions within Workfront don't always apply in other Adobe applications.

### Environments using both Adobe enterprise storage and legacy Workfront storage

Document access behaves differently depending on whether the project is on Adobe enterprise storage or legacy Workfront storage: 

* **Legacy Workfront storage**: Projects, programs, portfolios, and templates that use legacy Workfront storage follow standard Workfront access level logic for document access. When an access level has **No access** selected for documents, they are unable to see documents in Workfront or other Adobe products like Frame.io or Creative Cloud.
* **Adobe enterprise storage**:  Projects, programs, portfolios, and templates that use Adobe enterprise storage follow Adobe enterprise storage access level logic for other Adobe products.


    * **Projects, programs, portfolios, and templates object permissions**: When an access level has **No access** selected for projects, programs, portfolios, and templates but the object is shared with them, users are unable to see the object in Workfront, but they can still view the object name and any associated documents in other Adobe tools, such as Frame.io and Adobe Creative Cloud. 
    * **Documents permissions**: When an access level has **No access** selected for documents, users are unable to see documents on projects in Workfront, but they can still view and manage documents for projects shared with them in other Adobe tools, such as Frame.io and Adobe Creative Cloud. This is because document access is determined by project-level permissions in Adobe enterprise storage, rather than Workfront access levels alone.

If you have Adobe enterprise storage enabled in your Workfront environment, you can create both Adobe enterprise storage projects and legacy Workfront storage projects. Legacy Workfront storage projects show an icon next to the project name wherever it displays in Workfront. Adobe enterprise storage projects do not show an icon.

![legacy workfront storage icon next to project name](assets/legacy-project-icon.png)


### Environments using only Adobe enterprise storage

You cannot modify document permissions at the access level for projects, programs, and portfolios that use Adobe enterprise storage. 

All access levels have edit access to documents. Project-level permissions determine document access in other Adobe tools.

You cannot restrict document inheritance access.


### Environments using only legacy Workfront storage

No changes to document access levels or behavior.

## Object permissions

Object permissions determine what users can see and do with projects, tasks, issues, and documents in Workfront. Object permissions are determined when sharing an object with a user or group.

### Project permissions

Users with project-level permissions can view and manage documents for projects in other Adobe products like Frame.io and Adobe Creative Cloud. Project names are also visible outside of Workfront for ESM projects. Other project data is not visible outside of Workfront for projects on enterprise storage.

### Task and issue permissions

Tasks and issues inherit permissions from the project, but task-level sharing can be refined. You can add users to a task or issue and by default they are given access to documents in the system-generated folder that is linked. 

Document access for tasks and issues is inherited from the project and cannot be modified at the document level. Even if a user is added to a task as View only, they receive Manage access to documents associated with that task.


* When a document is uploaded to a task, a primary folder is created automatically if one does not already exist.
* Primary folders are created with the task name can be renamed and moved. if moved to another location, the link to the task is broken and permissions are inherited from the new object. 
* Adding a user to a task shares that task's primary folder with the user.
* Removing a user from a task does not automatically remove that user's folder access. If only task access is removed, users can still access the folder through project-level access.
* Subtasks do not inherit primary folder permissions from parent tasks. Only users directly added to a task are added to that task's primary folder.

Issues and requests follow the same behavior as tasks.

### Document permissions

Individual document permissions are not available for projects using enterprise storage. Instead, document permissions are determined at the project, task, or issue level.

Users with access to the project, task, or issue will have access to all documents linked with that object. You cannot modify their level of access. Users have manage access or no access.

#### Linked objects

Linked objects are a way to associate document folders with tasks and issues. Linked objects can be changed at the project level. When a user uploads a document to a task or issue, a primary folder is automatically created and linked to that task or issue.

* If a primary folder is moved, its link to the task or issue is broken.
* Documents in a folder inherit that folder's linked object.
* A document that inherits from its folder cannot be reassigned unless it is moved out of that folder.
* Subfolders inherit associations from their parent folder.
* At the project level, users can see which task or issue a document or folder is connected to.

#### Folders

Folders and subfolders do not have permissions and inherit permissions from the project, task, or issue. You cannot modify their level of access. They can have manage access or no access.

In Adobe enterprise storage, document access is driven by folder access. Document permissions are inherited from the folder where the document is uploaded and cannot be changed directly on the document.

* Users can be added to a folder even if they are not added to the related task or issue.
* A sharable folder is created on upload.
* Users cannot upload a document outside of a folder.
* Additional folders created inside a primary or system-level folder inherit the parent folder's permissions.
* Documents outside of folders at the project level are available only to users with project-level access.
* Users with task- or issue-level access only can see documents in the folder associated with that task or issue.

#### Approvals

When a user is added to a document approval workflow, they will be able to see the following information in Workfront and other Adobe products, such as Frame.io and Adobe Creative Cloud, regardless of project permissions:

* Project name
* Document name
* Document thumbnail 










