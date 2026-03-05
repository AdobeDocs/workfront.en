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

Object permissions are different on projects using ESM storage. 

## Project permissions

Users with project-level permissions can view and manage documents for projects in other Adobe products like Frame.io and Adobe Creative Cloud. They will also see project names in other Adobe products. 

## Tasks and issues permissions

Documents are stored at the project level can be associated with tasks and issues. Tasks and issues inherit permissions from the project but can be refined at the task level. 

Users with task and issue access automatically inherit document access from the project. You cannot modify their level of access. They can have manage access or no access.

## Document permissions

Individual document permissions are not available for projects using Adobe enterprise storage. Instead, document permissions are determined at the project, task, or issue level.

Users with access to the project, task, or issue will have access to all documents associated with that object. You cannot modify their level of access. They can have manage access or no access.

Folders and subfolders do not have permissions and inherit permissions from the project, task, or issue. You cannot modify their level of access. They can have manage access or no access.

Any documents outside of a folder at the project level cannot be seen at the task level. 

THe only way to see tasks at the task and issue leves is through folders. 

### Folders



### Approvals

When a user is added to a document approval workflow, they will be able to see the following information in Workfront and other Adobe products, such as Frame.io and Adobe Creative Cloud, regardless of project permissions:

* Project name
* Document name
* Document thumbnail 




## Document permissions and folder sharing



### Document permissions

Document permissions are determined by 



folder access in Adobe enterprise storage. Document permissions are inherited from the folder they are uploaded to. Document permissions cannot be changed directly on the document. Instead, folder sharing and permissions must be managed to manage document permissions. Document permissions are inherited from the folder they are uploaded to.


behavior is driven by folder access and document-to-work-item associations.

* Folders can be shared with users using supported ESM permission levels.
* Users can be added to a folder even if they are not added to the related task or issue.
* Project managers can share folders from the project level in ESM environments.
* Sharable folder is created on upload. 
* Users cannot upload a document outside of a folder.
* Documents in a folder inherit that folder's linked object.
* A document that inherits from its folder cannot be reassigned unless it is moved out of that folder.
* Subfolders inherit associations from their parent folder.
* At the project level, users can see which task or issue a document or folder is connected to.
* Documents outside of folders at the project level are only available to users with project level access. 

Users with task level access only will only see doucments in the folder associated with that task. 

Workfront access-level controls still apply in Workfront, but folder sharing and permissions are managed through Adobe Enterprise Storage folder access behavior and may result in different access than expected outside of Workfront. For example, a user with **No access** to documents but with project-level permissions may still have access to documents in other Adobe products like Frame.io and Adobe Creative Cloud.



### Linked objects

Linked objects are a way to associate document folders with tasks and issues. Linked objects can be changed at the project level. When a user uploads a document to a task or issue, a primary folder is automatically created and linked to that task or issue.




on task 
Inherited perissions when turned on people will get access to the documents





External shared can be on task 

anyone without project acess removed from a task will retain access on the project 






## Project, task, and issue permissions

Users with project-level permissions can view and manage documents for projects in other Adobe products like Frame.io and Adobe Creative Cloud. Project names are also visible outside of Workfront for ESM projects. Financial data is not visible outside of Workfront for ESM projects.

### Tasks

Tasks use a primary folder model for document uploads.

* Project managers can view all folders on a task.
* When a document is uploaded to a task, a primary folder is created automatically if one does not already exist.
* Additional folders created inside a primary folder inherit that folder's permissions.
* Primary folders can be renamed and moved.
* If a primary folder is moved, its link to the task is broken.
* Adding a user to a task automatically shares that task's primary folder with the user.
* Removing a user from a task does not automatically remove that user's folder access.
    you can choose what access to remove. If just task access is removed, users can access the folder at the project leve. 
* Subtasks do not inherit primary folder permissions from parent tasks. Only users directly added to a task are added to that task's primary folder.

### Issues

Issues follow the same behavior as tasks.

* Project managers can view and manage issue folders the same way they manage task folders.
* Primary folders for issues follow the same creation, sharing, rename, move, and link behavior as task primary folders.
* If a user has issue access but not folder access, uploads are blocked and an error is shown.