---
product-area: templates
navigation-topic: templates-navigation-topic
title: Copy a Project Template
description: In addition to creating a project template from scratch, you can also copy an existing one and modify it.
author: Alina
feature: Work Management
exl-id: b2e0878b-8245-4e01-819d-c3746f553d95
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/6d0OXEaAdH-569LF5nuQ8wcJd-Iq7KYz8os3IOyx0yA
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
    internal-label: Work management
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
    internal-label: Administration
subfeature_v2:
  - id: b04e3dc0-3a59-45b1-aa02-b0b6d5f87eff
    internal-label: Approvals
  - id: d87de1f9-8e24-4c4d-aa4c-a403075091a1
    internal-label: Custom forms
  - id: f0dd7b45-76b5-49d4-afe3-39f436b6fbd3
    internal-label: Projects
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
---
# Copy a project template

<!--Audited: 5/2025-->

In addition to creating a project template from scratch, you can also copy an existing one and modify it in Adobe Workfront. 

## Access requirements

+++ Expand to view access requirements for the functionality in this article. 

You must have the following access.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront package</td> 
   <td> <p>Any </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license</td> 
   <td><p>Standard</p> 
   <p>Plan</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>Edit access to Templates</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View or higher permissions to a template</p>  </td> 
  </tr> 
 </tbody> 
</table>

*For information, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md). 

+++

<!--
Old:

 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan</td> 
   <td> <p>Any </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td><p>New: Standard</p> 
   <p>Current: Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>Edit access to Templates</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View or higher permissions to a template</p>  </td> 
  </tr> 
 </tbody> 
</table>
-->

## Considerations about copying templates

The following items are always copied from an existing template to a new one:

* Template Tasks
* Template Task Default information (Task Default Approval Process, Task Default Custom Forms)
* Custom forms
* Risks
* Queue Setup information
* Portfolio and Program
* Approvals
* Documents
* The days of the original template tasks transfer to the new template. You must change the Start or Completion day of the template (depending on its Schedule Mode) to update the days on the template tasks, if needed. 

The following items are never copied from an existing template to a new one:   

* Billing Rates
* User comments  

## Copy a template

<!--ensure steps and casing on the fields and buttons is accurate with unshim-->

1. Go to the template that you want to copy.
1. Click the **More** menu ![More icon](assets/more-icon.png) to the right of the template name in the header, then click **Copy**.

   The **Copy Template** box opens.

   ![Copy template box](assets/copy-template-box.png)

1. Specify a name for the template in the **New Template Name** field.

   By default, Workfront sets the new name following this format: `Copy of Original template name`.

1. Select the **Retain user assignments on tasks and template** option, if you want to carry all task and template assignments from the original template to the new template. Template task assignments, and the Template Owner and Sponsor are transferred to the copied template. 
1. Click **Save** to create a copy of the template.

   The new template displays in the template list in the Template area of Workfront. 
