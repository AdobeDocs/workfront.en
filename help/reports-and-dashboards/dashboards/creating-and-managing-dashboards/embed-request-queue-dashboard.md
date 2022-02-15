---
filename: embed-request-queue-dashboard
product-area: dashboards
navigation-topic: create-and-manage-dashboards
---



# Embed a request queue in a dashboard {#embed-a-request-queue-in-a-dashboard}

You can embed a new request queue in a dashboard to provide direct access to the request queue to your users, without having to go to the Requests area.&nbsp;


For example, if you have a request queue that is open to your entire organization, like a Help Desk Queue, or a PTO Request queue that everyone must access on a regular basis, it might be convenient to insert the request queue directly into one of their dashboards for quick and easy access. The process of setting this up is similar to that of creating an external page on a dashboard.


First, you need to obtain a URL to the request queue. Secondly, you can embed the URL into a dashboard by adding an external page. 


## Access requirements {#access-requirements}

You must have the following access to perform the steps in this article:

<table style="width: 100%;margin-left: 0;margin-right: auto;mc-table-style: url('../../../Resources/TableStyles/TableStyle-List-options-in-steps.css');" class="TableStyle-TableStyle-List-options-in-steps" cellspacing="0"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2"> 
 <tbody> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader"><span class="mc-variable WFVariables.FullProdNameWF variable varname">Adobe Workfront</span> plan*</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p>Any</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader"><span class="mc-variable WFVariables.FullProdNameWF variable varname">Adobe Workfront</span> license*</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray"> <p><span class="mc-variable WFVariables.WFLicense-Plan variable varname">Plan</span> </p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader">Access level configurations*</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p>Edit access to&nbsp;Reports, Dashboards,&nbsp;Calendars</p> <p>Note: If you still don't have access, ask your <span class="mc-variable WFVariables.AdminWF variable varname">Workfront administrator</span> if they set additional restrictions in your access level. For information on how a <span class="mc-variable WFVariables.AdminWF variable varname">Workfront administrator</span> can change your access level, see <a href="create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-MediumGray" role="rowheader">Object permissions</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-MediumGray"> <p>Manage permissions to the dashboard</p> <p>For information on requesting additional access, see <a href="request-access.md" class="MCXref xref">Request access to objects in Adobe Workfront</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your *`Workfront administrator`*.


## Prerequisites {#prerequisites}

Both of the following must be created before you can embed a request queue in a dashboar:



*  **The dashboard**: For information on creating dashboards, see [Create a dashboard](create-dashboard.md).
*  **The request queue**: For information on creating request queues, see [Create a Request Queue](create-request-queue.md)




## Obtain the URL of the request queue {#obtain-the-url-of-the-request-queue}

You can obtain the URL of a request queue in multiple ways, depending on what portion of the request queue you want to expose to the users when they access it from a dashboard. 



