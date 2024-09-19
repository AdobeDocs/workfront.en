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
---
# Deactivate or reactivate a custom form

You can reactivate or deactivate a custom form. We recommend deactivating custom forms rather than deleting forms you no longer use to retain historical data.

>[!NOTE]
>
>If a custom form is deactivated but is still part of a queue topic or request queue definition, it will be attached to new requests. If you do not want the form to be on the requests, you must manually remove it from the request queue.

## Access requirements

+++ Expand to view access requirements for the functionality in this article.

You must have the following to perform the steps in this article:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>Adobe Workfront plan</p> </td> 
   <td>Any</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license</td> 
   <td>
   <p>New: Standard</p>
   <p>or</p>
   <p>Current: Plan</p></td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>Administrative access to custom forms</p></td> 
  </tr>  
 </tbody> 
</table>

For more detail about the information in this table, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

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
