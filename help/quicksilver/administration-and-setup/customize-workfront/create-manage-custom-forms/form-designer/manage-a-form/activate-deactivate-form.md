---
title: Deactivate or Reactivate a Custom Form
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: You can reactivate or deactivate a custom form. We recommend deactivating custom forms rather than deleting forms you no longer use to retain historical data.
author: Lisa
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: 6d9a409d-8d16-4c58-ad02-f60aa1ac1714
TQID: https://experienceleague.adobe.com/w4GbXu2z8f8kymWMp7mGn5qRm5gf5X0u9WAI2b5Lcdk
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
    internal-label: Administration
subfeature_v2:
  - id: d87de1f9-8e24-4c4d-aa4c-a403075091a1
    internal-label: Custom forms
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
    internal-label: Admin
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
---
# Deactivate or reactivate a custom form

You can reactivate or deactivate a custom form. We recommend deactivating custom forms rather than deleting forms you no longer use to retain historical data.

>[!NOTE]
>
>If a custom form is deactivated but is still part of a queue topic or request queue definition, it will be attached to new requests. If you do not want the form to be on the requests, you must manually remove it from the request queue.

## Access requirements

+++ Expand to view access requirements for the functionality in this article.

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
   <td>Access level configurations</td> 
   <td> <p>Administrative access to custom forms</p> </td> 
  </tr>  
 </tbody> 
</table>

For information, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Deactivate a custom form

You can deactivate custom forms you no longer use without losing their associated historical data. Users can't add an inactive custom form to objects, but they can still view and add data to its fields on objects where it was already attached.

Fields on an inactive custom form are also still available to inline-edit in a View. If a user adds a field from an inactive custom form during an inline edit, the form attaches to the object automatically, even though the custom form is deactivated.

To deactivate a custom form:

{{step-1-to-setup}}

1. In the left panel, choose **Custom Forms**.
1. In the **Forms** area, select the custom form you want to deactivate.
1. In the Is Active column, choose **False** and click out of the column. The form is no longer active.

## Reactivate a custom form

If you reactivate a custom form, it retains the settings it had before and users can interact with it as if it was never deactivated.

{{step-1-to-setup}}

1. In the left panel, choose **Custom Forms**.
1. In the **Forms** area, select the custom form you want to reactivate.
1. In the Is Active column, choose **True** and click out of the column. The form is now active.
