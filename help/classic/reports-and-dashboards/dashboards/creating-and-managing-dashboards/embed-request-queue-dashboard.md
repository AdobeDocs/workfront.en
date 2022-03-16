---
filename: embed-request-queue-dashboard
product-area: dashboards
navigation-topic: create-and-manage-dashboards
title: Embed a request queue in a dashboard
description: You can embed a new request queue in a dashboard to provide direct access to the request queue to your users, without having to go to the Requests area.
---

# Embed a request queue in a dashboard

You can embed a new request queue in a dashboard to provide direct access to the request queue to your users, without having to go to the Requests area.&nbsp;

For example, if you have a request queue that is open to your entire organization, like a Help Desk Queue, or a PTO Request queue that everyone must access on a regular basis, it might be convenient to insert the request queue directly into one of their dashboards for quick and easy access. The process of setting this up is similar to that of creating an external page on a dashboard.

First, you need to obtain a URL to the request queue. Secondly, you can embed the URL into a dashboard by adding an external page.

## Access requirements

You must have the following access to perform the steps in this article:

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to&nbsp;Reports, Dashboards,&nbsp;Calendars</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to the dashboard</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects in Adobe Workfront</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your Workfront administrator.

## Prerequisites

Both of the following must be created before you can embed a request queue in a dashboar:

* **The dashboard**: For information on creating dashboards, see [Create a dashboard](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/create-dashboard.md).
* **The request queue**: For information on creating request queues, see [Create a Request Queue](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md)

## Obtain the URL of the request queue

You can obtain the URL of a request queue in multiple ways, depending on what portion of the request queue you want to expose to the users when they access it from a dashboard.

