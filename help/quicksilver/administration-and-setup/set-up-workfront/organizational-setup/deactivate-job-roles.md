---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: organization-setup
title: Deactivate Job Roles
description: As an [!DNL Adobe Workfront] administrator or a user with administrative access to Job Roles, you can deactivate job roles that become obsolete in your system. When you deactivate a job role instead of deleting it, you can keep any historical information that is associated with it.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 934cef1a-8157-45db-b000-24a08a94dd18
TQID: https://experienceleague.adobe.com/e8vdktak-XCg5wC1h4mYTMUtOHVOssw7BSFri6rAx5Y
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
    internal-label: Administration
subfeature_v2:
  - id: b04e3dc0-3a59-45b1-aa02-b0b6d5f87eff
    internal-label: Approvals
  - id: d3382524-5489-431b-bde9-271ab257bc37
    internal-label: Workfront Scenario Planner
  - id: d87de1f9-8e24-4c4d-aa4c-a403075091a1
    internal-label: Custom forms
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
    internal-label: Admin
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
    internal-label: Reporting
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
---
# Deactivate job roles

As an [!DNL Adobe Workfront] administrator or a user with administrative access to Job Roles, you can deactivate job roles that become obsolete in your system. When you deactivate a job role instead of deleting it, you can keep any historical information that is associated with it.

You can also reactivate job roles that have previously been deactivated.

## Access requirements

## Access requirements

+++ Expand to view access requirements for the functionality in this article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Adobe Workfront] package</td> 
   <td><p>Any</p></td> 
  </tr> 
  <tr> 
   <td>[!DNL Adobe Workfront] license</td> 
   <td><p>[!UICONTROL Standard]</p>
       <p>[!UICONTROL Plan]</p></td>
  </tr> 
  <tr> 
   <td>Access level configurations</td> 
   <td>Administrative access to Job Roles</td>
  </tr> 
 </tbody> 
</table>

For information, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## The impact of deactivating job roles

If you deactivate a job role, it no longer displays in the following areas:

* The [!UICONTROL Assignments] typeahead field (for tasks, template tasks, issues, approvals, and routing rules)
* The [!UICONTROL Assignments] fields in lists and reports
* User profiles

   >[!NOTE]
   >
   >When you add a new role to a user, a deactivated job role doesn't display. But it does continue to display in the [!UICONTROL Primary Role] and [!UICONTROL Other Roles] fields if the user was associated with the job role before it was deactivated.

* The [!UICONTROL Sharing] dialog box for objects, including layout template assignment
* Typeahead fields in custom forms
* The [!UICONTROL Pool Members] field in [!UICONTROL Resource Pools]
* The [!UICONTROL Job Role] field of a [!UICONTROL Billing Rate] edit screen when a user is overriding billing rates for projects
* The [!UICONTROL Add assignment to Kanban board] dialog box in a project
* The [!UICONTROL Job Role] field of a plan or an initiative when someone is using the [!DNL Adobe Workfront Scenario Planner].

   The [!DNL Scenario Planner] is available only in the new [!DNL Adobe Workfront] experience and requires an additional license. For information about the [!DNL Workfront Scenario Planner], see [The [!DNL Scenario Planner] overview](../../../scenario-planner/scenario-planner-overview.md).

>[!TIP]
>
>Deactivated roles always display in filters in lists, reports, and other tools such as the [!UICONTROL Workload Balancer].

## Considerations before deactivating a job role

It is better to deactivate rather than delete job roles that become obsolete so that you can keep all the historical information associated with roles you may have used in the past.

>[!NOTE]
>
>Any work assigned to the job role prior to deactivation remains assigned.

We recommend that you do the following before deactivating an unused job role:

* Build reports for any objects that are assigned to the role you plan to deactivate and reassign them to an active job role. For information about building reports, see [Create a report](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-report.md).

   >[!TIP]
   >
   >You can create a report to filter for any tasks or issues where the deactivated role is assigned. Then use the report to reassign outstanding tasks or issues to an active role.

* Take an inventory of all approval processes, current approval paths, and routing rules or other objects that are assigned to the job role you plan to deactivate and reassign them to an active role.

   >[!TIP]
   >
   >When using request queues, if you deactivate a job role assigned as the default assignee in a routing rule, the role remains and requests are still routed to the deactivated role. We recommend updating routing rules with active roles before you deactivate the team.

   For information about creating approval processes and routing rules, see the following articles:

   * [Create an approval process for work items](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md)
   * [Create Routing Rules](../../../manage-work/requests/create-and-manage-request-queues/create-routing-rules.md)

## Deactivate a job role

{{step-1-to-setup}}

1. In the left panel, click&#x200B; **[!UICONTROL Job Roles].**
1. (Optional) In the **[!UICONTROL Filter]** drop-down menu, select **[!UICONTROL Active]** to display only active job roles.
1. Click the name of the job role that you want to deactivate.
1. In the **[!UICONTROL Is Active]** drop-down menu, select **[!UICONTROL No]**.

   ![Deactivate job role](assets/deactivate-job-role-edit-role-box-nwe.png)

1. Click **[!UICONTROL Save Changes]**.

   The job role is deactivated and can no longer be assigned to work, associated with layout templates, and so on. For information about all uses of job roles in [!DNL Workfront], see [Job role overview](../../../administration-and-setup/set-up-workfront/organizational-setup/job-role-overview.md).
