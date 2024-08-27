---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;setup
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: Configure POP in Microsoft Exchange
description: A POP email account in [!DNL Microsoft Exchange] is disabled.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 4f7b6f40-cfbd-4f02-8c3e-de26b05db13b
---
# Configure POP in [!DNL Microsoft Exchange]

## Problem

A POP email account in [!DNL Microsoft Exchange] is disabled.

## Solution

Before spending time troubleshooting the problem, ensure the user's POP account is configured properly. If you continue to experience problems after you confirm the POP account is correctly configured, contact [!DNL Microsoft] Support or one of their partners for additional help.

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">For instructions on integrating a POP account in Adobe Workfront, see .</p>
-->

## Access requirements

+++ Expand to view access requirements for the functionality in this article.

You must have the following access to perform the steps in this article:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan</td> 
   <td>Any</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] license</td> 
   <td>
   <p>New: Standard</p>
   <p>or</p>
   <p>Current: Plan</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td>You must be a [!DNL Workfront] administrator. </td> 
  </tr> 
 </tbody> 
</table>

For more detail about the information in this table, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Configure POP in [!DNL Microsoft Exchange]

>[!NOTE]
>
>The following steps may be used as a general guide for configuring POP in [!DNL Microsoft Exchange] for a production [!DNL Workfront] system. The steps may differ significantly depending on the version of Exchange or the code changes made by Microsoft.

1. Start and enable the POP3 service on the Exchange 2010 server.

   >[!NOTE]
   >
   >By default, POP3 service is not started.

   1. Start [!DNL Microsoft]'s Server Manager.
   1. Navigate: **[!UICONTROL Server Manager]** > **[!UICONTROL Configuration]** >**[!UICONTROL Windows Firewall with Advanced Security]** > **[!UICONTROL Services]**.

   1. Right-click **[!DNL Microsoft Exchange] POP3**, then click **[!UICONTROL Properties]**.

   1. (Conditional) To ensure the POP service automatically starts, on the **[!UICONTROL General]** tab, set the **[!UICONTROL Startup]** type to [!UICONTROL Automatic].

1. Configure POP3 for the server.

   1. Start the [!DNL Microsoft Exchange] Management console.
   1. Navigate: [!DNL Microsoft] **[!UICONTROL Exchange On-Premise]** > **[!UICONTROL Server Configuration]** > **[!UICONTROL Client Access]**.

   1. Choose **[!UICONTROL POP3]**.

      POP3 is on the list under the [!UICONTROL POP3] and [!UICONTROL IMAP4] tabs.

   1. On the right side under **[!UICONTROL Actions]**, select **[!UICONTROL POP3]**, then choose **[!UICONTROL Properties]**.

   1. Click **[!UICONTROL POP3 Properties]**, then open the **[!UICONTROL Binding]** tab.

      All available IP addresses and port numbers configured for the POP3 server display. The top box shows the Unencrypted and the bottom box shows the IP and ports for SSL/TLS connections.

   1. Click **[!UICONTROL POP3 Properties]**, then open the **[!UICONTROL Authentication]** tab.

   1. **[!UICONTROL Select Secure]** login.

      A TLS connection is required for the client to authenticate to the server.

1. Enable or allow users to connect to POP.

   1. Start the [!DNL Microsoft Exchange] Management console.
   1. Navigate: [!DNL Microsoft] **[!UICONTROL Exchange On-Premise]** > **[!UICONTROL Recipient Configuration]** > **[!UICONTROL Mailbox]**.

      A list of mailboxes or users displays.

   1. Highlight the email being used within [!DNL Workfront].
   1. On the right side under **[!UICONTROL Actions]**, select **[!UICONTROL Properties]**, then open the **[!UICONTROL Mailbox Features]** tab.

   1. (Conditional) If POP3 is disabled, click **[!UICONTROL POP3]**, then click **[!UICONTROL Enable]**.

      A list of mailboxes or users displays.

1. Configure receive connectors.

   1. Start [!DNL Microsoft Exchange] Management console.
   1. Navigate: [!DNL Microsoft] **[!UICONTROL Exchange On-Premise]** > **[!UICONTROL Server Configuration]** > **[!UICONTROL Hub Transport]**.

      A list of receive connectors displays.

   1. Confirm the receive connector *Client* *EX01* is enabled.

      Where *Client* *EX01* is the name of your Exchange server.

   1. Select *Client EX01*, then on the right under **[!UICONTROL Actions]**, select **[!UICONTROL Properties]**.

   1. Open the **[!UICONTROL Authentication]** tab, then ensure **[!UICONTROL Transport Layer Security (TLS)]** is checked.

      >[!NOTE]
      >
      >In order to have Basic Authentication, you may need to start TLS and Integrated Windows Authentication.
