---
title: Auto-complete a request with data from previous requests
content-type: reference
description: You can use AI to auto-complete request fields using data from previous requests.
author: Alina
feature: Get Started with Workfront
exl-id: a0cd1fbf-d3c6-454c-a85a-ceca4b1e8a7b
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/EJR8tFVdc-sYRL5kXf-Ex9WExL0hcbkhQ1ZwEmpmU-s
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
    internal-label: Administration
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
topic_v2:
  - id: bce87dde-a4ab-44c9-8a18-ad66e4ddb377
    internal-label: Customer experience
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
---
# Auto-complete a request with data from previous requests

AI can help you auto-complete request fields based on previous requests. You can approve or reject these suggestions before submitting the request. 

Auto-complete does not overwrite any fields that you have already filled in.

Users do not receive suggestions of data that they do not otherwise have access to.

## Access requirements

+++ Expand to view access requirements for the functionality in this article.

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
   <td> <p>Contributor or higher</p>
   <p>Request or higher</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>Edit access to Issues</p>  </td> 
  </tr> 
   <td role="rowheader">Object permissions</td> 
   <td><p>Access to add requests to a request queue</p> <p>View or higher permissions on the existing request</p> <p>For information on setting up a request queue, see <a href="../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">Create a Request Queue</a>. </p> </td> 
  <tr>
  </tr>
 </tbody> 
</table>

For information, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md). 

+++

## Get suggestions when filling out form 

Auto-complete can suggest field values while you are filling out the form. As you enter values into the request fields, Workfront compares those values with previous requests. If the entered value closely correlates with other field values in similar contexts in previous requests, Workfront suggests those values.

For example, if a clinic always uses the same billing code, Workfront would suggest that billing code in the appropriate field when the clinic name is entered.

To use suggestions based on previous requests:

1. Begin creating a request.

   For instructions, see [Create and submit requests](/help/quicksilver/manage-work/requests/create-requests/create-submit-requests.md).

1. Begin filling in fields.

   As you fill in fields, other fields may show suggestions.

1. For each field suggestion, select **Accept** or **Reject** for that field.

   ![Accept or reject suggestion](assets/accept-reject-suggestion.png)

   Or

   Select **Accept all** or **Reject all** at the top of the page to accept or reject all suggestions. 

   >[!NOTE]
   >
   >Any unreviewed suggestions will be automatically accepted when you submit the request.
