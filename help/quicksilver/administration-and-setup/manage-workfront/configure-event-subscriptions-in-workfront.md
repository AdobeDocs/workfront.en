---
user-type: administrator
content-type: how-to
product-area: system-administration
navigation-topic: manage-workfront
title: Configure event subscriptions in Workfront
description: As an Adobe Workfront administrator, you can create, view, and delete event subscriptions from the Setup area to send Workfront events to an external endpoint.
feature: System Setup and Administration
role: Admin
author: Courtney
---

# Configure event subscriptions in Workfront

{{highlighted-preview-article-level}}

As an Adobe Workfront administrator, you can create, view, and delete event subscriptions from the Setup area. Event subscriptions send Workfront event information to an external endpoint when specified events occur.

You can create and delete event subscriptions in Workfront, but you cannot edit an existing subscription. If you need to change a subscription, delete it and create a new one.

For more information about event subscriptions, see the articles under [Event Subscriptions](/help/quicksilver/wf-api/api/event-subscriptions.md).

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
   <td>You must be a Workfront administrator.</td>
  </tr>
 </tbody>
</table>

For information, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Create an event subscription

{{step-1-to-setup}}

1. In the left navigation panel, click **System**, then click **Event Subscriptions**.
1. Click **New event subscription**.
1. In the **Object** field, select the Workfront object that you want to monitor.
1. In the **Event type** field, select whether you want the event subscription to trigger when the object is created, updated, deleted, or shared..
1. In the **Webhook URL** field, enter the endpoint that should receive the event payload.
1. In the **Authentication token** field, enter the token used to authenticate the request to your endpoint.
1. If you want Workfront to encode the payload before sending it, enable the option to send the payload as Base64.
1. If needed, add one or more filters to limit which events trigger the subscription. Available filters are based on the selected object.
1. Click **Create**.

For information about endpoint requirements, see [Event Subscription delivery requirements](/help/quicksilver/wf-api/general/setup-event-sub-endpoint.md).

## View event subscriptions

{{step-1-to-setup}}

1. In the left navigation panel, click **System**, then click **Event Subscriptions**.

From the Event Subscriptions page, you can review the subscriptions configured for your environment. You can also see how many total subscriptions your organization has, and how many of those are active, disabled or frozen. 

* **Disabled subscriptions**: These subscriptions have been automatically disabled due to repeated delivery failures.
* **Frozen subscriptions**: These subscriptions are temporarily frozen due to delivery issues.

## Delete an event subscription

{{step-1-to-setup}}

1. In the left navigation panel, click **System**, then click **Event Subscriptions**.
1. Select the event subscription that you want to remove.
1. Click **Delete**.
