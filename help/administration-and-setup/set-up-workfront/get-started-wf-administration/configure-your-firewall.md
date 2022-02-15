---
filename: configure-your-firewall
user-type: administrator
product-area: system-administration;setup
navigation-topic: start-with-workfront-administration
---




# Configure your firewall {#configure-your-firewall}

If your firewall or mail server is configured to allow access only to specific vendors, you must add certain IP addresses to the allowlist in order to allow open communication between your environment and the `Workfront` servers. (This is required in order to perform any of the processes described in the section, [Workfront processes that require firewall access](#workfront-processes-that-require-firewall-access).)


You also need to open certain ports in order for email messages to be delivered encrypted.


For information about allowing access to `Workfront` only from designated IP addresses, see .


## IP addresses to add to the allowlist<![CDATA[    ]]> {#ip-addresses-to-add-to-the-allowlist}

The IP addresses that you must add to your allowlist on your firewall vary depending on the cluster where your Production environment is running.&nbsp;


To find out what cluster your Production environment is on, contact  `Workfront` Support (see [Contact Customer Support](contact-customer-support.md)).



* [IP addresses to allow for Clusters 1, 2, 3, and 5](#ip5)<![CDATA[                ]]>
* [IP addresses to allow for Cluster 4](#cluster-4) 
* [IP addresses to allow for Cluster 6](#ip3) 
* [IP addresses to allow for a Test Drive](#ip%c2%a0addre2) 
* [IP addresses to allow when implementing Event Subscriptions](#ip-addresses-to-whitelist-when-implementing-event-subscriptions) 




### IP addresses to allow for Clusters 1, 2, 3, and 5 {#ip-addresses-to-allow-for-clusters-and}

If your Production environment is on Cluster 1, 2, 3, or 5, add the following IP addresses for SSO and to receive email from the  `Workfront` application:


#### For SSO: {#for-sso}




* 35.160.0.242
* 34.213.36.118
* 3.209.27.146
* 18.205.251.4




#### For email: {#for-email}




* 54.240.60.174
* 54.240.60.175
* 13.58.86.183
* 34.209.181.84
* 35.161.82.137
* 52.14.70.114
* 52.15.230.220
* 54.71.252.65




### IP addresses to allow for Cluster 4 {#ip-addresses-to-allow-for-cluster}




If your Production environment is on Cluster 4, add the following IP addresses for SSO and to receive email from the  `Workfront` application:



*  52.31.132.175
*  52.19.188.226
*  52.28.49.94
*  52.29.41.175
*  52.29.197.69
*  52.48.124.108&nbsp;
*  69.169.230.231
*  69.169.230.232
*  3.121.91.129
*  3.122.11.35
*  34.246.27.40
*  52.208.123.166




### IP addresses to allow for Cluster 6 {#ip-addresses-to-allow-for-cluster-1}

If your Production environment is on Cluster 6, add the following IP addresses for receiving email from the  `Workfront` application:



* 34.94.227.64
* 34.94.227.65
* 34.94.227.66
* 34.94.227.67
* 34.66.82.64
* 34.66.82.65
* 34.66.82.66
* 34.66.82.67


In addition to adding the above IP&nbsp;addresses to your allowlist, you must also add the following IP&nbsp;addresses to your allowlist in order to use the AWS email service:



* 54.240.60.174
* 54.240.60.175
*  13.58.86.183
*  34.209.181.84
*  35.161.82.137
*  52.14.70.114
*  52.15.230.220
*  54.71.252.65




### IP&nbsp;addresses to allow for a Test Drive {#ip-addresses-to-allow-for-a-test-drive}

Add the following IP addresses for receiving email from the  `Workfront` application when using&nbsp;a Test Drive:



* 69.42.126.188
* 66.119.37.185
* 66.119.37.186


Add the following IP addresses for SSO when using a Test Drive:



* 69.42.126.188 (this address must also be added to your allowlist to receive emails from `Workfront`)
* 66.119.37.186
* 66.119.37.167




### IP addresses to allow when implementing Event Subscriptions  {#ip-addresses-to-allow-when-implementing-event-subscriptions}

For all environments, add the following IP addresses to receive payloads from `Workfront` Event Subscriptions:



* 35.162.39.124
* 52.89.16.253&nbsp;




## IP addresses to add for accessing `Workfront Fusion 2.0`  {#ip-addresses-to-add-for-accessing-workfront-fusion}

Add the following IP addresses to your allowlist to ensure access to `Workfront Fusion 2.0` 2.0:



* 35.160.0.242
* 34.213.36.118
* 3.209.27.146
* 18.205.251.4




## IP addresses to add for accessing Legacy Workfront Fusion {#ip-addresses-to-add-for-accessing-legacy-workfront-fusion}

Add the following IP addresses to your allowlist to ensure access to `Workfront Fusion 2.0` 2.0:



* 18.216.172.146
* 18.218.153.209




## IP addresses to add for using `Workfront` for Jira {#ip-addresses-to-add-for-using-workfront-for-jira}

Add the following IP address to your allowlist to use the `Workfront` for Jira integration:



* 35.162.128.73


The jira.workfront.com domain must also be accessible from your corporate servers. This domain is required because it serves as middleware between `Workfront` for Jira.


## IP addresses to add for using Workfront Ascent {#ip-addresses-to-add-for-using-workfront-ascent}

Add the following IP address to your allowlist to access Workfront training resources via Workfront Ascent. 



* 18.223.140.34
* 3.13.223.30
* 3.13.19.112




## URLs to add for viewing guided tours and self-help content within `Workfront` {#urls-to-add-for-viewing-guided-tours-and-self-help-content-within-workfront}

Add the following URLs to allow guided tours and self-help content to display in your `Workfront` environment. 



* https://app.pendo.io/ 
* https://cdn.pendo.io/




## Domains to add for accessing `Workfront` {#domains-to-add-for-accessing-workfront}

For all environments, add the following domains to allow access to `Workfront` on any cluster:



*  events.split.io
* sdk.split.io




## URLs to add for accessing `Workfront Proof` {#urls-to-add-for-accessing-workfront-proof}

For all environments, add the following URLs to allow `Workfront Proof` to access `Workfront` on any cluster:



* &#42;.workfront.com - Required to view proofs 
* webcapture.int.proofhq.com - web capture tool
* mx.proofhq.com - email servers




>[!NOTE]
>
>We do not support adding IP addresses to your allowlist for `Workfront Proof`. They are dynamic since Workfront moved to AWS. Instead, we recommend that you allow `Workfront Proof` domains only.
>
>
>If there is an issue with adding these domains to your allowlist and an IP address is needed instead, please contact Workfront Customer Support.





## Ports to open to ensure best `proof` performance with `Workfront Proof` {#ports-to-open-to-ensure-best-proof-performance-with-workfront-proof}

Open the following ports if you are experiencing problems with `proofs` loading or not working:



* 5671
* 5672




## Ports to open for&nbsp;encrypted email {#ports-to-open-for-encrypted-email}

Emails from the  `Workfront` application&nbsp;are sent encrypted using ports 465 and 587. If your mail server does not support encrypted email,&nbsp;emails are delivered unencrypted using port 25.


## `Workfront` processes that require firewall access {#workfront-processes-that-require-firewall-access}

Add certain `Workfront` IP addresses to your firewall allowlist for the following purposes:



* Allowing messages from the `Workfront`&nbsp;application
* Using Single Sign-On (SSO) with Active Directory or LDAP
*  Using Document&nbsp;Webhooks when configuring custom document integrations. 


  For more information, see&nbsp; [Configure document integrations](configure-document-integrations.md).

* Using `Workfront` Event Subscriptions  
  For more information, see [Event Subscription API](https://experience.workfront.com/s/article/Event-Subscription-API-2100945680).



