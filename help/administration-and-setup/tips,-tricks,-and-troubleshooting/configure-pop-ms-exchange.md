---
filename: configure-pop-ms-exchange
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;setup
navigation-topic: tips-tricks-troubleshooting-setup-admin
---




# Configure POP in Microsoft Exchange {#configure-pop-in-microsoft-exchange}



## Problem {#problem}

A POP email account in Microsoft Exchange is disabled.


## Solution {#solution}

Before spending time troubleshooting the problem, ensure the user's POP account is configured properly. If you continue to experience problems after you confirm the POP account is correctly configured, contact Microsoft Support or one of their partners for additional help.


For instructions on integrating a POP account in `Workfront`, see [Allow users to reply to email notifications](allow-users-reply-to-email-notifications.md).


>[!NOTE]
>
>The following steps may be used as a general guide for configuring POP in Microsoft Exchange for a production `Workfront` system. The steps may differ significantly depending on the version of Exchange or the code changes made by Microsoft.





1. Start and enable the POP3 service on the Exchange 2010 server.   


   >[!NOTE]
   >
   >By default, POP3 service is not started.



    
    
    1. Start Microsoft's Server Manager.
    1. Navigate:&nbsp;**Server Manager** > **Configuration** >**Windows Firewall with Advanced Security** > **Services.**
    
    1. Right-click **Microsoft Exchange POP3**, then click&nbsp;**Properties**.
    
    1. (Conditional) To ensure the POP service automatically starts, on the **General** tab, set the **Startup** type to Automatic**.**
    
    
    

1. Configure POP3 for the server.  

    
    
    1. Start the Microsoft Exchange Management console.
    1. Navigate: Microsoft **Exchange On-Premise** > **Server Configuration** > **Client Access**.
    
    1. Choose&nbsp;**POP3.**
    
    
       POP3 is on the list under the POP3 and IMAP4 tabs.  

    
    1. On&nbsp;the right side under **Actions, **select&nbsp;**POP3**, then choose **Properties**.
    
    1. Click&nbsp;**POP3 Properties, **then open the**&nbsp;****Binding **tab.
    
    
       All available IP addresses and port numbers configured for the POP3 server display. The top box shows the Unencrypted and the bottom box shows the IP and ports for SSL/TLS connections.
    
    1. Click **POP3 Properties**, then open the **Authentication** tab.
    
    1. **Select Secure** login.
    
    
       A TLS connection is required for the client to authenticate to the server.
    
    
    

1. Enable or allow users to connect to POP.  

    
    
    1. Start the Microsoft&nbsp;Exchange&nbsp;Management console.
    1. Navigate: Microsoft **Exchange On-Premise** > **Recipient Configuration** > **Mailbox.**
    
    
       A list of mailboxes or users displays.
    
    1. Highlight the email being used within `Workfront`.
    1. On the right side under **Actions**, select **Properties**, then open the **Mailbox Features** tab.
    
    1. (Conditional) If POP3 is disabled, click **POP3**, then click **Enable**.
    
    
       A list of mailboxes or users displays.
    
    
    

1. Configure receive connectors.  

    
    
    1. Start Microsoft Exchange&nbsp;Management console.
    1. Navigate: Microsoft **Exchange On-Premise** > **Server Configuration** > **Hub Transport.**
    
    
       A list of receive connectors displays.
    
    1. Confirm the receive connector *Client* *EX01* is enabled.
    
    
       Where *Client*&nbsp;*EX01* is the name of your Exchange server.
    
    1. Select&nbsp;*Client EX01*, then on the right under **Actions**, select **Properties.**
    
    1. Open the **Authentication** tab, then ensure **Transport Layer Security (TLS)** is checked.
    
    
       >[!NOTE]
       >
       >In order to have Basic Authentication, you may need to start TLS and Integrated Windows Authentication.
    
    
    
    
    



