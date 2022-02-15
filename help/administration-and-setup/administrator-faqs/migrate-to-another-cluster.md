---
filename: migrate-to-another-cluster
title: Migrate to another cluster
user-type: administrator
content-type: faq
product-area: system-administration
navigation-topic: administrator-faqs
---




# Migrate to another cluster {#migrate-to-another-cluster}

When we are migrating your `Workfront` environment to a new cluster, consult this document to answer some of the frequently asked questions about this process. 


## How do I request a migration to another cluster? {#how-do-i-request-a-migration-to-another-cluster}

`Workfront` established very specific business reasons for which you can request your environment to be migrated to another cluster. Contact your Account Representative to see if you qualify for a migration. 


## What should I know about migrating to a new cluster? {#what-should-i-know-about-migrating-to-a-new-cluster}




*  During the migration, your production environment will be inaccessible for up to 60 minutes. 
*  If you have API integrations, you may have to regenerate the API key and update it in your API integrations.   
  Any API integrations may not work after the migration without this step completed. For more information about resetting the API key in `Workfront`, see the section in 





## What should I do to prepare for the migration? {#what-should-i-do-to-prepare-for-the-migration}




*   We recommend that your company's firewall is configured in a way that allows for `Workfront` to access your environment.


  If your company needs to allow specific IP addresses on your firewall configuration, ensure that the IP addresses we recommend to be accessible through your firewall are added to the allowlist in order to continue successfully using the following features after the migration: 

*  `<li value="1"> emails, including POP emails </li>` `<li value="2"> SSO </li>` `<li value="3"> <p> Document Webhooks </p> <p> For a complete list of IP addresses that need to be added to the allowlist, see <a href="configure-your-firewall.md" class="MCXref xref" xrefformat="{para}">Configure your firewall</a>.</p> </li>` 





>[!NOTE]
>
>Ensure that all `Workfront administrator`s can log in to `Workfront` using their `Workfront` credentials (not their SSO credentials). Your SSO login should work after the migration, but this will ensure that at least the `Workfront administrator`s can log in, should the SSO configuration need to be reset. 





*  We recommend that you designate someone in your company to test important workflows in `Workfront` to make sure they are working correctly after the migration. 
*  Notify your users that there will be a disruption in service to ensure everyone is logged out of your environment before the migration occurs. Any users logged in during the migration will be automatically logged out. 




## How do I log in after the migration? {#how-do-i-log-in-after-the-migration}




*  Use your existing URL for your Production environment to log in after the migration has completed: *https://[Domain].my.workfront.com* . Replace [Domain] with your `Workfront` domain name. 

*  If your `Workfront` instance has been integrated with SSO, log in with your SSO credentials. If this fails and you are a `Workfront administrator`, log in with your `Workfront` credentials and test your SSO configuration. If this is not working (this is very rare), contact our Support Team. 





## What areas of functionality should I include in my testing, after the migration completes? {#what-areas-of-functionality-should-i-include-in-my-testing-after-the-migration-completes}




*  Your Production environment should be accessible after the migration. If you cannot access your Production environment, contact our Support Team. 
*  Ensure that your branding customizations are in place. 
*  Ensure that your users are able to log in. 
*  Test all important workflows. We recommend that you should test the following: 
*  `<li value="1"> All day-to-day workflows for your company, including reports and dashboards </li>` `<li value="2"> Email communication from <span class="WFVariablesProdNameWF">Workfront</span> (which includes event notifications, reminder notifications, automatic reminders, if they are enabled). </li>` `<li value="3"> Any API integrations, if you have any. </li>` 

*  Search functionality will take some time to work properly. You should expect full search capabilities within a few hours of the migration. 
*  If you find any abnormalities in your data after 24 hours from when the maintenance window closed, contact our Support Team. 
*  You will need to manage your subscriptions to notifications you might be receiving from our [Trust Site](https://trust.workfront.com/) to ensure you subscribe to your new cluster notifications. 




## What about my sandbox environments? {#what-about-my-sandbox-environments}




*  Your Preview environment will be available the Sunday following the migration.  
  The URL for the Preview environment will be the same: *https://[Domain].preview.workfront.com* . Replace [Domain] with your `Workfront` domain name. 

*  Your Custom Refresh Sandbox will be reset during the migration and will be unavailable for 1-5 days while your data is fully synchronized. Any customization, configurations, or other testing currently in your Custom Refresh Sandbox will be overwritten with a current copy of your production data.  
  The URL for the Custom Refresh Sandbox will be the same: *https://[Domain].sb01.workfront.com* . Replace [Domain] with your `Workfront` domain name. 





## How do I get help if I have more questions? {#how-do-i-get-help-if-i-have-more-questions}




*  You can contact our Support Team, the same way you would normally contact them and open a ticket.  
  For more information about how you can open a Support ticket, see&nbsp; [Contact Customer Support](contact-customer-support.md).&nbsp;



