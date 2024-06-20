---
content-type: api
navigation-topic: general-api
title: Event Subscription delivery requirements
description: Event Subscription delivery requirements
author: Becky
feature: Workfront API
role: Developer
exl-id: 1b621b35-6c8b-4f6a-bcba-ed6cbfe83a8c
---

# Event Subscription delivery requirements

Event subscription messages are notifications that can be setup to notify users when certain events occur. To learn more about what Event Subscriptions are see [FAQs - Event Subscriptions](../../wf-api/general/event-subs-faq.md).

## Standards for Event Subscription message delivery

Service endpoints that consume Adobe Workfront event subscription messages must meet the following basic requirements, in order to ensure that messages will be sent and received correctly:

* The service endpoint must accept HTTP POST requests. HTTP POST is the request method used in all deliveries of event subscription messages, including validation messages.
 
* In order for the event subscription delivery system to acknowledge the message was successfully received, the endpoint must return a 200-level HTTP status (for example, 200 OK or 202) for all incoming messages.

* If a 200-level status is not returned, the event subscription system assumes the message was not delivered successfully and begins applying the appropriate retry policy. To learn more about the Workfront retry policy, see [Event subscription retries](../../wf-api/api/event-sub-retries.md).

* In conjunction with returning a 200-level status as the response status, the HTTP response must be received within five seconds after the delivery attempt started.This constraint ensures that consumer business processes or infrastructure limitations do not delay the delivery of other messages pending delivery.

* If a long-running business process triggers from an event&nbsp;subscription message, Workfront recommends&nbsp; that

   1. the endpoint saves the message information upon receipt and immediately responds with a 200-level status. 
   1. After an endpoint has responded to an event subscription delivery request, the saved messages can be processed.
