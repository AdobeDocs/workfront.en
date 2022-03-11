---
filename: ip-addresses-for-fusion
content-type: reference
product: workfront-fusion
product-area: workfront-integrations
navigation-topic: get-started-with-workfront-fusion-2-0
title: IP Addresses for accessing Adobe Workfront Fusion
description: Adobe Workfront Fusion requires an Adobe Workfront Fusion license in addition to an Adobe Workfront license.
---

# IP Addresses for accessing `Adobe Workfront Fusion`

`Adobe Workfront Fusion` requires an `Adobe Workfront Fusion` license in addition to an `Adobe Workfront` license.
If your firewall or mail server is configured to allow access to only certain vendors, you must add certain IP addresses to its allowlist in order to allow open communication between your environment and `Adobe Workfront Fusion`.

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

For more information on setting up your organization's allowlist, see [Configure your firewall's allowlist](../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).
