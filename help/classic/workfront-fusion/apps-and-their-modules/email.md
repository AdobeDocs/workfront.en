---
filename: email
content-type: reference
product: workfront-fusion
product-area: workfront-integrations
navigation-topic: apps-and-their-modules
title: Email
description: This isn't a list of modules. It's just about connecting email to fusion. Does it need to be in a different section from all the other apps?
hidefromtoc: true
---

# Email

<!--
<p style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">This isn't a list of modules. It's just about connecting email to fusion. Does it need to be in a different section from all the other apps?</p>
-->

Adobe Workfront Fusion requires an Adobe Workfront Fusion license in addition to an Adobe Workfront license.
In a Adobe Workfront Fusion scenario, you can connect your [Fusion app] account to multiple third-party applications and services.This allows you to download emails via IMAP, send emails via SMTP, create new drafts, move and copy emails from one folder to another folder, mark emails as read or unread, and delete emails.

## Connect your email to Workfront Fusion

* [IMAP connection settings](#imap-connection-settings) 
* [SMTP connection settings](#smtp-connection-settings)

### IMAP connection settings {#imap-connection-settings}

IMAP connection allows you to access your mailbox remotely and read or manipulate messages in your mailbox. IMAP connection is used by most of the Email modules. For instructions about connecting your IMAP account to Workfront Fusion, see [Create a connection to Workfront Fusion - Basic instructions](../../workfront-fusion/connections/connect-to-fusion-general.md) Before you click **Continue**, select whether you want an IMAP or Google connection. These are both IMAP connections, but Gmail requires a different type of authorization.

Screenshot

* [Connect to email](#connect-to-email) 
* [Connect to other mailboxes via IMAP](#connect-to-other-mailboxes-via-imap)

#### Connect to email {#connect-to-email}

For instructions about connecting your email account to Workfront Fusion, see [Create a connection to Workfront Fusion - Basic instructions](../../workfront-fusion/connections/connect-to-fusion-general.md)

#### Connect to other mailboxes via IMAP {#connect-to-other-mailboxes-via-imap}

For instructions about connecting your email account to Workfront Fusion, see [Create a connection to Workfront Fusion - Basic instructions](../../workfront-fusion/connections/connect-to-fusion-general.md)

When choosing a type of connection, select the IMAP option. In the next step, you need to set all the parameters necessary for connecting to your mailbox. The easiest way is to locate your email service provider in the displayed list and select it. When you do this, Workfront Fusion will only require you to provide your mailbox password and username. If your provider is not on the list, select the Other option and specify your host, port, and connection security type. To find this information, check the Help section for your mailbox. If you don’t have this information available, contact your email service provider.

### SMTP connection settings {#smtp-connection-settings}

A SMTP connection allows Workfront Fusion to send emails. For instructions about connecting your email account to Workfront Fusion, see [Create a connection to Workfront Fusion - Basic instructions](../../workfront-fusion/connections/connect-to-fusion-general.md) Before you click the Continue button, select the type of connection you want to establish (SMTP or Google). These are both SMTP connections. However, Google Gmail requires a different type of authorization.

Screenshot

* [Connect to Gmail](#connect-to-gmail) 
* [Connect to other mailboxes via SMTP](#connect-to-other-mailboxes-via-smtp)

#### Connect to Gmail {#connect-to-gmail}

You can create scenarios with email modules that require IMAP connection to your Gmail.

For instructions about connecting your email account to Workfront Fusion, see [Create a connection to Workfront Fusion - Basic instructions](../../workfront-fusion/connections/connect-to-fusion-general.md)

When choosing a type of connection, select the Google option.

#### Connect to other mailboxes via SMTP {#connect-to-other-mailboxes-via-smtp}

you can create scenarios with email modules that require IMAP connection to your Gmail.When choosing a type of connection, select the SMTP option. In the next step, you need to set all the parameters necessary for connecting to your mailbox. The easiest way is to locate your email service provider in the displayed list and select it. When you do this, Workfront Fusion will only require you to provide your mailbox username and password. If your provider is not on the list, select the Other option and specify your host, port, and connection security type. To find this information, check the Help section for your mailbox. If you don’t have this information available, contact your email service provider.

## Unique email ID in IMAP protocol

The Unique Email ID known as 'Email ID (UID)' is the email's identifier. The Email ID is specific for each of the email's folders. Hint: For getting and deleting the same email from the same folder, you can see below:

* Getting an email from 'Inbox' folder

  <!--
  <p style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">screenshot</p>
  -->

* Deleting the email from 'Inbox' folder

  <!--
  <p style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">screenshot</p>
  -->

## Change displayed name of sender

1. Open the Send an email action advanced settings using the **Show advanced settings** checkbox. 
1. Enter the required sender name or email.

   >[!IMPORTANT]
   >
   >Use the correct syntax as shown in the hint on the screenshot below.    >
   >
   >```   >
   >name@email.com
   >```   >
   >
   >or    >
   >
   >```   >
   >"Name" name@email.com
   >```   >
   >

   2019-01-10_16_29_32-Microsoft_Edge.png

