---
content-type: api;faq
navigation-topic: general-api
title: FAQs - Event Subscriptions
description: FAQs - Event Subscriptions
author: Becky
feature: Workfront API
role: Developer
exl-id: a6120939-5d76-4f46-a304-125de6b22502
---
# FAQs - Event Subscriptions

<!--
{{highlighted-preview}}
-->

The following are frequently asked questions about Event Subscriptions:

## What is a subscription?

A subscription is a set of data used to match and deliver Adobe Workfront events to a customer's HTTP endpoint. This resource is made up of 4 primary attributes:

* customer_id
* obj_code
* obj_id
* url

A subscription can also have other attributes—such as its own unique ID and the date it was created—but the attributes listed above are primarily used to match events and deliver them to customers.

## Am I able to select which events are sent to an endpoint based on certain criteria within an event payload?

Event subscription filters are a way that event subs can be sorted by specified criteria. It is recommended that you apply filters to event subscriptions as it may significantly reduce the number of messages that an endpoint needs to consume. For more information see [Event subscription filtering](../../wf-api/general/event-subs-api.md#event).

## Why is the API returning a 409 conflict response code?

If you attempt to create an event subscription and receive a response code: 409 conflict, then the subscription you attempted to create is a duplicate. Workfront does not allow the creation of duplicate subscriptions.

## What should I do if my messages aren't being delivered to my endpoint?

Look for the following scenarios and use the recommended solution:

* Ensure that your subscription endpoint—defined by the **url** field—is returning a 2XX HTTP response code. If it is not, contact Workfront Support or see [Event Subscription delivery requirements](../../wf-api/general/setup-event-sub-endpoint.md).

* The event delivery request could be timing out before it completes. Ensure that your endpoint consistently responds within 5 seconds. This is the default timeout set for the HTTP request to deliver an Event Subscription message. If your endpoint is not responding within 5 seconds, contact Workfront Support or see [Event Subscription delivery requirements](../../wf-api/general/setup-event-sub-endpoint.md).
* The events might not generate the way you think. Ensure that you're not making assumptions about how or when events should and do fire. For example, you might think that updating a document on a task generates a task update event, but instead, it generates a document create or document update event.
* Your subscription might not be configured as you expect. You can create event subscriptions in different environments and expect them to transfer as their other Workfront data does. However, Event Subscription data is not configured to be copied or promoted to other environments. Ensure that you're issuing API requests to the correct environment and that the subscriptions in that environment are configured as expected.
* The payload was not received because the necessary Workfront IP address hasn't been added to the allowlist on your firewall. Event Subscription events are sent from only a few IP addresses. Ensure that the destination network has all IP exceptions necessary to receive payloads from Workfront Event Subscriptions.

## Why is it taking an excessive amount of time for my messages to reach my endpoint?

Some of the following scenarios might be responsible:

* A large operation—such as a bulk update—in the system can cause a large volume of messages to be enqueued all at once, which can take some time to process.
* Long-running calculations or timeline calculations on large projects could be causing a delay in the publication of messages to Event Subscriptions to consume.
* The subscription might have been disabled.

   * After a 100-message grace period, if a particular URL—which could be associated with one or more subscriptions—fails more than 70% of the time or if the URL&nbsp;fails to deliver after 2000 consecutive attempts, all messages matching subscriptions with that same URL are not attempted for delivery. Instead, those messages are immediately queued for a retry.

     Every 10 minutes after a URL is disabled, we attempt to deliver the next message that comes through for processing. If that message succeeds, then we re-enable that URL and subsequently any matching subscriptions. If that message fails to send, then that 10-minute timer resets and we try again after it expires.

     This behavior can be perceived as inconsistent or delayed deliveries, but it simply follows our policies for how Event Subscription messages are handled.
   
   * An Event Subscription URL&nbsp;will be hard disabled if either of the following conditions are met:

      * The Subscription URL has failed to deliver for 7 days and has failed at least 2000 consecutive delivery attempts in the last 72 hours.
      * The Subscription URL failed to deliver 50,000 consecutive attempts.

## What should I&nbsp;do if I'm receiving a 500 response status when I attempt to call the Event Subscription API?

Please contact Workfront Support. To learn how to contact support, see [Contact Customer Support](../../workfront-basics/tips-tricks-and-troubleshooting/contact-customer-support.md).

## What different types of authentication can I use with Workfront Event Subscriptions?

You can use any authentication that uses a bearer token. The **authToken** field of a subscription is a string that represents an OAuth2 bearer token used to authenticate with the URL specified in the **url** field. In theory, this token value could be anything as long as the destination endpoint is aware of how to handle its encoding, which is **utf-8**.

## How long should it be before I receive my event payload from Workfront Event Subscriptions?

In general, you can expect to receive Event Subscription event delivery requests in less than 5 seconds from the data change being logged. On average, webhook notifications are received in less than 1 second from the time the data change is made. However, the service can receive messages in such large quantities that it might also take longer.

## Additional resources

* **API Documentation**: [Event Subscription API](../../wf-api/general/event-subs-api.md)

* **Best practices**: [Event subscription best practices](../../wf-api/general/event-sub-best-practice.md)

* **Fields that trigger Event Subscription payloads**: [Event subscription resource fields](../../wf-api/api/event-sub-resource-fields.md)

* **Understanding Event Subscription retries**: [Event subscription retries](../../wf-api/api/event-sub-retries.md)

* **Configuring your firewall for Workfront**: [Configure your firewall's allowlist](../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md)