* [Obtain a link to a specific queue topic with ability to change the request type](#obtain2) 
* [Obtain a link to a request queue and ability to change the request type](#obtain3) 
* [Obtain a link to a request queue with no ability to change the request type](#obtain4)

### Obtain a link to a specific queue topic with ability to change the request type

When you share a link to a specific queue topic with other users, the request form opens at the exact queue topic that they need to use to submit the request. This is helpful when users might not be sure which queue topic to choose when logging requests for a specific request queue.

Users can change the request type or choose another topic if they need to. The navigation of the Requests area also displays.

1. Go to the Requests area in your Global Navigation Bar. 
1. Continue selecting topic groups and queue topics until you reach the queue you want to share on the dashboard, if you want to share specific queue. For information about submitting requests, see [Create and submit Adobe Workfront requests](../../../manage-work/requests/create-requests/create-submit-requests.md).

   >[!TIP]
   >
   >Selecting topic groups and queue topics is optional.

1. Obtain the URL of the request queue from your address bar.

### Obtain a link to a request queue and ability to change the request type

When you share a link to a request type, the request type is selected for the user. This is helpful when users need to choose from multiple topic groups or queue topics for the same request type. Users can change the request type and choose another one. The navigation of the Requests area also displays.

1. Go to a project designated as a request queue.

   For information about creating a request queue from a project, go to [Create a Request Queue](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md). 

1. Go to Queue Setup > Queue Details. 
1. Copy the code that you find in the `Direct Access URL` field.

   The code should look similar to the following:

   `<samp>https://<yourdomain>.my.workfront.com/requests/new?activeTab=tab-new-helpRequest&projectID=50062d6f000849c95ab3513c0e84a51e&path=</samp>`

   This is the link to the request queue associated with the selected project.The Request Type is preselected.

   Users can select any topic group or queue topic they need, or they can choose another request type.

### Obtain a link to a request queue with no ability to change the request type

When you share a link to a preselected request type, the request type is selected for the user and cannot be changed . Users can choose the topic groups or queue topics they need. This is helpful when you do not want users to view and select other request types. The navigation of the Requests area does not display.

1. Go to a project designated as a request queue.

   For information about creating a request queue from a project, go to [Create a Request Queue](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md). 

1. Go to Queue Setup > Queue Details. 
1. Copy the code that you find in the `Embedded Code` field.

   The code should look similar to the following:

   `<samp><iframe src="https://<yourdomain>my.workfront.com/requests/newRequestEmbedded?projectID=612518c7000404462d3bc9a0bc09fa71" frameborder="0" width="500" height="600"></iframe></samp>` 

1. Edit the code to preserve only the information below:

   `<samp>https://<yourdomain>.my.workfront.com/requests/newRequestEmbedded?projectID=612518c7000404462d3bc9a0bc09fa71</samp>`

   >[!TIP]
   >
   >You can preserve the `<samp>iframe </samp>`tag when embedding the code in an application other than&nbsp;Workfront.

   This is the link to the request queue associated with the selected project. The Request Type is preselected and cannot be changed.

   Users can select any topic group or queue topic they need for the selected request type. Users cannot select another request type.

## Embed a request queue in a dashboard

You can embed a link to the requests queue or to a queue topic nested under a request queue into a dashboard to give users direct access to entering requests.

1. Obtain a request queue&nbsp;URL using one of the methods described in the [Obtain the URL of the request queue](#obtain) section of this article. 
1. Go to Reporting in your Global Navigation Bar, then select the Dashboards tab. 
1. Type a `Name` for the dashboard. This is a required field.
1. Click `Add External Page`.

1. In the `Add External Page` box, edit the following fields:

  * `Name`: enter the name of the request queue as you want it to appear on the dashboard. This is a required field.

  * `Description`: enter a description about that this external page displays. This is not a required field and it is important only for reporting purposes. It does not display in the dashboard.&nbsp;
  * `URL`:paste the URL you obtained using one of the methods described in Step 1.
  * `Height`: enter the height of the external page. This defines how much space the external page containing the request queue occupies on the dashboard. This is a required field and the default value is 500.&nbsp;

1. Click `Save`. 
1. Click `Save + Close`.&nbsp;

   The request queue displays in the dashboard as a separate dashboard component.&nbsp;

1. (Optional) Click `Dashboard Actions`, then `Edit` to add reports, calendars, or additional external pages to the same dashboard.  
   For information about adding components to a dashboard, see [Create a dashboard](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/create-dashboard.md).

&nbsp;

&nbsp;

<!--
Go to the Requests area in your Global Navigation Bar. Select the Request Type for the queue you would like added to the dashboard. (Optional) Select a Queue Topic and a Topic Group. Depending on how the project manager set up the request queue, the names of these fields are different in each Workfront instance. Go to the URL of this request queue in your browser, and copy the portion of the URL starting with projectID=. Note: The pathID can sometimes have no value. Copy the entire rest of the URL, starting with projectID=, including the value of the pathID, if there is one. For example, your information from the URL might look like one of the following: projectID=5c53339f0017e56de1b41278355f9fa8&path= projectID=555f815500fe2d8bdb898dd975d70c53&path=565e01c8027d2749044c9aef223999c3 Use the following example to build the URL of your external page. Replace the portion of the URL indicated in bold with information from your Workfront instance: https://<yourCompanyDomain>.my.workfront.com/requests/newRequestEmbedded?projectID=<the projectID and pathID information you copied from the request queue in Step 4>. The resulting URL should be similar to one of the following: https://yourcompany.my.workfront.com/requests/newRequestEmbedded?projectID=5c53339f0017e56de1b41278355f9fa8&path= https://yourcompany.my.workfront.com/requests/newRequestEmbedded?projectID=555f815500fe2d8bdb898dd975d70c53&path=565e01c8027d2749044c9aef223999c3 Copy the URL you built in Step 5. For example, enter a URL similar to one of the following: https://yourcompany.my.workfront.com/requests/newRequestEmbedded?projectID=5c53339f0017e56de1b41278355f9fa8&path= https://yourcompany.my.workfront.com/requests/newRequestEmbedded?projectID=555f815500fe2d8bdb898dd975d70c53&path=565e01c8027d2749044c9aef223999c3
-->

