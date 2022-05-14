---
filename: about-connecting-wf-fusion-to-app-or-service
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: connections-annd-webhooks
title: About connecting Adobe Workfront Fusion to an app or service
description: For most apps, it is necessary to create a connection, through which Adobe Workfront Fusion can communicate with the given third-party service according to the settings of the specific scenario.
---

# About connecting Adobe Workfront Fusion to an app or service

For most apps, it is necessary to create a connection, through which Adobe Workfront Fusion can communicate with the given third-party service according to the settings of the specific scenario.

For example, if you want to create a scenario that retrieves information from Workfront, you must grant access permission for Workfront Fusion to access your Workfront account.

## Access requirements

You must have the following access to use the functionality in this article:

<table> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Pro or higher</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Plan, Work</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront Fusion license**</td> 
   <td> <p>Workfront Fusion for Work Automation and Integration </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>Your organization must purchase Adobe Workfront Fusion as well as Adobe Workfront to use functionality described in this article.</td> 
  </tr> <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td role="rowheader">Access level configurations*</td> 
    <td>
      <p data-mc-conditions="QuicksilverOrClassic.Draft mode">You must be a Workfront Fusion administrator for your organization.</p>
      <p data-mc-conditions="QuicksilverOrClassic.Draft mode">You must be a Workfront Fusion administrator for your team.</p>
    </td> 
   </tr>
  --> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your Workfront administrator.

&#42;&#42;For information on Adobe Workfront Fusion licenses, see [Adobe Workfront Fusion licenses](../../workfront-fusion/get-started/license-automation-vs-integration.md)

## Access rights

For every connection, Workfront Fusion requires only those access rights that are necessary to successfully complete a given scenario. For example, if you create a scenario to list documents from Google Docs, Workfront Fusion does not ask for permission to get the content of the documents.

Unfortunately, not all services allow you to limit access to specific tasks. Therefore, Workfront Fusion must require full access rights. For more information on how to restrict Workfront Fusion access to your account registered to those services, see the application-specific documentation.

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">Organizational data security is Workfront Fusion's top priority. For detailed information on how data is secured and protected in Workfront Fusion, click here.
<MadCap:conditionalText style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">
Sam: Exclude until after GA release
</MadCap:conditionalText>
</p>
-->

## About administering connections

You can administer all connections from one place in the Connections section. Here you can:

* See which permissions were given to Workfront Fusion for each connection
* Rename connections 
* Reauthorize existing connections
* Delete existing connections
* Verify that the connection to the service was established successfully

## Renew a connection

Workfront Fusion usually obtains access rights to a given service for an unlimited period of time. However, this is not always the case. With some services, the access permission must be renewed after a certain period of time. In these cases, Workfront Fusion notifies you via email shortly before its access rights expire.

To renew a connection:

1. Click the **Reauthorize** button in the **Connections** section.

