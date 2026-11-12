---
content-type: api
navigation-topic: general-api
title: Manage event subscriptions as a non-admin user
description: If your Workfront access allows it, you can create, view, and delete event subscriptions that are within the scope permitted by your permissions and system configuration.
author: Courtney
feature: Workfront API
role: Developer
---

# Manage event subscriptions as a non-admin user

If your Workfront access allows it, you can create, view, and delete event subscriptions from the Setup area. However, your access is limited to the subscriptions and actions that are authorized for your role and by your organization's system configuration.

This feature is not available to every user in the same way as it is to Workfront administrators. Users with the required access can manage event subscriptions only within the scope granted to them.

For example, your permissions may allow you to manage only certain object types, event types, or subscriptions for a defined set of work. You cannot manage event subscriptions outside the scope allowed by your access and configuration.

For administrator-managed setup, see [Configure event subscriptions in Workfront](/help/quicksilver/administration-and-setup/manage-workfront/manage-event-subscriptions/configure-event-subscriptions-in-workfront.md).

For information about the Event Subscriptions API, see [Event Subscription API](/help/quicksilver/wf-api/general/event-subs-api.md).

>[!NOTE]
>
>Users can manage event subscriptions only within the scope allowed by their permissions and the organization's system configuration. Access is not automatically equivalent to administrator access.

## Access requirements

+++ Expand to view access requirements for the functionality in this article.

<table style="table-layout:auto">
 <col>
 <col>
 <tbody>
  <tr>
   <td role="rowheader">Adobe Workfront package</td>
   <td>Any</td>
  </tr>
  <tr>
   <td role="rowheader">Adobe Workfront license</td>
   <td>
    <p>Standard</p>
    <p>Plan</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader">Access level configurations</td>
   <td>
    <p>You must have the appropriate access to manage event subscriptions.</p>
    <p>Your access is limited to the subscriptions and actions allowed by your permissions and your organization's system configuration.</p>
   </td>
  </tr>
 </tbody>
</table>

For information, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Work with event subscriptions

{{step-1-to-setup}}

1. In the left navigation panel, click **System**, then click **Event Subscriptions**.
1. Review the subscriptions available to you.
1. Create, view, or delete only the subscriptions that fall within your authorized scope.

If you do not see the options you expect, or if you are unable to create or manage a subscription, contact your Workfront administrator to confirm whether your access is limited by role, permissions, or system configuration.

## Related articles

* [Configure event subscriptions in Workfront](/help/quicksilver/administration-and-setup/manage-workfront/manage-event-subscriptions/configure-event-subscriptions-in-workfront.md)
* [Event Subscription API](/help/quicksilver/wf-api/general/event-subs-api.md)
