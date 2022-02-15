---
filename: configure-your-firewall
user-type: administrator
product-area: system-administration;setup
navigation-topic: start-with-workfront-administration
---



# Configure your firewall {#configure-your-firewall}

If your firewall or mail server is configured to allow access to only certain vendors, you must add certain IP addresses to its allowlist. This opens communication between your environment and the *`Adobe Workfront`* servers and allows the following processes:



* Sending messages from the *`Workfront`* application
*  Using single sign-on (SSO) with Active Directory or Lightweight Directory Access Protocol (LDAP)
* Using document webhooks when configuring custom document integrations
*  Using *`Workfront`* Event Subscriptions


  For more information, see [Event Subscription API](https://experience.workfront.com/s/article/Event-Subscription-API-2100945680).  




You also need to open certain ports in order for email messages to be encrypted when they are delivered.


>[!TIP] {type="tip"}
>
>If your organization uses the *`Enterprise`* plan, you can configure the *`Workfront`* email allowlist to control where users can email data stored in *`Workfront`*. For more information, see [Configure your email allowlist](configure-your-email-allowlist.md).




## Access requirements {#access-requirements}

You must have the following to perform the steps in this article:

<table style="width: 100%;margin-left: 0;margin-right: auto;mc-table-style: url('../../Resources/TableStyles/TableStyle-List-options-in-steps.css');" class="TableStyle-TableStyle-List-options-in-steps" cellspacing="0"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2"> 
 <tbody> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader"><span class="mc-variable WFVariables.FullProdNameWF variable varname">Adobe Workfront</span> plan</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p>Any</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader"><span class="mc-variable WFVariables.FullProdNameWF variable varname">Adobe Workfront</span> license</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray"> <p><span class="mc-variable WFVariables.WFLicense-Plan variable varname">Plan</span> </p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-LightGray" role="rowheader">Access level configurations</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-LightGray"> <p>You must be a <span class="mc-variable WFVariables.AdminWF variable varname">Workfront administrator</span>. For more information, see <a href="grant-a-user-full-administrative-access.md" class="MCXref xref">Grant a user full administrative access</a>.</p> <p>Note: If you still don't have access, ask your <span class="mc-variable WFVariables.AdminWF variable varname">Workfront administrator</span> if they set additional restrictions in your access level. For information on how a <span class="mc-variable WFVariables.AdminWF variable varname">Workfront administrator</span> can modify your access level, see <a href="create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>



## IP addresses to add to the allowlist  {#ip-addresses-to-add-to-the-allowlist}

The IP addresses that you must add to your allowlist on your firewall depend on the cluster where your Production environment runs. You can find out which cluster this is by viewing Setup > System > Custom Info. For more information, see the section [Configure Basic Info](configure-basic-info.md#configuring-basic-info) in the article [Configure basic information for your system](configure-basic-info.md).


>[!IMPORTANT] {type="important"}
>
>Some *`Workfront`* integrations do not work when the allowlist is enabled because they can’t be configured with a static IP address. To use the following integrations, you must disable the allowlist.
>
>
>
>* *`Workfront for G Suite`* 
>* *`Workfront`* for Microsoft Teams
>* *`Workfront for Outlook`* 
>* *`Workfront for Salesforce`* 
>
>






* [IP addresses to allow for Clusters 1, 2, 3, 5, and 7](#ip5)<![CDATA[                ]]>
* [IP addresses to allow for Cluster 4](#cluster-4) 
* [IP addresses to allow for Cluster 6](#ip3) 
* [IP addresses to allow for a Test Drive](#ip%20addre2) 
* [IP addresses to allow when implementing event subscriptions](#ip-addresses-to-whitelist-when-implementing-event-subscriptions) 
* [IP addresses to allow for enhanced authentication](#ip6) 
* [IP addresses to add for accessing Workfront Fusion](#ip-addresses-to-add-for-accessing-workfront-fusion) 
* [IP addresses to add for using Workfront for Jira](#ip) 
* [IP addresses to add for using Workfront Ascent](#ip2) 
* [URLs to add for all clusters Workfront](#urls2) 




### IP addresses to allow for Clusters 1, 2, 3, 5, and 7 {#ip-addresses-to-allow-for-clusters-and}

If your Production environment is on Cluster 1, 2, 3, 5, or 7 you must allow the following IP addresses.

<table style="width: 100%;margin-left: 0;margin-right: auto;mc-table-style: url('../../Resources/TableStyles/TableStyle-List-options-in-steps.css');" class="TableStyle-TableStyle-List-options-in-steps" cellspacing="0"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2"> 
 <tbody> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader"> <h4>For SSO, document webhooks, or other functionality:</h4> </td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> 
    <ul> 
     <li>35.160.0.242</li> 
     <li>34.213.36.118</li> 
     <li>3.209.27.146</li> 
     <li> <p>18.205.251.4</p> <p>The following highlighted IP addresses were announced on October 15, 2021, and are required as of November 15, 2021.<br></p> </li> 
     <li> <p>34.211.224.9</p> </li> 
     <li> <p>54.218.48.56</p> </li> 
     <li> <p>52.36.154.34</p> </li> 
    </ul> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-MediumGray" role="rowheader">To receive email from the <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span> application:</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-MediumGray"> 
    <ul> 
     <li>54.240.60.174</li> 
     <li>54.240.60.175</li> 
     <li>13.58.86.183</li> 
     <li>34.209.181.84</li> 
     <li>35.161.82.137</li> 
     <li>52.14.70.114</li> 
     <li>52.15.230.220</li> 
     <li>54.71.252.65</li> 
    </ul> <p>For information about the following IP addresses, see <a href="new-email-ip-21.1.md" class="MCXref xref">New IP addresses for Adobe Workfront email with the 21.1 release</a></p> 
    <ul> 
     <li> <p>23.251.237.107</p> </li> 
     <li> <p>23.251.237.108</p> </li> 
     <li> <p>23.251.237.109</p> </li> 
     <li> <p>23.251.237.106</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>



### IP addresses to allow for Cluster 4 {#ip-addresses-to-allow-for-cluster}

If your Production environment is on Cluster 4, add the following IP addresses for SSO, document webhook integrations, and to receive email from the *`Workfront`* application:



*  52.31.132.175
*  52.19.188.226
*  52.28.49.94
*  52.29.41.175
*  52.29.197.69
*  52.48.124.108 
*  69.169.230.231
*  69.169.230.232
*  3.121.91.129
*  3.122.11.35
*  34.246.27.40
*  52.208.123.166


  The following highlighted IP addresses were announced on October 15, 2021, and are required as of November 15, 2021.  


*  52.208.159.124
*  52.17.130.201
*  34.252.250.191


For information about the following IP addresses, see [New IP addresses for Adobe Workfront email with the 21.1 release](new-email-ip-21.1.md)



*  23.251.239.98
*  23.251.239.99




### IP addresses to allow for Cluster 6 {#ip-addresses-to-allow-for-cluster-1}

If your Production environment is on Cluster 6, add the following IP addresses for receiving email from the *`Workfront`* application:



* 34.94.227.64
* 34.94.227.65
* 34.94.227.66
* 34.94.227.67
* 34.66.82.64
* 34.66.82.65
* 34.66.82.66
* 34.66.82.67


In addition to adding the above IP addresses to your allowlist, you must also add the following IP addresses to your allowlist in order to use the AWS email service:



* 54.240.60.174
* 54.240.60.175
*  13.58.86.183
*  34.209.181.84
*  35.161.82.137
*  52.14.70.114
*  52.15.230.220
*  54.71.252.65




### IP addresses to allow for a Test Drive {#ip-addresses-to-allow-for-a-test-drive}

Add the following IP addresses for receiving email from the *`Workfront`* application when using a Test Drive:



* 69.42.126.188
* 66.119.37.185
* 66.119.37.186


Add the following IP addresses for SSO, and document webhook integrations when using a Test Drive:



* 69.42.126.188 (this address must also be added to your allowlist in order for your users to receive emails from *`Workfront`*)
* 66.119.37.186
* 66.119.37.167




### IP addresses to allow when implementing event subscriptions  {#ip-addresses-to-allow-when-implementing-event-subscriptions}

For all environments, add the following IP addresses to receive payloads from *`Workfront`* event subscriptions:

<table style="width: 100%;margin-left: 0;margin-right: auto;mc-table-style: url('../../Resources/TableStyles/TableStyle-List-options-in-steps.css');" class="TableStyle-TableStyle-List-options-in-steps" cellspacing="0"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2"> 
 <tbody> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader"> For customers in Europe:</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> 
    <ul> 
     <li> <p>3.122.135.96</p> </li> 
     <li> <p>3.122.150.235</p> </li> 
     <li> <p>52.19.64.185</p> </li> 
     <li> <p>52.212.92.170</p> </li> 
    </ul> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-MediumGray" role="rowheader">For customers in locations other than Europe:</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-MediumGray"> 
    <ul> 
     <li> <p>35.160.0.242</p> </li> 
     <li> <p>34.213.36.118</p> </li> 
     <li> <p>3.209.27.146</p> </li> 
     <li> <p>18.205.251.4</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>



### IP addresses to allow for enhanced authentication {#ip-addresses-to-allow-for-enhanced-authentication}

If your environment is on Cluster 1, 2, 3, or 5, add the following IP addresses to use enhanced authentication for Preview or Production:



*  35.167.74.121
*  35.166.202.113
*  35.160.3.103
*  54.183.64.135
*  54.67.77.38
*  54.67.15.170
*  54.183.204.205
*  35.171.156.124
*  18.233.90.226
*  3.211.189.167
*  18.232.225.224
*  34.233.19.82
*  52.204.128.250
*  3.132.201.78
*  3.19.44.88
*  3.20.244.231


If your environment is on Cluster 4, add the following IP addresses to use enhanced authentication for Preview or Production:



*  52.28.56.226
*  52.28.45.240
*  52.16.224.164
*  52.16.193.66
*  34.253.4.94
*  52.50.106.250
*  52.211.56.181
*  52.213.38.246
*  52.213.74.69
*  52.213.216.142
*  35.156.51.163
*  35.157.221.52
*  52.28.184.187
*  52.28.212.16
*  52.29.176.99
*  52.57.230.214
*  54.76.184.103
*  52.210.122.50
*  52.208.95.174




### IP addresses to add for accessing *`Workfront Fusion`*  {#ip-addresses-to-add-for-accessing-workfront-fusion}

Add the following IP addresses to your allowlist to enable *`Workfront Fusion`* to access your system:



* 35.160.0.242
* 34.213.36.118
* 3.209.27.146
* 18.205.251.4


If your organization uses outbound network filtering, add the following domain to your allowlist to enable your system to access *`Workfront Fusion`*. 



*  hook.app.workfrontfusion.com 




>[!NOTE]
>
>Outbound network filtering is uncommon. Check with your network administrator to see if you need to update your allowlist to accommodate for it.




### IP addresses to add for using *`Workfront`* for Jira {#ip-addresses-to-add-for-using-workfront-for-jira}

Add the following IP address to your allowlist to use the *`Workfront`* for Jira integration:



*  35.162.128.73
*  52.42.25.64
*  34.213.36.118
*  35.160.0.242 
*  3.209.27.146
*  18.205.251.4  



The jira.workfront.com domain must also be accessible from your corporate servers. This domain is required because it serves as middleware between *`Workfront`* and Jira.


### IP addresses to add for using Workfront Ascent {#ip-addresses-to-add-for-using-workfront-ascent}

Add the following IP address to your allowlist to access *`Workfront`* training resources via *`Workfront`* Ascent:



* 18.223.140.34
* 3.13.223.30
* 3.13.19.112


Add the following IP addresses to your allowlist to receive email notifications from *`Workfront`* Ascent:



*  23.251.227.75
*  23.251.227.76
*  23.251.227.77
*  23.251.227.78
*  23.251.227.79
*  23.251.227.80
*  23.251.227.81
*  23.251.227.82




## Domains to add for accessing *`Workfront`* {#domains-to-add-for-accessing-workfront}

If your organization uses outbound network filtering, add the following domains to your allowlist to enable your system to access *`Workfront`*.


>[!NOTE]
>
>Outbound network filtering is uncommon. Check with your network administrator to see if you need to update your allowlist to accommodate for it.





*  <your domain>.my.workfront.com
*  <your domain>.preview.workfront.com
*  <your domain>.sb01.workfront.com
*  <your domain>.sb02.workfront.com
*  events.split.io
*  sdk.split.io
*  auth.split.io
*  rum-http-intake.logs.datadoghq.com
*  mfe.static.workfront.com
* https://app.pendo.io/
* https://cdn.pendo.io/




## URLs to add for all clusters *`Workfront`* {#urls-to-add-for-all-clusters-workfront}

Add the following URLs to allow help content to display in your *`Workfront`* environment. 



* https://app.pendo.io/
* https://cdn.pendo.io/




## IP addresses and URLs to add for accessing *`Workfront Proof`* {#ip-addresses-and-urls-to-add-for-accessing-workfront-proof}



### IP&nbsp;addresses to add {#ip-addresses-to-add}

The highlighted information in this section was announced on October 15, 2021, and are required as of November 15, 2021.


You must add the following IP&nbsp;addresses to your allowlist in order to use various functions.


**For callbacks and webcapture proofs:** 


Prod-US (Clusters 1, 2, 3, 5, and 7)


34.213.36.118


35.160.0.242


3.209.27.146


18.205.251.4


35.165.152.202


54.184.151.122


35.84.40.190


54.218.48.56


34.211.224.9


52.36.154.34


34.232.138.38


54.237.6.156


54.237.12.32


44.241.82.96


54.244.142.219


52.39.217.230


52.207.47.153


50.16.118.214


52.54.180.191


Prod-EU (Cluster 4)


34.246.27.40


52.208.123.166


3.121.91.129


3.122.11.35


34.241.103.51


46.51.203.201


54.247.174.227


52.208.159.124


52.17.130.201


34.252.250.191


52.30.133.50


54.220.93.204


34.254.76.122


Please note that DNS server options are no longer supported.


**For outgoing email:** 


prod-us (Clusters 1, 2, 3, 5, and 7)


23.251.237.106


23.251.237.107


23.251.237.108


54.240.60.174


54.240.60.175


prod-eu (Cluster 4)


23.251.239.98


69.169.230.231


69.169.230.232


### URLs to add {#urls-to-add}

For all environments, add the following URLs to allow *`Workfront Proof`* to access *`Workfront`* on any cluster:



* &#42;.workfront.com - Required to view proofs in *`Workfront`*
* &#42;.proofhq.com - Required to view proofs in *`Workfront Proof`*
* &#42;.proofhq.eu - Required to view proofs in *`Workfront Proof`*




>[!NOTE]
>
>We do not support adding IP addresses to your allowlist for *`Workfront Proof`*. They have been dynamic after *`Workfront`* moved to AWS. Instead, we recommend that you allow *`Workfront Proof`* domains only.
>
>
>If there is an issue with adding these domains to your allowlist and you need an IP address instead, contact Workfront Customer Support.





## Ports to open for best *`Workfront Proof`* performance {#ports-to-open-for-best-workfront-proof-performance}

Open the following ports if you are experiencing problems with *`proofs`* loading or not working in *`Workfront Proof`*:



* 5671
* 5672




## Ports to open for encrypted email {#ports-to-open-for-encrypted-email}

Emails from the *`Workfront`* application are sent encrypted using ports 465 and 587. If your mail server does not support encrypted email, emails are delivered unencrypted using port 25.


## Email notifications from *`Workfront`* Support {#email-notifications-from-workfront-support}

If you are not receiving emails from *`Workfront`* Support, ensure that you add the Salesforce IP addresses and domains that you need. For more information, see the Salesforce help article about Salesforce IP addresses and domains to allow.
