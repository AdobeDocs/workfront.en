---
user-type: administrator
product-area: system-administration;setup
navigation-topic: start-with-workfront-administration
title: Configure your firewall's allowlist
description: If your firewall or mail server is configured to allow access to only certain vendors, you must add certain IP addresses to its allowlist. This opens communication between your environment and the Adobe Workfront servers and allows your users to send messages from Workfront and to use SSO with Active Directory or LDAP.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 264eed40-6d90-498b-83cc-2500c8b19c84
---
# Configure your firewall's allowlist

<!-- Audited: 12/2023 -->

>[!IMPORTANT]
>
>The procedure described on this page applies only to organizations that have not yet been onboarded to the Admin Console. If your organization has been onboarded to the Adobe Admin Console, you must perform this action through the Adobe Admin Console.
>
>To configure your allowlist if your organization has been onboarded to the Adobe Admin Console, see [Domains to be allowed for Adobe Apps and Services](https://helpx.adobe.com/enterprise/kb/network-endpoints.html).
>
>For a list of procedures that differ based on whether your organization has been onboarded to the Adobe Admin Console, see [Platform-based administration differences (Adobe Workfront/Adobe Business Platform)](../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

>[!NOTE]
>
>The way an organization configures its allowlist is unique to each organization. Work with your IT team to identify your organization's procedure and implement these additions.

If your firewall or mail server is configured to allow access to only certain vendors, you must add certain IP addresses to its allowlist. This opens communication between your environment and the Adobe Workfront servers and allows the following processes:

* Sending messages from the Workfront application

  >[!NOTE]
  >
  >This is not available if your organization's Workfront instance is enabled with Adobe IMS. See your network or IT administrator if you need more information.

* Using document webhooks when configuring custom document integrations
* Using Workfront Event Subscriptions

  For more information, see [Event Subscription API](https://experience.workfront.com/s/article/Event-Subscription-API-2100945680).

You also need to open certain ports in order for email messages to be encrypted when they are delivered.

## Workfront allowlists you can use

If your organization has the Enterprise plan, you can also configure two Workfront allowlists:

* **Email allowlist**: Lets you control where users can email data stored in Workfront. For more information, see [Configure your email allowlist](../../administration-and-setup/get-started-wf-administration/configure-your-email-allowlist.md).
* **IP allowlist**: Limits access to Workfront to 45 IP addresses or IP address ranges that you specify, providing an additional layer of security for the Workfront application. For more information, see [Restrict access to Adobe Workfront by IP address](../../administration-and-setup/manage-workfront/security/restrict-access-workfront-ip-address.md).

## Locate your Workfront cluster

The IP addresses that you must add to your allowlist on your firewall depend on the cluster where your Production environment runs. 

To locate your organization's cluster:

1. As a Workfront administrator, click the **Main Menu** icon ![Main Menu](assets/main-menu-icon.png), then click **Setup**.
1. In the left navigation, click **System**, then select **Customer Info**.
1. Locate the **Cluster Setup** field at the upper-right corner of the page. Your organization's cluster is listed here.

   CL01 refers to Cluster 1, CL02 is Cluster 2, and so on.

For more information, see the section [View your organization's cluster and Workfront plan](../../administration-and-setup/get-started-wf-administration/firewall-overview.md#view-your-organizations-cluster-and-workfront-plan) in the article [Firewall overview](../../administration-and-setup/get-started-wf-administration/firewall-overview.md).

## IP addresses to add to the allowlist

>[!IMPORTANT]
>
>Some Workfront integrations do not work when the allowlist is enabled because they can't be configured with a static IP address. To use the following integrations, you must disable the allowlist.
>
>* Workfront for G Suite 
>* Workfront for Outlook 
>* Workfront for Salesforce

* [IP addresses to allow for Clusters 1, 2, 3, 5, 7, 8 and 9](#ip-addresses-to-allow-for-clusters-1-2-3-5-7-8-and-9) 
* [IP addresses to allow for Cluster 4](#ip-addresses-to-allow-for-cluster-4) 
* [IP addresses to allow for Cluster 6](#ip-addresses-to-allow-for-cluster-6) 
* [IP addresses to allow for a Test Drive](#IP%20Addre2) 
* [IP addresses to allow when implementing event subscriptions](#ip-addresses-to-allow-when-implementing-event-subscriptions) 
* [IP addresses to allow for enhanced authentication](#ip-addresses-to-allow-for-enhanced-authentication) 
* [IP addresses to add for accessing Workfront Fusion](#ip-addresses-to-add-for-accessing-workfront-fusion) 
* [IP addresses to add for using Workfront for Jira](#ip-addresses-to-add-for-using-workfront-for-jira) 
* [URLs to add for all clusters Workfront](#urls-to-add-for-all-clusters-workfront)

### IP addresses to allow for Clusters 1, 2, 3, 5, 7, 8 and 9 {#ip-addresses-to-allow-for-clusters-1-2-3-5-7-8-and-9}

If your Production environment is on Cluster 1, 2, 3, 5, or 7 you must allow the following IP addresses.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">For SSO, document webhooks, or other functionality</td> 
   <td> 
    <ul> 
     <li>35.160.0.242</li> 
     <li>34.213.36.118</li> 
     <li>3.209.27.146</li> 
     <li>18.205.251.4</li> 
     <li>34.211.224.9</li> 
     <li>54.218.48.56</li> 
     <li>52.36.154.34</li> 
     <li>54.244.142.219</li> 
     <li>52.39.217.230</li> 
     <li>44.241.82.96</li> 
     <li>54.203.255.135/32</li> 
     <li>35.155.2.51/32</li> 
     <li>52.34.192.77/32</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">To receive email from the Workfront application</td> 
   <td> 
    <ul> 
     <li>54.240.60.174</li> 
     <li>54.240.60.175</li> 
     <li>13.58.86.183</li> 
     <li>34.209.181.84</li> 
     <li>35.161.82.137</li> 
     <li>52.14.70.114</li> 
     <li>52.15.230.220</li> 
     <li>54.71.252.65</li> 
    </ul> <p>For information about the following IP addresses, see <a href="../../product-announcements/announcements/announcement-archive/new-email-ip-21-1.md" class="MCXref xref">New IP addresses for Adobe Workfront email with the 21.1 release</a></p> 
    <ul> 
     <li>23.251.237.107</li> 
     <li>23.251.237.108</li> 
     <li>23.251.237.109</li> 
     <li>23.251.237.106</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### IP addresses to allow for Cluster 4 {#ip-addresses-to-allow-for-cluster-4}

If your Production environment is on Cluster 4, add the following IP addresses for SSO, document webhook integrations, and to receive email from the Workfront application:

* 52.31.132.175
* 52.19.188.226
* 52.28.49.94
* 52.29.41.175
* 52.29.197.69
* 52.48.124.108 
* 69.169.230.231
* 69.169. 230.232
* 3.121.91.129
* 3.122.11.35
* 34.246.27.40
* 52.208.123.166
* 52.208.159.124
* 52.17.130.201
* 34.252.250.191
* 52.30.133.50
* 54.220.93.204
* 34.254.76.122
* 34.242.62.80/32
* 46.51.194.192/32
* 54.229.129.66/32

For information about the following IP addresses, see [New IP addresses for Adobe Workfront email with the 21.1 release](../../product-announcements/announcements/announcement-archive/new-email-ip-21-1.md)

* 23.251.239.98
* 23.251.239.99

### IP addresses to allow for Cluster 6 {#ip-addresses-to-allow-for-cluster-6}

If your Production environment is on Cluster 6, add the following IP addresses.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">To receive email from the Workfront application</td> 
   <td> 
    <ul> 
     <li>34.94.227.64</li> 
     <li>34.94.227.65</li> 
     <li>34.94.227.66</li> 
     <li>34.94.227.67</li> 
     <li>34.66.82.64</li> 
     <li>34.66.82.65</li> 
     <li>34.66.82.66</li> 
     <li>34.66.82.67</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">To use the AWS email service</td> 
   <td> 
    <ul> 
     <li>54.240.60.174</li> 
     <li>54.240.60.175</li> 
     <li>13.58.86.183</li> 
     <li>34.209.181.84</li> 
     <li>35.161.82.137</li> 
     <li>52.14.70.114</li> 
     <li>52.15.230.220</li> 
     <li>54.71.252.65 </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### IP addresses to allow for a Test Drive

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">To receive email from the Workfront application when using a Test Drive</td> 
   <td> 
    <ul> 
     <li>69.42.126.188 </li> 
     <li>66.119.37.185</li> 
     <li>66.119.37.186</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">For SSO and document webhook integrations when using a Test Drive</td> 
   <td> 
    <ul> 
     <li> <p>69.42.126.188:</p> <p>This address must also be added to your allowlist in order for your users to receive emails from Workfront.</p> </li> 
     <li>66.119.37.186</li> 
     <li>66.119.37.167</li> 
     <li>54.244.142.219</li> 
     <li>52.39.217.230</li> 
     <li>44.241.82.96</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### IP addresses to allow when implementing event subscriptions  {#ip-addresses-to-allow-when-implementing-event-subscriptions}

For all environments, add the following IP addresses to receive payloads from Workfront event subscriptions.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> For customers in Europe</td> 
   <td> 
    <ul> 
     <li>52.30.133.50</li> 
     <li>52.208.159.124</li> 
     <li>54.220.93.204</li> 
     <li>52.17.130.201</li> 
     <li>34.254.76.122</li> 
     <li>34.252.250.191</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">For customers in locations other than Europe</td> 
   <td> 
    <ul> 
     <li>54.244.142.219</li> 
     <li>44.241.82.96</li> 
     <li>52.36.154.34</li> 
     <li>34.211.224.9</li> 
     <li>54.218.48.56</li> 
     <li>52.39.217.230</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### IP addresses to allow for enhanced authentication {#ip-addresses-to-allow-for-enhanced-authentication}

Add the following IP addresses to use enhanced authentication for Preview or Production.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">If your environment is on Cluster 1, 2, 3, 5, 7, 8, or 9</td> 
   <td> 
    <ul> 
     <li>35.167.74.121</li> 
     <li>35.166.202.113</li> 
     <li>35.160.3.103</li> 
     <li>54.183.64.135</li> 
     <li>54.67.77.38</li> 
     <li>54.67.15.170</li> 
     <li>54.183.204.205</li> 
     <li>35.171.156.124</li> 
     <li>18.233.90.226</li> 
     <li>3.211.189.167</li> 
     <li>18.232.225.224</li> 
     <li>34.233.19.82</li> 
     <li>52.204.128.250</li> 
     <li>3.132.201.78</li> 
     <li>3.19.44.88</li> 
     <li>3.20.244.231</li> 
     <li>54.244.142.219</li> 
     <li>52.39.217.230</li> 
     <li>44.241.82.96</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">If your environment is on Cluster 4</td> 
   <td> 
    <ul> 
     <li>52.28.56.226</li> 
     <li>52.28.45.240</li> 
     <li>52.16.224.164</li> 
     <li>52.16.193.66</li> 
     <li>34.253.4.94</li> 
     <li>52.50.106.250</li> 
     <li>52.211.56.181</li> 
     <li>52.213.38.246</li> 
     <li>52.213.74.69</li> 
     <li>52.213.216.142</li> 
     <li>35.156.51.163</li> 
     <li>35.157.221.52</li> 
     <li>52.28.184.187</li> 
     <li>52.28.212.16</li> 
     <li>52.29.176.99</li> 
     <li>52.57.230.214</li> 
     <li>54.76.184.103</li> 
     <li>52.210.122.50</li> 
     <li>52.208.95.174</li> 
     <li>52.30.133.50</li> 
     <li>54.220.93.204</li> 
     <li>34.254.76.122</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### IP addresses to add for accessing Workfront Fusion  {#ip-addresses-to-add-for-accessing-workfront-fusion}

Add the following IP addresses to your allowlist to enable Workfront Fusion to access your system.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront EU Datacenter</td> 
   <td> 
    <ul> 
     <li>52.30.133.50</li> 
     <li>54.220.93.204</li> 
     <li>34.254.76.122</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Adobe Workfront US Datacenter</p> </td> 
   <td> 
    <ul> 
     <li>54.244.142.219</li> 
     <li>52.39.217.230</li> 
     <li>44.241.82.96</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

Also, if your organization uses outbound network filtering, add the following domain to your allowlist to enable your system to access Workfront Fusion. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront EU Datacenter</td> 
   <td> <p> hook.app-eu.workfrontfusion.com </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Adobe Workfront US Datacenter</p> </td> 
   <td> <p>hook.app.workfrontfusion.com </p> </td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>Outbound network filtering is uncommon. Check with your network administrator to see if you need to update your allowlist to accommodate for it.

### IP addresses to add for using Workfront for Jira {#ip-addresses-to-add-for-using-workfront-for-jira}

Add the following IP addresses to your allowlist to use the Workfront for Jira integration.

The jira.workfront.com domain must also be accessible from your corporate servers. This domain is required because it serves as middleware between Workfront and Jira.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> For customers in Europe</td> 
   <td> 
    <ul> 
     <li>52.30.133.50</li> 
     <li>52.208.159.124</li> 
     <li>54.220.93.204</li> 
     <li>52.17.130.201</li> 
     <li>34.254.76.122</li> 
     <li>34.252.250.191</li> 
     <li>35.162.128.73</li> 
     <li>52.42.25.64</li> 
     <li>34.213.36.118</li> 
     <li>35.160.0.242 </li> 
     <li> <p>3.209.27.146</p> </li> 
     <li> <p>18.205.251.4</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">For customers in locations other than Europe</td> 
   <td> 
    <ul> 
     <li>54.244.142.219</li> 
     <li>44.241.82.96</li> 
     <li>52.36.154.34</li> 
     <li>34.211.224.9</li> 
     <li>54.218.48.56</li> 
     <li>52.39.217.230</li> 
     <li>35.162.128.73</li> 
     <li>52.42.25.64</li> 
     <li>34.213.36.118</li> 
     <li>35.160.0.242 </li> 
     <li>3.209.27.146</li> 
     <li>18.205.251.4</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

## Domains to add for accessing Workfront

If your organization uses outbound network filtering, add the following domains to your allowlist to enable your system to access Workfront.

>[!NOTE]
>
>Outbound network filtering is uncommon. Check with your network administrator to see if you need to update your allowlist to accommodate for it.

* `<your domain>`.my.workfront.com
* `<your domain>`.preview.workfront.com
* `<your domain>`.sb01.workfront.com
* `<your domain>`.sb02.workfront.com
* events.split.io
* sdk.split.io
* auth.split.io
* rum-http-intake.logs.datadoghq.com
* mfe.static.workfront.com
* https://app.pendo.io/
* https://cdn.pendo.io/

## URLs to add for all clusters Workfront {#urls-to-add-for-all-clusters-workfront}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">To allow help content to display in your Workfront environment</td> 
   <td> 
    <ul> 
     <li>https://app.pendo.io/</li> 
     <li>https://cdn.pendo.io/</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">To allow Workfront Proof to access Workfront on any cluster, add these to all environments</td> 
   <td> 
    <ul> 
     <li>*.workfront.com - Required to view proofs in Workfront</li> 
     <li>*.proofhq.com - Required to view proofs in Workfront Proof</li> 
     <li>*.proofhq.eu - Required to view proofs in Workfront Proof</li> 
    </ul> <p><b>NOTE</b>:  <p>We do not support adding IP addresses to your allowlist for Workfront Proof. They have been dynamic after Workfront moved to AWS. Instead, we recommend that you allow Workfront Proof domains only.</p> <p>If there is an issue with adding these domains to your allowlist and you need an IP address instead, contact Workfront Customer Support.</p> </p> </td> 
  </tr> 
 </tbody> 
</table>

## IP addresses and URLs to add for accessing Workfront Proof

You must add the following IP addresses to your allowlist in order to use various functions.

* [For callbacks and webcapture proofs](#for-callbacks-and-webcapture-proofs) 
* [For outgoing email](#for-outgoing-email)

### For callbacks and webcapture proofs {#for-callbacks-and-webcapture-proofs}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Prod-US (Clusters 1, 2, 3, 5, and 7)</td> 
   <td> 
    <ul> 
     <li>34.213.36.118</li> 
     <li>35.160.0.242</li> 
     <li>3.209.27.146</li> 
     <li>18.205.251.4</li> 
     <li>35.165.152.202</li> 
     <li>54.184.151.122</li> 
     <li>35.84.40.190</li> 
     <li>54.218.48.56</li> 
     <li>34.211.224.9</li> 
     <li>52.36.154.34</li> 
     <li>34.232.138.38</li> 
     <li>54.237.6.156</li> 
     <li>54.237.12.32</li> 
     <li>44.241.82.96</li> 
     <li>54.244.142.219</li> 
     <li>52.39.217.230</li> 
     <li>52.207.47.153</li> 
     <li>50.16.118.214</li> 
     <li>52.54.180.191</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Prod-EU (Cluster 4)</td> 
   <td> 
    <ul> 
     <li>34.246.27.40</li> 
     <li>52.208.123.166</li> 
     <li>3.121.91.129</li> 
     <li>3.122.11.35</li> 
     <li>34.241.103.51</li> 
     <li>46.51.203.201</li> 
     <li>54.247.174.227</li> 
     <li>52.208.159.124</li> 
     <li>52.17.130.201</li> 
     <li>34.252.250.191</li> 
     <li>52.30.133.50</li> 
     <li>54.220.93.204</li> 
     <li>34.254.76.122</li> 
    </ul> <p><b>NOTE</b>: DNS server options are no longer supported.</p> </td> 
  </tr> 
 </tbody> 
</table>

### For outgoing email {#for-outgoing-email}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>Prod-US (Clusters 1, 2, 3, 5, and 7)</p> </td> 
   <td> 
    <ul> 
     <li> 23.251.237.106</li> 
     <li>23.251.237.107</li> 
     <li>23.251.237.108</li> 
     <li>54.240.60.174</li> 
     <li>54.240.60.175</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Prod-EU (Cluster 4)</td> 
   <td> 
    <ul> 
     <li>23.251.239.98</li> 
     <li>69.169.230.231</li> 
     <li>69.169.230.232</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

## Ports to open for best Workfront Proof performance

Open the following ports if you are experiencing problems with proofs loading or not working in Workfront Proof:

* 5671
* 5672
* 15671

## Ports to open for encrypted email

Emails from the Workfront application are sent encrypted using ports 465 and 587. If your mail server does not support encrypted email, emails are delivered unencrypted using port 25.

## Email notifications from Workfront Support

If you are not receiving emails from Workfront Support, ensure that you add the Salesforce IP addresses and domains that you need. For more information, see the Salesforce help article about Salesforce IP addresses and domains to allow.
