---
filename: wf-custom-refresh-sandbox-environment
user-type: administrator
content-type: overview;how-to-procedural
product-area: system-administration
navigation-topic: workfront-testing-environments
---



# The *`Adobe Workfront`* Custom Refresh Sandbox environment {#the-adobe-workfront-custom-refresh-sandbox-environment}

The Custom Refresh Sandbox is an environment where you can test and work using data from your production environment. It’s also ideal for running trainings and determining setup functionality.


>[!NOTE]
>
>This is different from the Preview Sandbox, which is also a testing environment that replicates your *`Workfront`* production environment.
>
>
>
>* New features are introduced to the Preview Sandbox before they become available in Production.
>*  New features are not introduced to the Custom Refresh Sandbox before they become available in Production.
>
>
>  Also, there is an additional cost to obtain the Custom Refresh Sandbox that is not required for the Preview Sandbox.
>
>
>  For more information about the Preview Sandbox, see [The Adobe Workfront Preview Sandbox Environment](wf-preview-sandbox-environment.md).
>
>
>





## Access requirements {#access-requirements}

You must have the following:

<table style="width: 100%;margin-left: 0;margin-right: auto;mc-table-style: url('../../../Resources/TableStyles/TableStyle-List-options-in-steps.css');" class="TableStyle-TableStyle-List-options-in-steps" cellspacing="0"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2"> 
 <tbody> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader"><span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span> plan</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p><span class="mc-variable WFVariables.WFPlan-Business variable varname">Business</span> or higher</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader"> <p role="rowheader"><span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span> license</p> </td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray"> <p><span class="mc-variable WFVariables.WFLicense-Plan variable varname">Plan</span> </p> <p>You must be a <span class="mc-variable WFVariables.AdminWF variable varname">Workfront administrator</span>. For information on <span class="mc-variable WFVariables.AdminWF-plur variable varname">Workfront administrators</span>, see <a href="grant-a-user-full-administrative-access.md" class="MCXref xref">Grant a user full administrative access</a>.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-LightGray" role="rowheader">Support package</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-LightGray"> <p>Plus, Preferred, or Enterprise</p> <p>The standard support package does not have access to the Custom Refresh Sandbox, but it does have access to the Preview Sandbox.</p> </td> 
  </tr> 
 </tbody> 
</table>



## Refreshing the Custom Refresh Sandbox {#refreshing-the-custom-refresh-sandbox}

The Custom Refresh Sandbox contains your actual production data, it does not refresh until you schedule it to do so. You can schedule a refresh any time is convenient for you, as frequently as once a week.


>[!NOTE]
>
>
>
>
>* You cannot schedule a refresh for the current day. For example, if today is June 1, the earliest day when you can schedule a refresh is June 2.
>* Your Custom Refresh Sandbox always has the same product features as your production environment. However, when you refresh your Custom Refresh Sandbox, it preserves branding only for the login screen background color. The login screen and navigation bar logos are reset to *`Workfront`* defaults, and any branding images you modified prior to the refresh do not display.
>
>





## Access the Custom Refresh Sandbox from your Production environment {#access-the-custom-refresh-sandbox-from-your-production-environment}

As a *`Workfront administrator`*, you can access your Custom Refresh Sandbox from your production environment.


