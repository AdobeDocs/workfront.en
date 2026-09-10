---
product-area: projects
navigation-topic: manage-issues
title: Automatically Update Issue Statuses from Awaiting Feedback to In Progress
description: When the Primary Contact of an issue makes an update to the issue by either updating a field (including a custom field) or adding a comment, the issue status updates to In Progress automatically.
author: Alina
feature: Work Management
exl-id: f94bb644-910f-4b46-80fd-fecbdf9cb18a
TQID: https://experienceleague.adobe.com/axgDUT8M6p79omHTSO8OrvM7qAM81AjG0Fug2JUl4ck
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
    internal-label: Work management
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
    internal-label: Administration
subfeature_v2:
  - id: f0dd7b45-76b5-49d4-afe3-39f436b6fbd3
    internal-label: Projects
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
---
# Automatically update issue statuses from Awaiting Feedback to In Progress

<!--Audited: 109/2025-->

When the Primary Contact of an issue makes an update to the issue by either updating a field (including a custom field) or adding a comment, the issue status updates to In Progress automatically.

In order for this automatic status change to occur, the following are required:

* The issue must be added using a request queue.

  For information about creating request queues, see the [Create and manage Request Queues](../../../manage-work/requests/create-and-manage-request-queues/create-manage-request-queues.md) section. 
  
  For information about submitting requests to a request queue, see [Create and submit Adobe Workfront requests](../../../manage-work/requests/create-requests/create-submit-requests.md).

* The Queue Details in the request queue must have these settings:  
  * **When someone makes a request, automatically grant** is set to **Contribute Access** 
  * **Change Status** is selected

  ![Queue Details give Contribute Access and Change Status is selected.](assets/queuedetails-contributeaccess-changestatus.png)

  >[!IMPORTANT]
  >
  >  When setting up a request queue, you can define the access primary contacts have to the issues they submit. 
  >
  >When you deselect the Change Status setting when setting up the request queue, remember that system administrators always have access to change the status of issues, even if the Change Status option is deselected in the request queue settings. 

  For more information about Queue Details, see [Create a Request Queue](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

* The issue must be in Awaiting Feedback status.
* There must be an Awaiting Feedback (AWF) status available for issues at the system level.

  For more information about system-level statuses, see [Create or edit a status](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).
