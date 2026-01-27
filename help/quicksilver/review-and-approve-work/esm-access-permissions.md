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
---

# Object permissions and access level overview for the Adobe enterprise storage model

<!--linked in UI -->

Adobe enterprise storage is a cloud-based storage solution that serves as the central repository for assets across Adobe enterprise products. Workfront environments that use Adobe enterprise storage have different permission and access level behaviors than legacy Workfront document storage. 

## Access levels

Workfront access levels apply only within Workfront. Users with project-level permissions on Adobe enterprise storage projects can still view and manage documents for those projects in other Adobe tools, such as Frame.io and Adobe Creative Cloud.

### Key differences between Adobe enterprise storage and legacy Workfront storage

Document access behaves differently depending on whether the project is on Adobe enterprise storage or legacy Workfront storage: 

* **Legacy Workfront storage**: Projects, programs, and portfolios that use legacy Workfront storage follow standard Workfront access level logic for document access. When has "no access" they are unable to see documents in Workfront or other Adobe products like Frame.io or Creative Cloud.
* **Adobe enterprise storage**: Projects, programs, and portfolios that use Adobe enterprise storage follow Adobe enterprise storage access level logic for document access. Users with project-level permissions can view and manage documents for those projects in other Adobe tools, even if they have "no access" in Workfront.

If you have Adobe enterprise storage enabled in your Workfront environment, you can create both Adobe enterprise storage projects and legacy Workfront storage projects. 

Legacy Workfront storage projects show an icon next to the project name whereever it displays in Workfront. Adobe enterprise storage projects do not show an icon.


### Specific behaviors environments that only use Adobe enterprise storage 

If ESM, Documents access - you cannot change access levels to have no access or view access to document. They also always have the option to create, delete, and share. - esm only envs?

Also if ESM, the option to never inherit document access permissions is no longer there. - esm only envs?

Document access cannot be restricted at the access level for ESM projects.- ESM only envs?

project name also available outside of WF for ESM projects, programs, portfolios. templates


Option 1
This setting only applies within Workfront. Users with project-level permissions on enterprise storage projects can still view and manage documents for those projects in other Adobe tools. Learn more.
Option 2
This setting only applies within Workfront. If a user has project-level permissions on an enterprise storage project, they can manage and view related documents in other Adobe tools. Learn more.


## Projects

Projects that use Adobe enterprise storage are available in other Adobe tools like Frame.io and Adobe Creative Cloud. 


Users with project-level permissions can manage and view documents for this project in other Adobe tools.

Project names are also visible outside of Workfront for ESM projects.

## Tasks and issues

Documents are stored at the project level but able to be shared to individual tasks and issues as needed. Users with task and issue access automatically in herit document access from the project. YOu cannot modify their level of access. They hava manage access or no access. 