*  [Obtain a link to a specific queue topic with ability to change the request type](#obtain2) 
*  [Obtain a link to a request queue and ability to change the request type](#obtain3) 
*  [Obtain a link to a request queue with no ability to change the request type](#obtain4) 




### Obtain a link to a specific queue topic with ability to change the request type {#obtain-a-link-to-a-specific-queue-topic-with-ability-to-change-the-request-type}

When you share a link to a specific queue topic with other users, the request form opens at the exact queue topic that they need to use to submit the request. This is helpful when users might not be sure which queue topic to choose when logging requests for a specific request queue. 


Users can change the request type or choose another topic if they need to. The navigation of the Requests area also displays. 



1.  Click the `Main Menu` > `Requests` >  `New Request`. 
1.  Continue selecting topic groups and queue topics until you reach the queue you want to share on the dashboard, if you want to share specific queue. For information about submitting requests, see [Create and submit Adobe Workfront requests](create-submit-requests.md). 


   >[!TIP] {type="tip"}
   >
   >Selecting topic groups and queue topics is optional. 



1.  
   Click  `Share path` in the upper-right corner of the New Request area. 


   This copies the link to the request queue or the queue topic as you display it on the screen. Users can update the Request Type or any of the topic groups and queue topics available. 


   ![](assets/share-request-queue-with-share-path-link-embedded-in-dashboard-nwe-350x116.png)






### Obtain a link to a request queue and ability to change the request type {#obtain-a-link-to-a-request-queue-and-ability-to-change-the-request-type}

When you share a link to a request type, the request type is selected for the user. This is helpful when users need to choose from multiple topic groups or queue topics for the same request type. Users can change the request type and choose another one. The navigation of the Requests area also displays. 



1.  Go to a project designated as a request queue. 


   For information about creating a request queue from a project, go to [Create a Request Queue](create-request-queue.md). 

1.  Go to `Queue Details`.
1.  Copy the code that you find in the `Direct Access URL` field.


   The code should look similar to the following:


   `<samp>https://<yourdomain>.my.workfront.com/requests/new?activeTab=tab-new-helpRequest&projectID=50062d6f000849c95ab3513c0e84a51e&path=</samp>` 


   This is the link to the request queue associated with the selected project.The Request Type is preselected. 


   Users can select any topic group or queue topic they need, or they can choose another request type. 


   ![](assets/share-request-queue-with-direct-url-embedded-in-dashboard-nwe-350x118.png)







### Obtain a link to a request queue with no ability to change the request type {#obtain-a-link-to-a-request-queue-with-no-ability-to-change-the-request-type}

When you share a link to a preselected request type, the request type is selected for the user and cannot be changed `<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver"> (it is dimmed)</MadCap:conditionalText>`. Users can choose the topic groups or queue topics they need. This is helpful when you do not want users to view and select other request types. The navigation of the Requests area does not display. 



1.  Go to a project designated as a request queue. 


   For information about creating a request queue from a project, go to [Create a Request Queue](create-request-queue.md). 

1.  Go to `Queue Details`.
1.  Copy the code that you find in the `Embedded Code` field.


   The code should look similar to the following:


   `<samp><iframe src="https://<yourdomain>my.workfront.com/requests/newRequestEmbedded?projectID=612518c7000404462d3bc9a0bc09fa71" frameborder="0" width="500" height="600"></iframe></samp>` 

1.  Edit the code to preserve only the information below: 


   `<samp>https://<yourdomain>.my.workfront.com/requests/newRequestEmbedded?projectID=612518c7000404462d3bc9a0bc09fa71</samp>` 


   >[!TIP] {type="tip"}
   >
   >You can preserve the `<samp>iframe </samp>`tag when embedding the code in an application other than  *`Workfront`*. 


   This is the link to the request queue associated with the selected project. The Request Type is preselected and cannot be changed. 


   Users can select any topic group or queue topic they need for the selected request type. Users cannot select another request type. 


   ![](assets/share-request-queue-with-embedded-code-embedded-in-dashboard-nwe-350x210.png)







## Embed a request queue in a dashboard {#embed-a-request-queue-in-a-dashboard-1}

You can embed a link to the requests queue or to a queue topic nested under a request queue into a dashboard to give users direct access to entering requests. 



1.  Obtain a request queue&nbsp;URL using one of the methods described in the [Obtain the URL of the request queue](#obtain) section of this article. 
1.  Click the `Main Menu` >  `Dashboards` > `New Dashboard`.
1.  Type a `Name` for the dashboard. This is a required field.
1.  Click `Add External Page`.


   ![](assets/add-external-page-highlighted---nwe-350x214.png)



1.  In the `Add External Page` box, edit the following fields: 

    
    
    *  `Name`: enter the name of the request queue as you want it to appear on the dashboard. This is a required field.
    
    

    
    
    * `Description`: enter a description about that this external page displays. This is not a required field and it is important only for reporting purposes. It does not display in the dashboard.&nbsp;
    * `URL`:`<MadCap:conditionalText data-mc-conditions="">  paste the URL you obtained using one of the methods described in Step 1.</MadCap:conditionalText>`
    
    * `Height`: enter the height of the external page. This defines how much space the external page containing the request queue occupies on the dashboard. This is a required field and the default value is 500.&nbsp;
    
    

1. Click `Save`. 
1.  Click `Save + Close`.&nbsp;


   The request queue displays in the dashboard as a separate dashboard component.&nbsp; 


   ![](assets/new-dashboard-with-embedded-request-queue-nwe-350x260.png)



1.  (Optional) Click `Dashboard Actions`, then `Edit` to add reports, calendars, or additional external pages to the same dashboard.  
   For information about adding components to a dashboard, see [Create a dashboard](create-dashboard.md).


&nbsp;


&nbsp;
