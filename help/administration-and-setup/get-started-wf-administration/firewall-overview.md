---
filename: firewall-overview
user-type: administrator
content-type: overview
product-area: system-administration;user-management
navigation-topic: start-with-workfront-administration
title: Firewall overview
description: Because Adobe Workfront communicates with your organization's network, your organization's firewall must be configured to allow that communication. Firewalls are highly effective security measures that function by separating an organization's network from the internet. They ensure that only selected data and network traffic can move into or out of the organization's network. The firewall allows or blocks data based on the site that is sending or receiving the data. As an Adobe Workfront administrator, you must ensure that data sent to or from Workfront can pass through your organization's firewall.
---

# Firewall overview

Because *Adobe Workfront* communicates with your organization's network, your organization's firewall must be configured to allow that communication. Firewalls are highly effective security measures that function by separating an organization's network from the internet. They ensure that only selected data and network traffic can move into or out of the organization's network. The firewall allows or blocks data based on the site that is sending or receiving the data. As an *Adobe Workfront administrator*, you must ensure that data sent to or from *Workfront* can pass through your organization's firewall.

This is accomplished through an allowlist, which is essentially a "list" of sites that are "allowed" to send or receive data through the firewall. Sites can be identified in one of two ways:

* **IP address**: a series of numbers such as 52.31.132.175
* **Domain**: part of a URL, such as "thisdomain" in www.thisdomain.com

*Workfront* uses specific IP addresses and domains for web communication. These must be added to your organization's allowlist before you can use *Workfront* in your organization.

Generally, an allowlist is configured by a network administrator. Work with your organization's network administrator to ensure that your firewall allows these IP addresses. If you do not know who your network administrator is, your organization's IT department can point you in the right direction.

>[!IMPORTANT]
>
>As a *Workfront administrator*, you must ensure that these IP addresses and domains are added to your organization's allowlist. This is true even if you do not add them yourself. *Workfront* cannot configure your organization's allowlist.

## Collect information for configuring your firewall

To configure your firewall for *Workfront*, your network administrator needs to know which IP addresses and domains to add. Some of this information is available only to a *Workfront* administrator. As the Workfront administrator, you must locate this information and provide it to your network administrator.

>[!NOTE]
>
>The best practice for security is to add only the IP addresses and domains that connect to functionality your organization is actively using. By providing this information, you can ensure that this best practice is followed.

Provide your network administrator with the following information:

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Specific IP addresses and domains to allow</td> 
   <td> <p>The article <a href="../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md" class="MCXref xref">Configure your firewall's allowlist</a> contains the list of IP addresses and domains that your organization must add to its allowlist. </p> <p>Your network administrator might not have access to the "Configure your firewall" article. In that case, you must provide it to them. We do not recommend printing a hard (paper) copy. A digital copy allows your network administrator to copy and paste the addresses, which is quicker and more accurate than typing from a hard copy.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Your cluster</td> 
   <td>To locate your organization's cluster, see <a href="#locate" class="MCXref xref">View your organization's cluster and Workfront plan</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Your <em>Workfront</em> Plan</td> 
   <td> <p>Your organization's plan is one of the following:</p> 
    <ul> 
     <li> <p><em>Enterprise</em> </p> </li> 
     <li> <p><em>Business</em> </p> </li> 
     <li> <p><em>Pro</em> </p> </li> 
     <li> <p><em>Team</em> </p> </li> 
    </ul> <p>To locate your plan, see <a href="#locate" class="MCXref xref">View your organization's cluster and Workfront plan</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Your domain</td> 
   <td> <p>To locate your domain, look at the web address that you use to connect to <em>Workfront</em>.</p> <p>Example: in the web address <code>greatcompany.my.workfront.com</code>, the domain is "greatcompany"</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Other Adobe Workfront products</td> 
   <td> <p>Inform your network administrator if you have licenses for either of the following:</p> 
    <ul> 
     <li> <p><em>Adobe Workfront</em> <em>Proof</em></p> </li> 
     <li> <p><em>Adobe Workfront Fusion</em> </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront integrations</td> 
   <td>Inform your network administrator if you use any of the following:
    <ul>
     <li><p><p><em>Workfront</em> for Jira</p></p></li>
     <li><p><em>Workfront</em> for G Suite</p></li>
     <li><p><em>Workfront</em> for Microsoft Teams</p></li>
     <li><p><em>Workfront</em> for Outlook</p></li>
     <li><p><em>Workfront</em> for Salesforce</p></li>
    </ul></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Additional Functionality</td> 
   <td> <p>Inform your network administrator if you use either of the following:</p> 
    <ul> 
     <li> <p>A <em>Workfront</em> test drive</p> </li> 
     <li> <p><em>Workfront</em> Ascent</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

>[!IMPORTANT]
>
>If you add any of these products, integrations, or functionalities at a later date, you must contact your network administrator so they can adjust the allowlist.

### View your organization's cluster and *Workfront* plan

<ol> 
 <li value="1">Click the <span class="bold">Main Menu</span> icon <img src="assets/main-menu-icon.png"> in the upper-right corner of <em>Adobe Workfront</em>, then click <span class="bold">Setup</span> <img src="assets/gear-icon-settings.png">.</li> 
 <li value="2">Click <b>System</b> in the left panel</li> 
 <li value="3"> <p>To view your cluster, Select <b>Customer Info</b>. </p> <p>Your cluster displays near the upper-right of the <b>Basic Info</b> section.</p> <draft-comment>
   <p data-mc-conditions="QuicksilverOrClassic.Quicksilver"> <img src="assets/locate-cluster-350x189.png" style="width: 350;height: 189;"> </p>
  </draft-comment><p data-mc-conditions="QuicksilverOrClassic.Quicksilver"> <img src="assets/locate-cluster-350x189.png" style="width: 350;height: 189;"> </p> </li> 
 <li value="4"> <p>To view your <em>Workfront</em> plan, select <b>Licenses</b>.</p> <p>Your plan displays near the bottom of the page.</p> <draft-comment>
   <p data-mc-conditions="QuicksilverOrClassic.Quicksilver"> <img src="assets/locate-plan-350x162.png" style="width: 350;height: 162;"> </p>
  </draft-comment><p data-mc-conditions="QuicksilverOrClassic.Quicksilver"> <img src="assets/locate-plan-350x162.png" style="width: 350;height: 162;"> </p> </li> 
</ol>

