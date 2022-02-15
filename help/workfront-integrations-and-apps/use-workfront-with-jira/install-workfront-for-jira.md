---
filename: install-workfront-for-jira
product-area: workfront-integrations;setup
navigation-topic: workfront-for-jira
---



# Install *`Adobe Workfront`* for Jira {#install-adobe-workfront-for-jira}

You can use *`Adobe Workfront`* for Jira to integrate your Jira and *`Workfront`* systems.


After installing the add-on, you can define workflows that create Jira issues automatically when *`Workfront`* work items are created. The items in both applications become linked, and some of their information can be automatically updated in both systems.&nbsp;


All users in *`Workfront`* and Jira can benefit from this integration. They only need a license for the system in which they work the most, and not for both systems.&nbsp;


This add-on is available for the Server, Data Center, and OnDemand (or Cloud) versions of Jira Software.


For a list of Jira versions that *`Workfront for Jira`* currently supports, see [ *`Workfront for Jira`*](https://marketplace.atlassian.com/apps/1218653/workfront-for-jira?hosting=cloud&tab=overview) at the Atlassian Marketplace.


## Access requirements {#access-requirements}

You must have the following:

<table style="width: 100%;margin-left: 0;margin-right: auto;mc-table-style: url('../../Resources/TableStyles/TableStyle-List-options-in-steps.css');" class="TableStyle-TableStyle-List-options-in-steps" cellspacing="0"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2"> 
 <tbody> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader"><a href="https://www.workfront.com/plans" target="_blank"><span class="mc-variable WFVariables.FullProdNameWF variable varname">Adobe Workfront</span> plan</a>*</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p>Pro or higher</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader"><a href="wf-licenses.md" class="MCXref xref">Adobe Workfront licenses overview</a>*</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray"> <p>Plan</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader">Jira access</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p>System administrator access</p> <p>Important:  We recommend that you create separate system administrator accounts in Jira and <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span> to dedicate to this integration, rather than using existing ones that might be attached to users.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-MediumGray" role="rowheader">Access level configurations*</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-MediumGray"> <p>You must be a <span class="mc-variable WFVariables.AdminWF variable varname">Workfront administrator</span>. For information on <span class="mc-variable WFVariables.AdminWF-plur variable varname">Workfront administrators</span>, see <a href="grant-a-user-full-administrative-access.md" class="MCXref xref">Grant a user full administrative access</a>.</p> <p>Note: If you still don't have access, ask your <span class="mc-variable WFVariables.AdminWF variable varname">Workfront administrator</span> if they set additional restrictions in your access level. For information on how a <span class="mc-variable WFVariables.AdminWF variable varname">Workfront administrator</span> can modify your access level, see <a href="create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your *`Workfront administrator`*.


## Install *`Workfront`* for Jira {#install-workfront-for-jira}

Installing *`Workfront`* for Jira OnDemand is identical to installing it on a Jira Server instance.


You must be a Jira administrator to install the *`Workfront`* add-on. 


If you are not a Jira administrator, you can browse for the *`Workfront`* add-on and request it to be installed. Your request is sent to the Jira administrator for approval and installation.


For more information about requesting an add-on to be installed on your Jira application, see [Managing user requests for add-ons.](https://confluence.atlassian.com/upm/managing-user-requests-for-add-ons-781394968.html)


To install *`Workfront`* for Jira:



1. Log in to Jira as a Jira administrator.
1. Find the ` *`Workfront`* for Jira`&nbsp;add-on in the [Atlassian Marketplace](https://marketplace.atlassian.com/apps/1218653/workfront-for-jira?hosting=cloud&tab=overview).

1.  Click `Get it now` to install it.  



   After the installation completes, you can log in to *`Workfront`* from Jira and configure your integration.


   For more information, see [Configure Adobe Workfront for Jira](configure-workfront-for-jira.md).





## Considerations for a Jira Server or Jira Data Center installation {#considerations-for-a-jira-server-or-jira-data-center-installation}



>[!NOTE]
>
>These requirements do not apply to the OnDemand (Cloud) version of Jira Software.


Although installing the *`Workfront`* add-on in the two Jira environments is similar, you must consider the following when working with a Jira Server installation: 



* When configuring the add-on in Jira, the address specified in the  `JIRA Base URL` field may not be the same URL you use to access Jira on your private server. The `JIRA Base URL` must be a publicly-accessible address connected to your private server using NAT or reverse proxy protocols, so *`Workfront`* can access it to make requests to your server.&nbsp;&nbsp;

*  You must use SSL encryption to secure the communication between JIRA and *`Workfront`*. When you enable SSL, you must have a full SSL certificate stack from a certificate authority. We do not support self-signed certificates.&nbsp; 
*  You must ensure that the jira.workfront.com domain is accessible from your corporate servers. It serves as a middleware environment between *`Workfront`* and Jira and is required for the add-on to operate.


  You must also add the following static IP addresses to the allowlist on your firewall for outbound and inbound connections.

    
    
    *      
    
      ```    
      35.162.128.73
      ```    
    

    *      
    
      ```    
      34.213.36.118
      ```    
    

    *  <![CDATA[ ]]>    
    
      ```    
      35.160.0.242
      ```    
    

    *      
    
      ```    
      3.209.27.146
      ```    
    

    *      
    
      ```    
      18.205.251.4
      ```    
    

    
    
  For more information about configuring your firewall for optimal functionality with *`Workfront`*, see [Configuring Your Firewall](configure-your-firewall.md).



