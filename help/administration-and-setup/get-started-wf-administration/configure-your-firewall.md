---
filename: configure-your-firewall
user-type: administrator
product-area: system-administration;setup
navigation-topic: start-with-workfront-administration
title: Configure your firewall's allowlist
description: If your firewall or mail server is configured to allow access to only certain vendors, you must add certain IP addresses to its allowlist. This opens communication between your environment and the Adobe Workfront servers and allows the following processes:
---

# Configure your firewall's allowlist

If your firewall or mail server is configured to allow access to only certain vendors, you must add certain IP addresses to its allowlist. This opens communication between your environment and the `Adobe Workfront` servers and allows the following processes:

<ul> 
 <li>Sending messages from the <span>Workfront</span> application</li> 
 <li> <p>Using single sign-on (SSO) with Active Directory or Lightweight Directory Access Protocol (LDAP)</p> <note type="note">
   This is not available if your organization’s 
   <span>Workfront</span> instance is enabled with Adobe IMS. See your network or IT administrator if you need more information.
  </note> </li> 
 <li>Using document webhooks when configuring custom document integrations</li> 
 <li> <p>Using <span>Workfront</span> Event Subscriptions</p> <p>For more information, see Event Subscription API.<br></p> </li> 
</ul>

You also need to open certain ports in order for email messages to be encrypted when they are delivered.

## `Workfront` allowlists you can use

If your organization has the `Enterprise` plan, you can also configure two `Workfront` allowlists:

* **Email allowlist**: Lets you control where users can email data stored in `Workfront`. For more information, see [Configure your email allowlist](../../administration-and-setup/get-started-wf-administration/configure-your-email-allowlist.md).
* **IP allowlist**: Limits access to `Workfront` to 45 IP addresses or IP address ranges that you specify, providing an additional layer of security for the `Workfront` application. For more information, see [Restrict access to Adobe Workfront by IP address](../../administration-and-setup/manage-workfront/security/restrict-access-workfront-ip-address.md).

## IP addresses to add to the allowlist

