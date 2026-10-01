---
title: Add an Approval to a Request Form in Adobe Workfront Planning
description: You can add an approval process to an Adobe Workfront Planning request form, to initiate an approval for every submitted request, before it creates a record.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 058148db-1795-4d39-be87-271008ae3d47
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: 'https://experienceleague.adobe.com/E9LEGJ8T822JuvIO3s8nn6UkLbX-j4ffwaKSviKxl0o'
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
    internal-label: Administration
  - id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
    internal-label: Work management
subfeature_v2:
  - id: b04e3dc0-3a59-45b1-aa02-b0b6d5f87eff
    internal-label: Approvals
  - id: e147ce9d-7675-49bd-8a32-44f27d865560
    internal-label: Get started
  - id: eb361af2-3e4f-4a79-b5f3-7a344ac5794c
    internal-label: Workfront Planning
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
    internal-label: Admin
topic_v2:
  - id: a004cc84-67b9-4a33-a3a7-8ec7273ef4dc
    internal-label: Metadata
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
---
# Add an approval to a request form in Adobe Workfront Planning

<!--update the metadata with real information when making this available in TOC and in the left nav-->


<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the release to Preview, the same features are also available monthly in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>


{{planning-important-intro}}

You can add an approval process to an Adobe Workfront Planning request form, to initiate an approval for every submitted request, before it creates a record.

<!--<span class="preview">Multiple stages are supported in the approval process. When all required decisions in a stage are made, the next stage begins and the new stage's approvers receive an email notification.</span>-->

This article describes how a workspace manager can add an approval to a request form associated with a record type. 

For information about creating a request form in Workfront Planning, see [Create and manage a request form in Adobe Workfront Planning](/help/quicksilver/planning/requests/create-request-form.md).

For information about submitting a request to a record type to create a record, see [Submit Adobe Workfront Planning requests to create records](/help/quicksilver/planning/requests/submit-requests.md). 

## Access requirements

+++ Expand to view access requirements for the functionality in this article. 

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront package</p></td> 
   <td> 
<ul> 
<li><p>Any Workfront or Workflow with a Planning package</p></li>
Or
<li><p>Any Planning package when purchased as a standalone product</p></li></ul>
   </td> </tr>
  <tr> 
   <td role="rowheader"><p>Adobe Workfront license</p></td> 
   <td><p>Workflow Standard</p>
   </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Adobe Planning license</p></td> 
   <td><p>Planning Standard</p>
   </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Access level configuration</p></td> 
   <td> <p>You must add both a Workflow and a Planning license type to the access level when you have both a Workflow and a Planning package</p>   
</td> 
  </tr>  
  <tr> 
   <td role="rowheader"><p>Object permissions</p></td> 
   <td>   <p>Manage permissions to a workspace and  record type</a> </p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p>  </td> 
  </tr>  
</tbody> 
</table> 

For more information about Workfront access requirements, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Considerations about adding approvals to a request form

* You can add one or multiple approvers (users or teams) to a request form or to an approval rule.
* Approval rules route requests based on field values in the submitted request (e.g., different approvers for different values of a "Campaign type" field).
* You can display approval info on the created record via the Approved by and Approved date fields. See Create fields.
* If all approvers approve, a record is created for the record type associated with the request form.
* If at least one approver rejects, no record is created for the record type; the request instead remains/lands in the Requests area of Workfront. (This point appeared in both sections with slightly different wording — merged here as one statement.)
* When multiple approvers are required, all of them must make a decision before the request is approved or rejected — unless the Only one decision is required option is enabled.
* If a team is set as an approver, only one decision is needed from one member of that team.
* Approvals are optional — if a request form has no approval attached, Workfront Planning creates the record immediately on submission.
* <span class="preview">You can add one or more stages to approvals.</span>

## Add approval rules to a request form 

Approval rules define the approval process based on field values in the submitted requests. 

For example, if a request form has the field "Campaign type," a rule can be created that sends the request to one person when the field has the value "Digital", and a different person when it has the value "Print."

To set approval rules for a request form:

1. Start creating a request form for a record type, as described in the article [Create and manage a request form in Adobe Workfront Planning](/help/quicksilver/planning/requests/create-request-form.md).
1. When the request form opens, click **Settings**.

   The **Settings** tab opens.
   
1. To begin configuring approval rules, click **Approvals** ![Approvals icon](assets/approvals-icon-on-form.png) in the left panel.

