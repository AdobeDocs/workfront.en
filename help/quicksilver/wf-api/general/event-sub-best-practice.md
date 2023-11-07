---
content-type: api
navigation-topic: general-api
title: Event subscription best practices
description: Event subscription best practices
author: Becky
feature: Workfront API
role: Developer
exl-id: 2c6e3567-d5eb-4528-a393-dbf235958ed2
---

# Event subscription best practices

Adobe Workfront Event Subscription messages automatically send from Workfront after you have correctly configured your service and created an Event Subscription to trigger those message deliveries. To learn more about properly setting up Event Subscriptions, see [Event Subscription delivery requirements](../../wf-api/general/setup-event-sub-endpoint.md).


Listed below are a few best practices to help you effectively create Event Subscriptions.

## Provide all required request body fields

Make sure that all required request body fields are provided to the API. For information about all required request attributes, please see [Event Subscription API](../../wf-api/general/event-subs-api.md).

## Avoid including extra body fields

Do not include extra body fields in the request, as this will result in the failure of the API to create a subscription.

## Complete testing within the grace period

Try to get all subscription testing done within the 100-message grace period. To learn more about this grace period, see [FAQs - Event Subscriptions](../../wf-api/general/event-subs-faq.md).

## Meet the Standard Event Subscription Message Delivery Requirements

Make sure your subscription endpoint conforms to the Standard Event Subscription Message Delivery Requirements. To learn about these requirements, see [Event Subscription delivery requirements](../../wf-api/general/setup-event-sub-endpoint.md).

## Allowlist IP addresses by global region

In order to receive event subscriptions payloads through your firewall, you must add the IP addresses to the allowlist by global region. To learn more, see [Event Subscription API](../../wf-api/general/event-subs-api.md).

## Have the right access level and an API key

To create, query, or delete an Event Subscription, your Workfront user needs:

* An access level of **System Administrator** 
  To learn more, see [Grant a user full administrative access](../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md) or [Grant users administrative access to certain areas](../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md).

* An API key

  <!--
  <p data-mc-conditions="QuicksilverOrClassic.Draft mode">To learn more, see .</p>
  -->
