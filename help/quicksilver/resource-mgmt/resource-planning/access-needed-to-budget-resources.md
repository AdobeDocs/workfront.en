---
content-type: reference
product-area: resource-management
navigation-topic: resource-planning
title: Access needed to budget resources in Workfront
description: You can view and manage information about resource planning for the projects that you have access to view when you have certain access level settings and the permissions for your work items, users, job roles, and teams.
author: Lisa
feature: Resource Management
exl-id: d2bfc411-188a-4f8b-8180-0e984f01b5ab
TQID: https://experienceleague.adobe.com/X0g8M77au0kHvFSt6q-v0TOc9Lh3VxaHtUngvg-uoUk
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
    internal-label: Administration
  - id: e14a7f57-c82c-4874-a495-5d036cbbdc3d
    internal-label: Resource Management
subfeature_v2:
  - id: d1573eb8-a2e8-4a06-9526-9c3410bf4914
    internal-label: Resource Planner
  - id: e147ce9d-7675-49bd-8a32-44f27d865560
    internal-label: Get started
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
topic_v2:
  - id: bce87dde-a4ab-44c9-8a18-ad66e4ddb377
    internal-label: Customer experience
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
---
# Access needed to budget resources in Workfront

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p><b>(LINKED TO PRODUCT</b>: This is also linked to the product, in two different tooltips in the RP:</p>
<p>- the tooltip for the View-only mode of the Budgeted Hours boxes. You gave this link to Vazgen and the team for the tooltip and documented this in this sheet:https://docs.google.com/spreadsheets/d/1zKjNVw_TyfQ474jbY7JorSWTkptMNb5RFCck2IficYs/edit#gid=0</p>
<p>- Also in the tooltip from this issue: https://hub.workfront.com/issue/view?ID=5ca708d00024a39e58b5dbeaceb00939)</p>
<p>This might need to be moved to Resource Management overview and title needs to be changed to "Acces needed to manage resources" when the res manager prerequisite will drop for resource scheduling and the field goes away.</p>
<p>This should be linked from Planning in the Resource Planner - in the Budgeting Resources in the RP area)</p>
</div>
-->

When your company has purchased an Adobe Workfront license that includes Resource Planning you can view resource budgeting information for the projects that you have permissions to view. You can view budgeting information in the Resource Planner. 

For additional information about prerequisites for using the budgeting tools in Workfront, see [Get started with Resource Planning](../../resource-mgmt/resource-planning/get-started-resource-planning.md).

In order to budget resources, manage Resource Pools, and see Cost information in the resource planning tools, your company and you must have the following access:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront package</td> 
   <td><p>Any</p></td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront license</td> 
   <td><p>Standard</p>
       <p>Plan</p></td>
  </tr>  
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> 
    <ul> 
     <li> <p>Edit access to Resource Management in your access level that includes:</p> 
      <ul> 
       <li> <p>Access to edit project priorities and budget hours. </p> </li> 
       <li> <p>Access to manage Resource Pools, if you need to manage Resource Pools.</p> </li> 
      </ul> <p>For information about the Resource Management access level, see the article <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-resource-management.md" class="MCXref xref">Grant access to Resource Management</a>.</p> </li> 
     <li> <p>Edit access to Projects and Users. </p> </li> 
     <li> <p> Edit access to Financial Data in your access level that includes access to View or Edit Cost Rates and View or Edit General Finance, if you need to view or manage information by Cost.</p> <p>For more information about the Financial Data access level, see the article <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md" class="MCXref xref">Grant access to financial data</a>.</p> </li> 
    </ul> 
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions on the project that include Edit Cost Rates and Edit General Finance permissions.</p> <p>For information about project permissions, see the article <a href="../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md" class="MCXref xref">Share a project in Adobe Workfront</a>.</p> <p>For information about financial permissions on a project, see the article <a href="../../workfront-basics/grant-and-request-access-to-objects/share-financial-permissions-object.md"><a href="../../workfront-basics/grant-and-request-access-to-objects/share-financial-permissions-object.md" class="MCXref xref">Share financial permissions on an object</a></a>.</p> 
   
   <p><b>NOTE:</b> When budgeting resources in the Role view, if you have less than Manage permissions for at least one project listed under the role, you cannot budget hours, FTE, or Cost for the role. You can budget only the projects that you have Manage permissions for.</p> </td> 
  </tr> 
 </tbody> 
</table>

For information, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).
