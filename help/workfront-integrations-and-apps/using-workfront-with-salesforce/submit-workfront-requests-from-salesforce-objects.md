---
filename: submit-workfront-requests-from-salesforce-objects
product-area: workfront-integrations
navigation-topic: workfront-for-salesforce
---



# Submit *`Adobe Workfront`* requests from Salesforce objects  {#submit-adobe-workfront-requests-from-salesforce-objects}

After installing *`Adobe Workfront`* for Salesforce, you can submit *`Workfront`* requests from Salesforce Opportunities and Accounts. This functionality exists in both the Classic and Lightning Experience frameworks.


## Access requirements {#access-requirements}

You must have the following access to use the functionality described in this article:

<table style="width: 100%;margin-left: 0;margin-right: auto;mc-table-style: url('../../Resources/TableStyles/TableStyle-List-options-in-steps.css');" class="TableStyle-TableStyle-List-options-in-steps" cellspacing="0"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2"> 
 <tbody> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader"><span class="mc-variable WFVariables.FullProdNameWF variable varname">Adobe Workfront</span> plan*</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p>Pro or higher</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-MediumGray" role="rowheader"><span class="mc-variable WFVariables.FullProdNameWF variable varname">Adobe Workfront</span> license*</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-MediumGray"> <p>Plan</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your *`Workfront administrator`*.


## Prerequisites {#prerequisites}

To submit a *`Workfront`* request from a Salesforce Opportunity or Account ensure that you have the following in your environment:



*  Your *`Workfront administrator`* has installed *`Workfront`* for Salesforce.  
  For more information about installing *`Workfront`* for Salesforce, see [Install Adobe Workfront for Salesforce](install-workfront-for-salesforce.md)

*  Your *`Workfront administrator`* has added the *`Workfront`* section to your Opportunity and Account page layouts.  
  For more information about adding the *`Workfront`* section to a page layout, see [Configure the Adobe Workfront section for Salesforce users](configure-wf-section-for-salesforce-users.md).

*  You have a *`Workfront`* account and you can log in to it from the *`Workfront`* section inside your Opportunity or Account.   
  Once you log in, you can see the New Requests tab where you can start entering requests.




## Submit *`Workfront`* requests from Salesforce {#submit-workfront-requests-from-salesforce}




1.  Go to an Opportunity or Account in Salesforce. 
1. Go to the *`Workfront`* section.
1.  In the `New Requests` tab, select a request type in the `Select a Request Type` drop-down menu.  



   You can see the same request queues that you have access to see in *`Workfront`*.&nbsp;

1.  Start filling out the available fields for your request.  



   Submitting a request from Salesforce is identical to submitting a request in the *`Workfront`* web application.


   Continue to follow the steps described in [Create and submit Adobe Workfront requests](create-submit-requests.md).

1. Click `Submit`.




## View *`Workfront`* requests {#view-workfront-requests}




1. Go to an Opportunity or Account in Salesforce.
1.  Go to the ` *`Workfront`*` section.


   >[!NOTE]
   >
   >Depending on how your *`Workfront administrator`* configured this section, it might have a different name.



1.  Select the `Submitted Requests` tab.  



   You can view all the requests that you or others have submitted from this Opportunity or Account in this tab.Requests that are submitted to this request queue in the web application do not display in this list in Salesforce.


   >[!NOTE]
   >
   >Requests that are submitted to this request queue in the web application do not display in this list in Salesforce.


   ![salesforce_submitted_requests.png](assets/salesforce-submitted-requests-350x58.png)




   You can view the following information about the submitted requests:

    
    
    * Requests Name (in the Subject&nbsp;column)
    * Reference Number
    * Request&nbsp;Type
    * Status
    * Submitted on&nbsp;Date
    * Requested by Name
    * Assigned to Name  
      When this information is updated in *`Workfront`*, it is also updated in this list.&nbsp;
    
    
    

1.  (Optional) Click the name of the request to open it in *`Workfront`*.&nbsp;


   On the Summary panel ![](assets/summary-panel-icon.png), notice the `Integrations` indicator that signifies that this issue originated in Salesforce and is currently linked to an item there.&nbsp;

1.  (Optional) Click `Go to Salesforce` to access the Opportunity or Account where the issue originated.


   >[!NOTE]
   >
   >The Go to Salesforce link is visible to all *`Workfront`* users who can view the issue. You must have a Salesforce account to be able to go to the Salesforce Opportunity or Account where the issue was logged.&nbsp;





