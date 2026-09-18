---
product-area: workfront-integrations
navigation-topic: workfront-for-slack
title: Search for [!DNL Adobe Workfront] items from [!DNL Slack]
description: You can search for [!DNL Adobe Workfront] items from [!DNL Slack], if your instance of Slack has had the [!DNL Workfront] app installed.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 85821f21-d4fd-4f28-bd7a-0c109a4433a8
TQID: https://experienceleague.adobe.com/JulYq173XQa6mG93qzUwfBDn4TPVEafD2OVpcIAXxi8
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
    internal-label: Administration
  - id: f48b5020-b9cd-4d99-bc6e-42c35e90c1f8
    internal-label: Integrations
subfeature_v2:
  - id: e4fedd42-4a54-4109-859f-13c7f0366a72
    internal-label: Adobe Workfront for Slack
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
---
# Search for [!DNL Adobe Workfront] items from [!DNL Slack]

You can search for [!DNL Adobe Workfront] items from [!DNL Slack], if your instance of [!DNL Slack] has had the [!DNL Workfront] app installed. 

For more information about configuring [!DNL Workfront] with [!DNL Slack], see [Configure [!DNL Adobe Workfront] for [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/configure-workfront-for-slack.md).

## Access requirements

+++ Expand to view access requirements for the functionality in this article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront package</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license</td> 
   <td> <p>Any</p>
  </tr> 
 </tbody> 
</table>

For information, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md). 

+++

## Prerequisites

Before you can search for [!DNL Workfront] items from [!DNL Slack], you must

* Configure [!DNL Workfront] for [!DNL Slack]\
   For instructions on configuring [!DNL Workfront for Slack], see [Configure [!DNL Adobe Workfront for Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/configure-workfront-for-slack.md).

## Search for [!DNL Workfront] items from [!DNL Slack]:

1. Log in to your [!DNL Slack] instance and log in to [!DNL Workfront] from [!DNL Slack].\
   For more information about logging in to [!DNL Workfront] from [!DNL Slack], see the "Logging In to [!DNL Workfront] from [!DNL Slack]" section in [Access [!DNL Adobe Workfront] from [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md).

1. From any channel, start typing either of the following commands in the message field: 

   `/workfront search <keyword>`

   Or

   `/wf search <keyword>`

   >[!NOTE]
   >
   >Commands are case sensitive. The keyword is not case sensitive and it must be entered without brackets or quotation marks.
   
1. In the field that appears, select an object type from the following:

   * Project
   * Task
   * Issue
   * Report
   * People
   * Template
   * Document
   * Portfolio
   * Program
   * Dashboard
   * Company
   * Note

      You can only select one object type at a time.\
      A list of items that match the search criteria displays.

1. Click the name of an item to open it in [!DNL Workfront] in a new browser tab.
