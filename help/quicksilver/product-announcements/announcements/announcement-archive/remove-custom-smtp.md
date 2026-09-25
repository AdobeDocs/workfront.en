---
content-type: reference
navigation-topic: announcements
title: Remove custom SMTP as an outgoing email option
description: With the 20.3 release (targeted for August 2020), Adobe Workfront is moving to a new email system that will greatly enhance the reliability of your email delivery for Workfront updates and notifications. As a result of this, customers will no longer be able to use their own SMTP email server to relay their email from the Workfront platform to the intended recipient. All email will be sent directly from the Workfront Mail Server.
author: Luke
feature: Product Announcements
exl-id: 73abd185-81c6-43fc-b8b0-cad14d15b348
TQID: 'https://experienceleague.adobe.com/q3IdES8LZlJDDBjUqTkHmWqjtVdMV-w80o7wC-uRSXg'
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
    internal-label: Administration
subfeature_v2:
  - id: a29813d3-f0cc-4b60-9396-13b558370803
    internal-label: Product announcements
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
---
# Remove custom SMTP as an outgoing email option

>[!NOTE]
>
>Functionality described in this article is no longer available, and the article will be removed in the near future.

With the 20.3 release (targeted for August 2020), Adobe Workfront is moving to a new email system that will greatly enhance the reliability of your email delivery for Workfront updates and notifications. As a result of this, customers will no longer be able to use their own SMTP email server to relay their email from the Workfront platform to the intended recipient. All email will be sent directly from the Workfront Mail Server.

This feature is accessed by logging in as a System Administrator and navigating to Setup > Email > Setup. Here is a screenshot highlighting the feature:

![Email server settings](assets/email-server-settings-350x226.png)

The setting highlighted in this screenshot will automatically transition to use the Workfront Mail Server option with the 20.3 release.

If you have configured a custom SMTP mail server, **we highly recommend that you reach out to your IT team** to ensure that email from notifications@my.workfront.com is not going to be blocked for incoming email to your system. You can also reference Configuring your firewall for details about which IP addresses our traffic and email come from.

If you have any other questions or concerns please contact the [Workfront Support Team](https://experienceleague.adobe.com/?support-tab=home#support).
