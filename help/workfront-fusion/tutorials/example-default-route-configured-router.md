---
filename: example-default-route-configured-router
product: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Example of a Default route configured for a router
description: The below scenario does the following:
---

# Example of a Default route configured for a router

The below scenario does the following:

* Filters email messages from specific senders and send them to a corresponding Slack channel
* Sends emails from all other senders to a specific Slack channel

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">screenshot</p>
-->

screenshot

Set filters for the routes as follows:

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">screenshot</p>
-->

screenshot

By selecting the Default route option when setting up a route filter, all emails that do not meet the filter conditions specified for the other routes, continue on via this route. The emails are filtered in the order the routes were attached to the router. If you are not sure in which order they were attached, click the Auto-align button

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
screenshot
</MadCap:conditionalText>
-->

`<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">  screenshot</MadCap:conditionalText>` in the menu below.

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">screenshot</p>
-->

screenshot