The IP addresses that you must add to your allowlist on your firewall depend on the cluster where your Production environment runs. You can find out which cluster this is by viewing Setup > System > Custom Info. For more information, see the section [Configure Basic Info](../../administration-and-setup/get-started-wf-administration/configure-basic-info.md#configuring-basic-info) in the article [Configure basic information for your system](../../administration-and-setup/get-started-wf-administration/configure-basic-info.md).

>[!IMPORTANT]
>
>Some `Workfront` integrations do not work when the allowlist is enabled because they can’t be configured with a static IP address. To use the following integrations, you must disable the allowlist.
>
>* `Workfront for G Suite` 
>* `Workfront for Outlook` 
>* `Workfront for Salesforce` 
>

* [IP addresses to allow for Clusters 1, 2, 3, 5, 7, 8 and 9](#ip5)<![CDATA[                ]]>
* [IP addresses to allow for Cluster 4](#cluster-4) 
* [IP addresses to allow for Cluster 6](#ip3) 
* [IP addresses to allow for a Test Drive](#ip%20addre2) 
* [IP addresses to allow when implementing event subscriptions](#ip-addresses-to-whitelist-when-implementing-event-subscriptions) 
* [IP addresses to allow for enhanced authentication](#ip6) 
* [IP addresses to add for accessing Workfront Fusion](#ip-addresses-to-add-for-accessing-workfront-fusion) 
* [IP addresses to add for using Workfront for Jira](#ip) 
* [IP addresses to add for using Workfront Ascent](#ip2) 
* [URLs to add for all clusters Workfront](#urls2)

### IP addresses to allow for Clusters 1, 2, 3, 5, 7, 8 and 9

If your Production environment is on Cluster 1, 2, 3, 5, or 7 you must allow the following IP addresses.

<table cellspacing="0"> 
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
     <li> <p>18.205.251.4</p> </li> 
     <li> <p>34.211.224.9</p> </li> 
     <li> <p>54.218.48.56</p> </li> 
     <li> <p>52.36.154.34</p> </li> 
     <li> <p>54.244.142.219</p> </li> 
     <li> <p>52.39.217.230</p> </li> 
     <li> <p>44.241.82.96</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">To receive email from the <span>Workfront</span> application</td> 
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
    </ul> <p>For information about the following IP addresses, see <a href="../../product-announcements/announcements/new-email-ip-21.1.md" class="MCXref xref">New IP addresses for Adobe Workfront email with the 21.1 release</a></p> 
    <ul> 
     <li> <p>23.251.237.107</p> </li> 
     <li> <p>23.251.237.108</p> </li> 
     <li> <p>23.251.237.109</p> </li> 
     <li> <p>23.251.237.106</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### IP addresses to allow for Cluster 4

If your Production environment is on Cluster 4, add the following IP addresses for SSO, document webhook integrations, and to receive email from the `Workfront` application:

* 52.31.132.175
* 52.19.188.226
* 52.28.49.94
* 52.29.41.175
* 52.29.197.69
* 52.48.124.108 
* 69.169.230.231
* 69.169. `230`.232
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

For information about the following IP addresses, see [New IP addresses for Adobe Workfront email with the 21.1 release](../../product-announcements/announcements/new-email-ip-21.1.md)

* 23.251.239.98
* 23.251.239.99

### IP addresses to allow for Cluster 6

If your Production environment is on Cluster 6, add the following IP addresses.

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">To receive email from the <span>Workfront</span> application</td> 
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

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">To receive email from the <span>Workfront</span> application when using a Test Drive</td> 
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
     <li>69.42.126.188 (this address must also be added to your allowlist in order for your users to receive emails from <span>Workfront</span>)</li> 
     <li>66.119.37.186</li> 
     <li>66.119.37.167</li> 
     <li>54.244.142.219</li> 
     <li>52.39.217.230</li> 
     <li>44.241.82.96</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### IP addresses to allow when implementing event subscriptions

For all environments, add the following IP addresses to receive payloads from `Workfront` event subscriptions.

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> For customers in Europe</td> 
   <td> 
    <ul> 
     <li> <p>52.30.133.50</p> </li> 
     <li> <p>52.208.159.124</p> </li> 
     <li> <p>54.220.93.204</p> </li> 
     <li> <p>52.17.130.201</p> </li> 
     <li> <p>34.254.76.122</p> </li> 
     <li> <p>34.252.250.191</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">For customers in locations other than Europe</td> 
   <td> 
    <ul> 
     <li> <p>54.244.142.219</p> </li> 
     <li> <p>44.241.82.96</p> </li> 
     <li> <p>52.36.154.34</p> </li> 
     <li> <p>34.211.224.9</p> </li> 
     <li> <p>54.218.48.56</p> </li> 
     <li> <p>52.39.217.230</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### IP addresses to allow for enhanced authentication

Add the following IP addresses to use enhanced authentication for Preview or Production.

<table cellspacing="0"> 
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

### IP addresses to add for accessing `Workfront Fusion`

Add the following IP addresses to your allowlist to enable `Workfront Fusion` to access your system.

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront EU Datacenter</td> 
   <td> 
    <ul> 
     <li> <p>52.30.133.50</p> </li> 
     <li> <p>54.220.93.204</p> </li> 
     <li> <p>34.254.76.122</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Adobe Workfront US Datacenter</p> </td> 
   <td> 
    <ul> 
     <li> <p>54.244.142.219</p> </li> 
     <li> <p>52.39.217.230</p> </li> 
     <li> <p>44.241.82.96</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

Also, if your organization uses outbound network filtering, add the following domain to your allowlist to enable your system to access `Workfront Fusion`.

* hook.app.workfrontfusion.com

>[!NOTE]
>
>Outbound network filtering is uncommon. Check with your network administrator to see if you need to update your allowlist to accommodate for it.

### IP addresses to add for using `Workfront` for Jira

Add the following IP addresses to your allowlist to use the `Workfront` for Jira integration.

The jira.workfront.com domain must also be accessible from your corporate servers. This domain is required because it serves as middleware between `Workfront` and Jira.

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> For customers in Europe</td> 
   <td> 
    <ul> 
     <li> <p>52.30.133.50</p> </li> 
     <li> <p>52.208.159.124</p> </li> 
     <li> <p>54.220.93.204</p> </li> 
     <li> <p>52.17.130.201</p> </li> 
     <li> <p>34.254.76.122</p> </li> 
     <li> <p>34.252.250.191</p> </li> 
     <li> <p>35.162.128.73</p> </li> 
     <li> <p>52.42.25.64</p> </li> 
     <li> <p>34.213.36.118</p> </li> 
     <li> <p>35.160.0.242 </p> </li> 
     <li> <p>3.209.27.146</p> </li> 
     <li> <p>18.205.251.4</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">For customers in locations other than Europe</td> 
   <td> 
    <ul> 
     <li> <p>54.244.142.219</p> </li> 
     <li> <p>44.241.82.96</p> </li> 
     <li> <p>52.36.154.34</p> </li> 
     <li> <p>34.211.224.9</p> </li> 
     <li> <p>54.218.48.56</p> </li> 
     <li> <p>52.39.217.230</p> </li> 
     <li> <p>35.162.128.73</p> </li> 
     <li> <p>52.42.25.64</p> </li> 
     <li> <p>34.213.36.118</p> </li> 
     <li> <p>35.160.0.242 </p> </li> 
     <li> <p>3.209.27.146</p> </li> 
     <li> <p>18.205.251.4</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### IP addresses to add for using Workfront Ascent

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">To access <span>Workfront</span> training resources via <span>Workfront</span> Ascent</td> 
   <td> 
    <ul> 
     <li>18.223.140.34</li> 
     <li>3.13.223.30</li> 
     <li>3.13.19.112</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">To receive email notifications from <span>Workfront</span> Ascent</td> 
   <td> 
    <ul> 
     <li> <p>23.251.227.75</p> </li> 
     <li> <p>23.251.227.76</p> </li> 
     <li> <p>23.251.227.77</p> </li> 
     <li> <p>23.251.227.78</p> </li> 
     <li> <p>23.251.227.79</p> </li> 
     <li> <p>23.251.227.80</p> </li> 
     <li> <p>23.251.227.81</p> </li> 
     <li> <p>23.251.227.82</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

## Domains to add for accessing `Workfront`

If your organization uses outbound network filtering, add the following domains to your allowlist to enable your system to access `Workfront`.

>[!NOTE]
>
>Outbound network filtering is uncommon. Check with your network administrator to see if you need to update your allowlist to accommodate for it.

* <your domain>.my.workfront.com
* <your domain>.preview.workfront.com
* <your domain>.sb01.workfront.com
* <your domain>.sb02.workfront.com
* events.split.io
* sdk.split.io
* auth.split.io
* rum-http-intake.logs.datadoghq.com
* mfe.static.workfront.com
* https://app.pendo.io/
* https://cdn.pendo.io/

## URLs to add for all clusters `Workfront`

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">To allow help content to display in your <span>Workfront</span> environment</td> 
   <td> 
    <ul> 
     <li>https://app.pendo.io/</li> 
     <li>https://cdn.pendo.io/</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">To allow <span>Workfront Proof</span> to access <span>Workfront</span> on any cluster, add these to all environments</td> 
   <td> 
    <ul> 
     <li>*.workfront.com - Required to view proofs in <span>Workfront</span></li> 
     <li>*.proofhq.com - Required to view proofs in <span>Workfront Proof</span></li> 
     <li>*.proofhq.eu - Required to view proofs in <span>Workfront Proof</span></li> 
    </ul> <p>Note:  <p>We do not support adding IP addresses to your allowlist for <span>Workfront Proof</span>. They have been dynamic after <span>Workfront</span> moved to AWS. Instead, we recommend that you allow <span>Workfront Proof</span> domains only.</p> <p>If there is an issue with adding these domains to your allowlist and you need an IP address instead, contact Workfront Customer Support.</p> </p> </td> 
  </tr> 
 </tbody> 
</table>

## IP addresses and URLs to add for accessing `Workfront Proof`

The highlighted information in this section was announced on October 15, 2021, and are required as of November 15, 2021.

You must add the following IP addresses to your allowlist in order to use various functions.

* [For callbacks and webcapture proofs](#for) 
* [For outgoing email](#for2)

### For callbacks and webcapture proofs

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Prod-US (Clusters 1, 2, 3, 5, and 7)</td> 
   <td> 
    <ul> 
     <li> <p>34.213.36.118</p> </li> 
     <li> <p>35.160.0.242</p> </li> 
     <li> <p>3.209.27.146</p> </li> 
     <li> <p>18.205.251.4</p> </li> 
     <li> <p>35.165.152.202</p> </li> 
     <li> <p>54.184.151.122</p> </li> 
     <li> <p>35.84.40.190</p> </li> 
     <li> <p>54.218.48.56</p> </li> 
     <li> <p>34.211.224.9</p> </li> 
     <li> <p>52.36.154.34</p> </li> 
     <li> <p>34.232.138.38</p> </li> 
     <li> <p>54.237.6.156</p> </li> 
     <li> <p>54.237.12.32</p> </li> 
     <li> <p>44.241.82.96</p> </li> 
     <li> <p>54.244.142.219</p> </li> 
     <li> <p>52.39.217.230</p> </li> 
     <li> <p>52.207.47.153</p> </li> 
     <li> <p>50.16.118.214</p> </li> 
     <li> <p>52.54.180.191</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Prod-EU (Cluster 4)</td> 
   <td> 
    <ul> 
     <li> <p>34.246.27.40</p> </li> 
     <li> <p>52.208.123.166</p> </li> 
     <li> <p>3.121.91.129</p> </li> 
     <li> <p>3.122.11.35</p> </li> 
     <li> <p>34.241.103.51</p> </li> 
     <li> <p>46.51.203.201</p> </li> 
     <li> <p>54.247.174.227</p> </li> 
     <li> <p>52.208.159.124</p> </li> 
     <li> <p>52.17.130.201</p> </li> 
     <li> <p>34.252.250.191</p> </li> 
     <li> <p>52.30.133.50</p> </li> 
     <li> <p>54.220.93.204</p> </li> 
     <li> <p>34.254.76.122</p> </li> 
    </ul> <p>Note: DNS server options are no longer supported.</p> </td> 
  </tr> 
 </tbody> 
</table>

### For outgoing email

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>Prod-US (Clusters 1, 2, 3, 5, and 7)</p> </td> 
   <td> 
    <ul> 
     <li> <p> 23.251.237.106</p> </li> 
     <li> <p>23.251.237.107</p> </li> 
     <li> <p>23.251.237.108</p> </li> 
     <li> <p>54.240.60.174</p> </li> 
     <li> <p>54.240.60.175</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Prod-EU (Cluster 4)</td> 
   <td> 
    <ul> 
     <li> <p>23.251.239.98</p> </li> 
     <li> <p>69.169.230.231</p> </li> 
     <li> <p>69.169.230.232</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

## Ports to open for best `Workfront Proof` performance

Open the following ports if you are experiencing problems with `proofs` loading or not working in `Workfront Proof`:

* 5671
* 5672
* 15671

## Ports to open for encrypted email

Emails from the `Workfront` application are sent encrypted using ports 465 and 587. If your mail server does not support encrypted email, emails are delivered unencrypted using port 25.

## Email notifications from `Workfront` Support

If you are not receiving emails from `Workfront` Support, ensure that you add the Salesforce IP addresses and domains that you need. For more information, see the Salesforce help article about Salesforce IP addresses and domains to allow.
