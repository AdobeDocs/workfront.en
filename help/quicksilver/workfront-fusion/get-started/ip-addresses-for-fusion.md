---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: get-started-with-workfront-fusion-2-0
title: IP Addresses for accessing Adobe Workfront Fusion
description: The Adobe Workfront Fusion documentation has moved to a new location. This article has been deprecated, but contains a link to the new article that covers this functionality.
author: Becky
feature: Workfront Fusion
exl-id: f6295cc7-367f-4c8b-891b-cc11ff42a225
---
# IP Addresses for accessing [!DNL Adobe Workfront Fusion]

>[!IMPORTANT]
>
>The Adobe Workfront Fusion documentation has moved to a new location. 
>
>The information in this article can now be found in the article:
>
>* [Configure IP Addresses for Fusion in your organization's allowlist](https://experienceleague.adobe.com/docs/workfront-fusion/using/set-up-and-manage-fusion/set-up-and-manage-orgs-and-teams/set-up-orgs-teams-and-users/set-up-ip-addresses-for-fusion.html)
>
>Please update any bookmarks.
>
>This article is no longer being updated, and will be removed in the near future.

>[!NOTE]
>
>[!DNL Adobe Workfront Fusion] requires an [!DNL Adobe Workfront Fusion] license in addition to an [!DNL Adobe Workfront license].

If your firewall or mail server is configured to allow access to only certain vendors, you must add certain IP addresses to its allowlist in order to allow open communication between your environment and [!DNL Adobe Workfront Fusion].

You can add all Fusion IP addresses and domains to your allowlist, or you can locate your Fusion cluster and add only the IP addresses and domains for that cluster.

## Add all Fusion IP addresses and domains

Add the following IP addresses to your allowlist:

* 52.30.133.50
* 54.220.93.204 
* 34.254.76.122
* 54.244.142.219 
* 52.39.217.230 
* 44.241.82.96
* 100.20.126.137
* 34.223.32.4
* 52.39.176.220
* 20.36.133.48/28 
* 20.81.156.240/28 
* 172.172.84.48/28 

Also, if your organization uses outbound network filtering, add the following domain to your allowlist to enable your system to access Workfront Fusion.

* hook.app.workfrontfusion.com
* hook.app-eu.workfrontfusion.com
* hook.app-az.workfrontfusion.com

## Add Fusion IP addresses and domains for your cluster only

### Identify your datacenter

The IP addresses vary based on where your data is stored. 

If you access Fusion through a URL, you can examine the URL to locate your datacenter.

| URL | Datacenter |
| --- | --- |
| `https://app.workfrontfusion.com/` | US datacenter |
| `https://app-eu.workfrontfusion.com/` | EU datacenter |
| `https://app-az.workfrontfusion.com/` | Azure datacenter |

If you access Fusion through experience.adobe.com, you can check the network tab in your browser to identify the datacenter.

| URL | Datacenter |
| --- | --- |
| Calls to `https://fusion.adobe.com` |US datacenter |
| Calls to `https://eu.fusion.adobe.com` | EU datacenter |
| Calls to `https://az.fusion.adobe.com`  | Azure datacenter |

### Add IP addresses and domains for your datacenter

Add the following IP addresses to your allowlist to enable [!DNL Workfront Fusion] to access your system.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] EU Datacenter</td> 
   <td> 
    <ul> 
     <li>52.30.133.50</li> 
     <li>54.220.93.204</li> 
     <li>34.254.76.122</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Adobe Workfront] US Datacenter</p> </td> 
   <td> 
    <ul> 
     <li>54.244.142.219</li> 
     <li>52.39.217.230</li> 
     <li>44.241.82.96</li>
     <li>100.20.126.137</li>
     <li>34.223.32.4</li>
     <li>52.39.176.220</li>
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] on the Microsoft Azure cluster</td> 
   <td> 
    <ul> 
     <li>20.36.133.48/28</li> 
     <li>20.81.156.240/28</li> 
     <li>172.172.84.48/28</li> 
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
   <td role="rowheader">[!DNL Adobe Workfront] EU Datacenter</td> 
   <td> <p> hook.app-eu.workfrontfusion.com </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Adobe Workfront] US Datacenter</p> </td> 
   <td> <p>hook.app.workfrontfusion.com </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Adobe Workfront Fusion] on the Microsoft Azure cluster</p> </td> 
   <td> <p>hook.app-az.workfrontfusion.com </p> </td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>Outbound network filtering is uncommon. Check with your network administrator to see if you need to update your allowlist to accommodate for it.

For more information on setting up your organization's allowlist, see [Configure your firewall's allowlist](../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).
