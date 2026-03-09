---
content-type: overview
product-area: projects
navigation-topic: financials
title: Set up a Job Role for Billing
description: Workfront allows you to bill a user under a different job role than their primary job role. This is useful when a person temporarily performs work that should be billed at a different rate.
author: Lisa
feature: Work Management
---
# Set up a Job Role for Billing

{{highlighted-preview-article-level}}

Workfront allows you to bill a user under a different job role than their primary job role. This is useful when a person temporarily performs work that should be billed at a different rate.

You can assign a Job Role for Billing in two ways:

* At the project level: Use this when the person should be billed under the same job role for the entire project.
* At the assignment level: Use this when you want to bill differently on specific tasks.

>[!NOTE]
>
>* A Job Role for Billing applies only to people (users). It does not apply to generic job roles or placeholders.
>* Adding a Job Role for Billing affects the billing rate only, not cost.
>* Assignment-level billing always takes priority over project-level billing.

For more information, see [Overview of revenue and cost hierarchy](/help/quicksilver/manage-work/projects/project-finances/overview-revenue-cost-hierarchy.md) and [Create advanced assignments](/help/quicksilver/manage-work/tasks/assign-tasks/create-advanced-assignments.md).

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
   <td> Edit access to Rate Cards</td> 
  </tr> 
  <tr> 
   <td>Object permissions</td> 
   <td>Manage permissions to the project </td> 
  </tr> 
 </tbody> 
</table>

For information, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Assign a Job Role for Billing at the project level

When you create a job role for billing on a project:

* The billing role applies to all tasks and assignments within the project for that user.
* Billing uses the selected job role's billing rate, but cost still follows the user's primary role.

To assign a job role for billing at the project level:

1. Open a project.
1. Click **Resource for Billing** in the left panel.
1. Select the **Job role for billing** tab if it is not already displayed.
1. Click **Add > Add job role for billing**.
1. On the **Add job role for billing** box, select the **User**.
1. Select the **Job role** to use as the job role for billing for this user on this project.
1. (Optional) Click **Add job role** to define effective dates for the job role for billing. Enter the **Start** and **End** dates for the job role.

   [Add job role for billing at project level](assets/jrfb-project-level.png)

1. Click **Add job role** again to specify additional billing roles for different time periods.
1. Click **Save**.

### Example at the project level

>[!BEGINSHADEBOX]

John's primary job role is Designer 1. The project requires a Senior Designer, and John is filling in.

You would set the Job Role for Billing to **Senior Designer** at the project level.

Result:

* Billing revenue is the Senior Designer rate
* Cost is the Designer 1 cost rate (John's actual cost rate)

>[!ENDSHADEBOX]

## Assign a Job Role for Billing at the assignment level

When you add a job role for billing on an assignment, the setting overrides a project-level billing role for that specific assignment only.

To assign a job role for billing at the assignment level:

1. Open a project and locate the task.
1. Go to the task's **Advanced Assignments**.
   
   For information, see [Create advanced assignments](/help/quicksilver/manage-work/tasks/assign-tasks/create-advanced-assignments.md).

1. On the task assignment grid, locate the column **Job role for billing**.
1. Select a job role for each assignment where you want different billing.

   >[!NOTE]
   >
   >If a job role for billing was assigned at the project level, it appears on the assignment. You can click in the **Job role for billing** field and select another job role to use for the assignment.
   >The information icon notifies you whether a job role for billing was defined at the project or the assignment level.

   ![Job role for billing on an assignment](assets/jrfb-assignment-level.png)

### Example at the assignment level

>[!BEGINSHADEBOX]

John's primary job role is Designer 1. He is billed as a Senior Designer at the project level, but there is one special task requiring a Principal Designer billing rate.

You would set the Job Role for Billing to Principal Designer on that assignment only.

Result:

* All of John's other tasks bill as Senior Designer
* This one task bills as Principal Designer
* Cost remains Designer 1

>[!ENDSHADEBOX]
