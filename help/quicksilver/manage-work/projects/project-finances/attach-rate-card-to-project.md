---
title: Attach a Rate Card to a Project
description: When you attach a rate card to a project, all of the roles and their associated billing rates are added to the project.
author: Lisa
feature: Work Management
role: User
exl-id: 97c33c5a-e42d-4015-841f-69dc44a0599d
TQID: https://experienceleague.adobe.com/waVWQfq2YqgDXZx3wl0ahzuQx7UJ78S1kYY8xBgi5OQ
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
    internal-label: Work management
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
    internal-label: Administration
subfeature_v2:
  - id: f0dd7b45-76b5-49d4-afe3-39f436b6fbd3
    internal-label: Projects
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
---
# Attach a rate card to a project

Rate cards store multiple billing rates per job role, based on attributes. For example, you could have a job role of Designer based in Paris for Agency A, another Designer based in Paris for Agency B, and a third Designer based in New York not assigned to an agency, each with different billing rates. However, attributes are not required for job roles on a rate card. The attributes serve as tools to establish more granular rates. A billing rate on a rate card can also be date effective, so that the rate starts and ends on specified dates.

When you attach a rate card to a project, all of the roles and their associated billing rates are added to the project.

>[!NOTE]
>
>Attaching a rate card overrides any existing rate card billing rates on the project. Billing rate overrides that were added directly to the project are not removed.

For information about creating rate cards, see [Manage rate cards](/help/quicksilver/administration-and-setup/manage-enterprise-operations/manage-rate-cards.md).

For general information about overriding job role billing rates for projects and calculating project revenue, see [Overview of overriding billing rates and calculating revenue on a project](/help/quicksilver/manage-work/projects/project-finances/override-role-billing-rates-and-calculate-project-revenue.md).

## Access requirements

+++ Expand to view access requirements for the functionality in this article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront package</td> 
   <td>Workflow Ultimate</td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront license</td> 
   <td>Standard</td> 
  </tr> 
  <tr> 
   <td>Access level configurations</td> 
   <td>Edit access to Projects, Financial Data, and Rate Cards</td> 
  </tr> 
  <tr> 
   <td>Object permissions</td> 
   <td>Manage permissions to the project with permissions to Edit Billing Rates</td> 
  </tr> 
 </tbody> 
</table>

For information, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Attach a rate card to a project

1. Go to the project.
1. Click **Rates** in the left panel, then select **Billing**.
1. Click **Add Billing Rate > Attach a Rate Card**.
   
   The **Attach a rate card** box opens. You can search for a rate card in the list.

   ![Attach a rate card box](assets/attach-rate-card-dialog.png)

   >[!NOTE]
   >
   >The Group and Company on the rate cards are used as filters on this list. Because projects also include Group and Company fields, Workfront uses these values to narrow the list of available rate cards to those relevant to the project's context, and not all rate cards across the system.
   >
   >The match does not need to be exact. Rate cards with blank Group and/or Company values may still appear depending on the project's Group/Company configuration. For example, if a project has a Group selected but the Company is blank, you may see rate cards associated with that Group even if the rate card's Company is different or blank.

1. Select the rate card to add to the project, and click **Attach**.

   The rate card and all of its job role rates are added to the billing rates list.

   ![Rate card added to project](assets/rate-card-on-project.png)

## Remove a rate card from a project

When you remove a rate card from a project, all of its job role rates are removed. You cannot remove an individual rate from the project that comes from a rate card.

Billing rate overrides for users or job roles that were added directly to the project can be removed without removing the entire rate card.

1. Go to the project.
1. Click **Rates** in the left panel, then select **Billing**.
1. Click the **Remove** icon ![Remove icon](assets/remove-icon.png).
1. Click **Confirm** on the confirmation message to remove the rate card.