>[!NOTE]
>
>If your account is on Cluster 4 (EMEA Cluster), you cannot access your Custom Refresh Sandbox from the Production Environment. For more information about how you can access your Custom Refresh Sandbox when you have an account on Cluster 4, see [Access the Custom Refresh Sandbox for Accounts on Cluster 4 (EMEA Accounts)](#custom-refresh-cluster-4) [Access the Custom Refresh Sandbox for Accounts on Cluster 4 (EMEA Accounts)](#custom-refresh-cluster-4).


To access your Custom Refresh Sandbox:



1. Click `Setup` near the upper-right corner of *`Adobe Workfront`* on the Global Navigation Bar.

1. Click `System` > `Preferences`.  

1.  In the `Test Environment` section, click `Sandbox 1` or `Sandbox 2`.


   Your support package specifies whether you have access to one or two Custom Refresh Sandboxes.

1.  Log in using your Custom Refresh Sandbox credentials.


   Your Custom Refresh Sandbox credentials are the same as your production credentials, unless you have changed your production credentials since you last refreshed your Custom Refresh Sandbox. The logins are synchronized only when a refresh occurs. They do not synchronize automatically.  



   The Custom Refresh Sandbox&nbsp;shows the version as well as the last refresh date in the banner at the top of the screen. All information from production is available and ready to work with after a&nbsp;refresh completes.





## Access the Custom Refresh Sandbox using a URL {#access-the-custom-refresh-sandbox-using-a-url}

Any user can access the Custom Refresh Sandbox by using a URL.



* [Access the Custom Refresh Sandbox for accounts on Clusters 1,2,3, and 5](#custom-refresh-1-2-3) 
* [Access the Custom Refresh Sandbox for Accounts on Cluster 4 (EMEA Accounts)](#custom-refresh-cluster-4) 




### `Access the Custom Refresh Sandbox for accounts on Clusters 1,2,3, and 5`  {#access-the-custom-refresh-sandbox-for-accounts-on-clusters-and}

Depending on your Support package, you should have access to one or two Custom Refresh Sandboxes. 


To access your Custom Refresh Sandbox using a URL: 



1.  Navigate to this URL if you only have one Custom Refresh Sandbox:


   https://companyname.sb01.workfront.com (old URL:https://cr1.attasksandbox.com/.)


   Or If you have two Custom Refresh Sandboxes, in addition to the URLs above, you can also Go to the following URL to access your second Custom Refresh Sandbox:


   https://companyname.sb02.workfront.com (old URL:https://cr2.attasksandbox.com/)

1. On the login screen, log in using your Custom Refresh Sandbox credentials.&nbsp;
1. Your Custom Refresh Sandbox credentials are the same as your production credentials, unless you have changed your production credentials since your Custom Refresh Sandbox was last refreshed. The logins are synchronized&nbsp;only when a refresh occurs. They do not synchronize automatically.




### `Access the Custom Refresh Sandbox for Accounts on Cluster 4 (EMEA Accounts)`  {#access-the-custom-refresh-sandbox-for-accounts-on-cluster-emea-accounts}

If your *`Workfront`* account is on Cluster 4 (EMEA cluster), you can access your Custom Refresh Sandbox only using a URL. To&nbsp;find out what cluster your account is on, contact our Customer Support team.&nbsp;


Depending on your Support package, you should have access to one or two Custom Refresh Sandboxes. 


To access your Custom Refresh Sandbox using a URL: 



1.  Navigate to this URL if you only have one Custom Refresh Sandbox:


   https://companyname.sb01.workfront.com (old URL:https://cr3.attasksandbox.com)


   Or


   Go to either one of these URLs if you have two Custom Refresh Sandboxes:


   https://companyname.sb01.workfront.com (old URL:https://cr3.attasksandbox.com)


   https://companyname.sb02.workfront.com (old URL:https://cr4.attasksandbox.com)

1.  On the login screen, log in using your Custom Refresh Sandbox credentials.   



   Your Custom Refresh Sandbox credentials are the same as your production credentials, unless you have changed your production credentials since your Custom Refresh Sandbox was last refreshed. The logins are synchronized&nbsp;only when a refresh occurs. They do not synchronize automatically.





## Schedule a refresh of your Custom Refresh Sandbox {#schedule-a-refresh-of-your-custom-refresh-sandbox}



>[!IMPORTANT] {type="important"}
>
>The duration of the refresh depends on the size of the data being refreshed. During the refresh process, it is critical that your custom refresh sandbox environment is not being used in any way (including API calls and integrations) as this will prevent the sandbox refresh from successfully finishing. *`Workfront`* will disable the custom refresh sandbox environment before it begins but you must end any active sessions to ensure that your sandbox refresh is successful.


After you schedule a refresh of your Custom Refresh Sandbox, you can cancel it by clicking Cancel at the top of the page. You can also reschedule it for a later time.  


>[!NOTE]
>
>You cannot schedule automatic sandbox refreshes.





To schedule a refresh of your Customer Refresh Sandbox: 



1. Log in to your Custom Refresh Sandbox.
1. Click `Schedule`in the banner at the top of the screen and select a date from the calendar.
1. Select a date for when you want the refresh to happen, then click `Schedule Refresh`.  





## Switch to Production from the Custom Refresh Sandbox {#switch-to-production-from-the-custom-refresh-sandbox}




1.  Log in to your Custom Refresh Sandbox. 


   For more information about accessing your Custom Refresh Sandbox, see [Access the Custom Refresh Sandbox from your Production environment](#accessing-your-custom-refresh-from-production) or [Access the Custom Refresh Sandbox using a URL](#accessing-your-custom-refresh-sandbox-using-a-url).

1.  Click `Go To Production` in the banner at the top of the screen.


   Remember that work done in the sandbox will not be visible in the production environment, as the transfer of data is unidirectional, from production to your Custom Refresh Sandbox,&nbsp;and not in reverse.





## Receive emails from the Custom Refresh Sandbox {#receive-emails-from-the-custom-refresh-sandbox}

*`Workfront`* disables all email communication from the Custom Refresh&nbsp;Sandbox environment. If you want to receive email notifications from the Custom Refresh Sandbox environment, you must enable this functionality in your user settings. For more information about enabling email notifications in the Custom Refresh Sandbox environment, see [Enable delivery of emails from the Preview Sandbox environment](enable-delivery-emails-from-preview-sandbox-environment.md).




>[!NOTE]
>
>Report delivery and push notifications on the mobile app are always disabled for the Custom Refresh Sandbox environment. Neither you nor the *`Workfront administrator`* can enable report delivery or push notifications for the mobile app when you access the Custom Refresh&nbsp;Sandbox environment.  
>For more information about report deliveries for the production environment, see [Report delivery overview](set-up-report-deliveries.md).For more information about push notifications on the mobile app for the production environment, see the section in .  






## Configure Single Sign-On in the Custom Refresh Sandbox {#configure-single-sign-on-in-the-custom-refresh-sandbox}

If you want to configure your Custom Refresh Sandbox to work with a Single Sign-On solution, you can do so by configuring it separately from your Production environment. The SSO configuration in the Custom Refresh Sandbox is independent from your SSO configuration in the Production environment.  
When you refresh your Custom Refresh Sandbox, the SSO information is not copied from your Production environment to overwrite the Custom Refresh Sandbox configuration.


The steps for configuring single sign-on in the Custom Refresh Sandbox are similar to those for configuring it in the Production environment.  
For more information about configuring *`Workfront`* with SSO, see [Overview of single sign-on in Adobe Workfront](sso-in-workfront.md).


## Intended use and availability {#intended-use-and-availability}

*`Workfront`* Custom Refresh Sandbox environments are not intended for performance or load testing. Rather, use these environments to validate feature functionality with your organization's existing workflows.


*`Workfront`* Custom Refresh Sandbox environments are intended to be always available. Any outage to a *`Workfront`* Custom Refresh Sandbox environment during regular business hours will be a first priority immediately after any Production issues are resolved if any exist. Any outage to a *`Workfront`* Custom Refresh Sandbox environment on weekends (Saturdays and Sundays) will be addressed so that the environment is running for business hours on Monday.