1. (Optional) If you want to set a default approval process, add at least one user or team to the **Approvers** field of the **Default approval rule** area, then click the **Only one decision is required** checkbox if you want the record to be created after any one of the default approvers has approved it.  

   ![Default approval rule area](assets/default-approvers.png)

1. (Optional) Start adding approval rules. For each custom approval rule, do the following:

   1. Click **Add approval rule**.
   1. Click the placeholder title **Untitled approval rule** and enter a name for the approval rule.
   1. Click **Select a field** and select the field that activates the rule.
   1. Select the operator for the rule. Operators vary based on the type of field.
   1. If the selected operator requires a value, click the plus icon and add one or more values.
   1. (Optional) Click **Add condition** to add more conditions and connect them by **And** or **Or** statements by configuring the additional conditions as in steps C-E.
   1. In the **Actions** area of the approval rule, in the **Approvers** field, add at least one user or team to be set as the approver when the condition is met.
   1. (Conditional and optional) If you want the record to be created after any one of the approvers has approved it, check the **Only one decision is required** checkbox. Otherwise, all approvers must decide on the approval before the request is accepted or rejected.

   >[!NOTE]
   >
   >   Consider the following when adding approval rules:
   >
   >   * If only a default rule is set up, it applies to every submitted request.
   >   * If a custom rule is met, the default is not applied to the request approval workflow. Only the matched custom rules apply for approvals and the default rule is ignored.
   >   * If multiple custom rules are met, the first one in the order applies. In this case, the default approval does not apply, if there is one.

1. <span class="preview">(Optional) Click **Add stage** to add another stage to the approval.</span>

1. Click **Save** to save the approval rules.

1. <span class="preview">(Optional) To add more stages to the approval, do the following:</span>

   1. <span class="preview">Click **Add stage**.</span>
   
      <span class="preview">The **Multi-stage approval** box appears. If you already created a default approval action, those approvers are automatically added to Stage 1.</span>

   1. <span class="preview">In the **Add people or teams** field, add at least one user or team to be set as the approver for the stage.</span>
   1. <span class="preview">(Conditional and optional) If you want the record to advance to the next stage after any one of the approvers has approved it, check the **Only one decision is required** checkbox. Otherwise, all approvers must decide on the approval before the request moves to the next stage.</span>
   1. <span class="preview">Click **Add stage** and repeat from step B to add more stages to the approval.</span>

      <span class="preview">When two or more stages exist, you can click the **Drag** icon ![Drag icon](assets/drag-icon.png) to drag and drop them in order.</span>

      <span class="preview">Click **Delete this stage** to delete a stage from the approval, or click the **Delete** icon ![Delete icon](assets/delete.png) next to an approver to delete the user or team from the list of approvers in a stage.</span>

      ![Multi-stage approval box](assets/planning-request-multi-stage-approval-box.png)

   1. <span class="preview">When you are finished building the approval workflow, click **Save**.</span>

      <span class="preview">You can edit or delete the multi-stage approval from the Approvals page.</span>

1. (Optional) Click **Publish** if you have never shared the request form before.



<!--

## Add an approval to a request form in the Production environment

1. Start creating a request form for a record type, as described in [Create and manage a request form in Adobe Workfront Planning](/help/quicksilver/planning/requests/create-request-form.md).
1. Click **Configuration**.

    The **Configuration** area displays.

    ![Configuration tab](assets/configuration-tab.png)
1. In the **Approvers** field, start typing the name of a user or team that you want to set as an approver, then select it when it displays in the list. 
1. (Optional and conditional) If you have set more than one approver, and only need one approver to make a decision, enable the **Only one decision is required** option.

    (****most of the Note below is duplicated in the Create a request form article***)

      >[!NOTE]
      >
      >
      >* You can add one or several approvers to a request form.
      >
      >* If you add more than one approver, and the Only one decision is required option is not enabled, all approvers must approve the request before Workfront Planning creates a record.
      >
      >* If at least one approver rejects the request, the request is rejected and the record is not created. The request remains in the Requests area of Workfront.
      >
      >* If you add more than one approver, and the Only one decision is required option is not enabled, all approvers must make a decision before a request is either approved or rejected.
      >
      >* If a team is set as an approver, only one decision is required from the team.


1. (Optional) Click **Publish** if you have never shared the request form before.

    Or

    Click **Share** to share the form, then **Copy link**. 
1. (Optional) After a user uses the link you share and submits a request, Workfront Planning sends an approval in-app notification and an email to the approvers.

   For information about approving requests, see [Approve a request](/help/quicksilver/planning/requests/approve-request.md).

-->