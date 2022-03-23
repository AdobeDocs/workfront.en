---
filename: configure-access-to-blueprints
user-type: administrator
product-area: system-administration;workfront-integrations
navigation-topic: best-practices-catalog
title: Configure access to blueprints
description: The information on this page refers to functionality not yet generally available. It is available only in the Preview Sandbox environment.
---

# Configure access to blueprints

The information on this page refers to functionality not yet generally available. It is available only in the Preview Sandbox environment.

All Adobe Workfront users can browse the catalog of blueprints. As a system administrator, you can enable access for users to request installation of blueprints by setting up a request queue to store the requests. There, you have a single location to track and update requests.

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">You can also define whether users with specific access levels can request blueprint installation or only browse the catalog.</p>
-->

Only the system administrator can install blueprints. For information, see [Install a blueprint](../../administration-and-setup/blueprints/blueprints-install.md).

## Access requirements

You must have the following access to perform the steps in this article:

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan</td> 
   <td> <p> Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>System administrator</p> </td> 
  </tr> 
 </tbody> 
</table>

## Set up the request queue

Before users can request that you install blueprints for them, you must set up a request queue for those requests. Until the request queue is set up, users can only browse the blueprints catalog.

You must use an existing request queue for the blueprint requests. If you want to create a new request queue, you should build it before setting up blueprints access. For information on creating a request queue, see [Create a Request Queue](../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

1. Click the **Main Menu** icon ![](assets/main-menu-icon.png) in the upper-right corner of Adobe Workfront, then click**Blueprints**.
1. Click **Configure blueprint requests**.
1. In the **Blueprints access setup** dialog, ensure that the **Configure request queues** tab is selected.
1. Begin typing the name of an active request queue, and select it when it appears in the search results.

   The request queue preference is set, and users can now request blueprint installation.

   To change the preference to a different request queue, click **Edit this request queue.**

1. (Optional) If the request queue has queue topics, you can select a topic from the list of available topics.
1. To return to the blueprints catalog, click **Close**.

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Define access levels</h2>
<p>After setting up the request queue, you can define whether users with specific access levels can request blueprint installation or only browse the catalog.</p>
<ol>
<li value="1"> <p>Click the <strong>Main Menu</strong> icon <img src="assets/main-menu-icon.png"> in the upper-right corner of Adobe Workfront, then click <strong>Setup</strong> <img src="assets/gear-icon-settings.png">.</p> </li>
</ol>
</div>
-->

