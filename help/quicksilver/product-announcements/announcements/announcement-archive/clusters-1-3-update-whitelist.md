---
content-type: reference
navigation-topic: announcements
title: Customers on Clusters 1, 2, and 3 must update any allowlist IP blocks to prevent the blocking of Adobe Workfront services
description: To enhance and improve our core infrastructure, we will soon migrate Adobe Workfront customers on Clusters 01, 02, and 03 to the AWS public cloud.
author: Luke
feature: Product Announcements
exl-id: 77d43206-1db7-4075-a063-043f8c9f75ed
TQID: https://experienceleague.adobe.com/I6EiM5bD37m-gC5wyB3DBaOscSTMX-18BpjogM1LcgU
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
    internal-label: Administration
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
topic_v2:
  - id: d095671a-1355-40aa-8b5f-06c33c68080b
    internal-label: Security
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
---
# Customers on Clusters 1, 2, and 3 must update any allowlist IP blocks to prevent the blocking of Adobe Workfront services

To enhance and improve our core infrastructure, we will soon migrate Adobe Workfront customers on Clusters 01, 02, and 03 to the AWS public cloud.

As part of this change, you need to add the following IPs to your allowlist IP blocks in order to prevent the blocking of Workfront services:

For SSO and POP:

* 34.215.145.168
* 54.69.155.48
* 35.160.44.226
* 34.213.96.218
* 3.16.210.22
* 3.16.229.153
* 18.224.117.99
* 3.18.123.153
* 3.211.159.196
* 3.85.255.45
* 3.210.78.197
* 3.211.23.183

For email:

* 54.240.60.174
* 54.240.60.175

Please ensure your allowlist IP blocks are updated by May 13, 2019. For more information, see [Configure your firewall's allowlist](../../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).

Thank you for your continued support of Workfront as we work to create a more reliable and robust experience for our customers.

If you have any additional questions, please reach out to our Support team by visiting experience.workfront.com or by calling 844.306.4357 (US) or +44.1256.274200 (EMEA).

## FAQ

### Why is Workfront making this change?

In an effort to consistently provide our customers with the best possible service, Workfront constantly looks at ways to improve the user experience. This change makes use of new technologies that enable us to provide the best experience possible and improve our already robust security model.

### What actions are required by me as a Workfront administrator?

Contact your internal IT or security department for assistance in reviewing your allowlist IP blocks and in adding the IPs listed above.

### What can my organization expect if we do not make this change?

You will be unable to access Workfront services as we migrate services to the new IPs.
