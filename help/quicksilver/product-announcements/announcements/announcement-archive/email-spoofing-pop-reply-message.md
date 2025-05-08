---
content-type: reference
navigation-topic: announcements
title: Email spoofing and POP reply removal
description: We are making two changes to the way Adobe Workfront sends and receives email with the 20.3 release (targeted August 2020).
author: Luke
feature: Product Announcements
exl-id: 9110f04d-b7a9-428b-928c-c4eb746fec3f
---
# Email Spoofing & POP Reply

We are making two changes to the way Adobe Workfront sends and receives email with the 20.3 release (targeted August 2020).

## Outbound Email from Workfront

In an effort to increase successful delivery of emails, we will be eliminating spoofing of emails, which is often tagged as spam (see Email spoofing). All email from Workfront will be sent from `notifications@my.workfront.com`, including both automated alerts and user to user communication. An example email from Joan Harris will look like this in the from area of your email:

![Example email](assets/noreply.png)

*We highly recommend that you reach out to your IT team* to ensure that email from `notifications@my.workfront.com` is not going to be blocked for incoming email to your system. You can also reference [Configure your firewall's allowlist](../../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md) for details about which IP addresses our traffic and email come from.

## Inbound Email Replies to Notifications (POP Reply)

Certain email notifications allow users to reply via email and have the reply be copied into Workfront as a comment reply in the Workfront system. System Administrators in Workfront have traditionally been able to choose between supplying their own POP email server for receiving those replies or to use the built-in Workfront reply system. The custom POP email server choice is being removed with the 20.3 release. All accounts configured to use a custom server will automatically be transitioned to use the native Workfront email reply system. There is no action required for System Administrators or other Workfront users.

There will be no change to emails coming directly from the Workfront Proof system. You will continue to receive those emails as you have in the past.

If you have any other questions or concerns, please contact the [Workfront Support Team](https://experienceleague.adobe.com/?support-tab=home#support).
