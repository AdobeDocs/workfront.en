---
product-area: templates
navigation-topic: templates-navigation-topic
title: Copy a project template
description: Rather than creating a new project template from scratch, you can copy an existing template and make changes to that, if needed.
author: Alina
feature: Work Management
exl-id: b2e0878b-8245-4e01-819d-c3746f553d95
---
# Copy a project template

Rather than creating a new project template from scratch, you can copy an existing template and make changes to that, if needed.

## Access requirements

You must have the following access to perform the steps in this article:

<table style="table-layout:auto"> 
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
   <td> <p>Edit access to Templates</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View or higher permissions to a template</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your Workfront administrator.


## Considerations about copying templates

The following items are always copied from an existing project to a new one:

* Template Tasks
* Template Task Default information (Task Default Approval Process, Task Default Custom Forms)
* Custom forms
* Risks
* Queue Setup information
* Portfolio and Program
* Approvals
* Documents
* The days of the original template tasks transfer to the new template. You must change the Start or Completion day of the template (depending on its Schedule Mode) to update the days on the template tasks, if needed. 

The following items are never copied from an existing project to a new one:   

* Billing Rates
* User comments  

## Copy a template

1. Go to the template that you want to copy.
1. Click the **More** menu ![](assets/qs-more-icon-on-an-object.png), then click **Copy**.
1. Specify a name for the template in the **New Template Name** field.

   By default, the new name is **Copy of `<original template name>`.**

1. Select whether you want to **Retain user assignments on tasks and template**: select this option to carry all task and template assignments from the original template to the new template.
1. Click **Save** to create a copy of the template.
