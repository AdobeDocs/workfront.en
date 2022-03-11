---
filename: configure-pop-ms-exchange
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;setup
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: Configure POP in Microsoft Exchange
description: A POP email account in Microsoft Exchange is disabled.
---

# Configure POP in Microsoft Exchange

## Problem

A POP email account in Microsoft Exchange is disabled.

## Solution

Before spending time troubleshooting the problem, ensure the user's POP account is configured properly. If you continue to experience problems after you confirm the POP account is correctly configured, contact Microsoft Support or one of their partners for additional help.

<!--
For instructions on integrating a POP account in Adobe Workfront, see .
-->

## Access requirements

You must have the following to perform the steps in this article:

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>You must be a Workfront administrator. For more information, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Grant a user full administrative access</a>.</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Configure POP in Microsoft Exchange

>[!NOTE]
>
>The following steps may be used as a general guide for configuring POP in Microsoft Exchange for a production Workfront system. The steps may differ significantly depending on the version of Exchange or the code changes made by Microsoft.

<ol> 
 <li value="1">Start and enable the POP3 service on the Exchange 2010 server. <br><note type="note">
    By default, POP3 service is not started.
  </note>
  <ol>
   <li value="1">Start Microsoft's Server Manager.</li>
   <li value="2">Navigate:&nbsp;<span class="bold">Server Manager</span> > <span class="bold">Configuration</span> ><span class="bold">Windows Firewall with Advanced Security</span> > <span class="bold">Services.</span></li>
   <li value="3">Right-click <span class="bold">Microsoft Exchange POP3</span>, then click&nbsp;<span class="bold">Properties</span>.</li>
   <li value="4">(Conditional) To ensure the POP service automatically starts, on the <span class="bold">General</span> tab, set the <span class="bold">Startup</span> type to Automatic<span class="bold">.</span></li>
  </ol></li> 
 <li value="2">Configure POP3 for the server.<br>
  <ol>
   <li value="1">Start the Microsoft Exchange Management console.</li>
   <li value="2">Navigate: Microsoft <span class="bold">Exchange On-Premise</span> > <span class="bold">Server Configuration</span> > <span class="bold">Client Access</span>.</li>
   <li value="3"><p>Choose&nbsp;<span class="bold">POP3.</span></p><p>POP3 is on the list under the POP3 and IMAP4 tabs.<br></p></li>
   <li value="4">On&nbsp;the right side under <span class="bold">Actions,</span> select&nbsp;<span class="bold">POP3</span>, then choose <span class="bold">Properties</span>.</li>
   <li value="5"><p>Click&nbsp;<span class="bold">POP3 Properties</span>, then open the <span class="bold">Binding</span> tab.</p><p>All available IP addresses and port numbers configured for the POP3 server display. The top box shows the Unencrypted and the bottom box shows the IP and ports for SSL/TLS connections.</p></li>
   <li value="6">Click <span class="bold">POP3 Properties</span>, then open the <span class="bold">Authentication</span> tab.</li>
   <li value="7"><p><span class="bold">Select Secure</span> login.</p><p>A TLS connection is required for the client to authenticate to the server.</p></li>
  </ol></li> 
 <li value="3">Enable or allow users to connect to POP.<br>
  <ol>
   <li value="1">Start the Microsoft&nbsp;Exchange&nbsp;Management console.</li>
   <li value="2"><p>Navigate: Microsoft <span class="bold">Exchange On-Premise</span> > <span class="bold">Recipient Configuration</span> > <span class="bold">Mailbox.</span></p><p>A list of mailboxes or users displays.</p></li>
   <li value="3">Highlight the email being used within Workfront.</li>
   <li value="4">On the right side under <span class="bold">Actions</span>, select <span class="bold">Properties</span>, then open the <span class="bold">Mailbox Features</span> tab.</li>
   <li value="5"><p>(Conditional) If POP3 is disabled, click <span class="bold">POP3</span>, then click <span class="bold">Enable</span>.</p><p>A list of mailboxes or users displays.</p></li>
  </ol></li> 
 <li value="4">Configure receive connectors.<br>
  <ol>
   <li value="1">Start Microsoft Exchange&nbsp;Management console.</li>
   <li value="2"><p>Navigate: Microsoft <span class="bold">Exchange On-Premise</span> > <span class="bold">Server Configuration</span> > <span class="bold">Hub Transport.</span></p><p>A list of receive connectors displays.</p></li>
   <li value="3"><p>Confirm the receive connector <em>Client</em> <em>EX01</em> is enabled.</p><p>Where <em>Client</em>&nbsp;<em>EX01</em> is the name of your Exchange server.</p></li>
   <li value="4">Select&nbsp;<em>Client EX01</em>, then on the right under <span class="bold">Actions</span>, select <span class="bold">Properties.</span></li>
   <li value="5"><p>Open the <span class="bold">Authentication</span> tab, then ensure <span class="bold">Transport Layer Security (TLS)</span> is checked.</p><note type="note">
      In order to have Basic Authentication, you may need to start TLS and Integrated Windows Authentication.
    </note></li>
  </ol></li> 
</ol>

