---
filename: firewall-overview
user-type: administrator
content-type: overview
product-area: system-administration;user-management
navigation-topic: start-with-workfront-administration
---



# Firewall overview {#firewall-overview}

Because *`Adobe Workfront`* communicates with your organization's network, your organization's firewall must be configured to allow that communication. Firewalls are highly effective security measures that function by separating an organization's network from the internet. They ensure that only selected data and network traffic can move into or out of the organization's network. The firewall allows or blocks data based on the site that is sending or receiving the data. As an *`Adobe Workfront administrator`*, you must ensure that data sent to or from *`Workfront`* can pass through your organization's firewall.


This is accomplished through an allowlist, which is essentially a "list" of sites that are "allowed" to send or receive data through the firewall. Sites can be identified in one of two ways:



*  **IP address**: a series of numbers such as 52.31.132.175
*  **Domain**: part of a URL, such as "thisdomain" in www.thisdomain.com


*`Workfront`* uses specific IP addresses and domains for web communication. These must be added to your organization's allowlist before you can use *`Workfront`* in your organization.


Generally, an allowlist is configured by a network administrator. Work with your organization's network administrator to ensure that your firewall allows these IP addresses. If you do not know who your network administrator is, your organization's IT department can point you in the right direction.


>[!IMPORTANT] {type="important"}
>
>As a *`Workfront administrator`*, you must ensure that these IP addresses and domains are added to your organization's allowlist. This is true even if you do not add them yourself. *`Workfront`* cannot configure your organization's allowlist.




## Collect information for configuring your firewall {#collect-information-for-configuring-your-firewall}

To configure your firewall for *`Workfront`*, your network administrator needs to know which IP addresses and domains to add. Some of this information is available only to a *`Workfront`* administrator. As the Workfront administrator, you must locate this information and provide it to your network administrator.


>[!NOTE]
>
>The best practice for security is to add only the IP addresses and domains that connect to functionality your organization is actively using. By providing this information, you can ensure that this best practice is followed.


Provide your network administrator with the following information:

<table style="width: 100%;mc-table-style: url('../../Resources/TableStyles/TableStyle-List-options-in-steps.css');" class="TableStyle-TableStyle-List-options-in-steps" cellspacing="0"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2"> 
 <tbody> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader">Specific IP addresses and domains to allow</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p>The article <a href="configure-your-firewall.md" class="MCXref xref">Configure your firewall</a> contains the list of IP addresses and domains that your organization must add to its allowlist. </p> <p>Your network administrator might not have access to the "Configure your firewall" article. In that case, you must provide it to them. We do not recommend printing a hard (paper) copy. A digital copy allows your network administrator to copy and paste the addresses, which is quicker and more accurate than typing from a hard copy.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader">Your cluster</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray">To locate your organization's cluster, see <a href="#locate" class="MCXref xref">View your organization's cluster and Workfront plan</a></td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader">Your <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span> Plan</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p>Your organization's plan is one of the following:</p> 
    <ul> 
     <li> <p><span class="mc-variable WFVariables.WFPlan-Enterprise variable varname">Enterprise</span> </p> </li> 
     <li> <p><span class="mc-variable WFVariables.WFPlan-Business variable varname">Business</span> </p> </li> 
     <li> <p><span class="mc-variable WFVariables.WFPlan-Pro variable varname">Pro</span> </p> </li> 
     <li> <p><span class="mc-variable WFVariables.WFPlan-Team variable varname">Team</span> </p> </li> 
    </ul> <p>To locate your plan, see <a href="#locate" class="MCXref xref">View your organization's cluster and Workfront plan</a></p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader">Your domain</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray"> <p>To locate your domain, look at the web address that you use to connect to <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span>.</p> <p>Example: in the web address <code>greatcompany.my.workfront.com</code>, the domain is "greatcompany"</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader">Other Adobe Workfront products</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p>Inform your network administrator if you have licenses for either of the following:</p> 
    <ul> 
     <li> <p><span class="mc-variable WFVariables.FullProdNameWF variable varname">Adobe Workfront</span> <span class="mc-variable WFVariables.Proof-UC-n variable varname">Proof</span></p> </li> 
     <li> <p><span class="mc-variable WFVariables.FullProdNameWFF variable varname">Adobe Workfront Fusion</span> </p> </li> 
    </ul> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader">Adobe Workfront integrations</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray">Inform your network administrator if you use any of the following:
    <ul>
     <li><p><p><span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span> for Jira</p></p></li>
     <li><p><span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span> for G Suite</p></li>
     <li><p><span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span> for Microsoft Teams</p></li>
     <li><p><span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span> for Outlook</p></li>
     <li><p><span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span> for Salesforce</p></li>
    </ul></td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-LightGray" role="rowheader">Additional Functionality</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-LightGray"> <p>Inform your network administrator if you use either of the following:</p> 
    <ul> 
     <li> <p>A <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span> test drive</p> </li> 
     <li> <p><span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span> Ascent</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>



>[!IMPORTANT] {type="important"}
>
>If you add any of these products, integrations, or functionalities at a later date, you must contact your network administrator so they can adjust the allowlist.




### View your organization's cluster and *`Workfront`* plan {#view-your-organizations-cluster-and-workfront-plan}




1. Click the `Main Menu` icon ![](assets/main-menu-icon.png) in the upper-right corner of *`Adobe Workfront`*, then click `Setup` ![](assets/gear-icon-settings.png).

1. Click **System** in the left panel
1.  To view your cluster, Select **Customer Info**. 


   Your cluster displays near the upper-right of the **Basic Info** section.


   ![](assets/locate-cluster-350x189.png)



1.  To view your *`Workfront`* plan, select **Licenses**.


   Your plan displays near the bottom of the page.


   ![](assets/locate-plan-350x162.png)





