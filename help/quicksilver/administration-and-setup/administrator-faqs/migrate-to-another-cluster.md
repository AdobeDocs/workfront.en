---
filename: migrate-to-another-cluster
title: Migrate to another cluster
user-type: administrator
content-type: faq
product-area: system-administration
navigation-topic: administrator-faqs
title: Migrating to another cluster
description: When we are migrating your Adobe Workfront environment to a new cluster, consult this document to answer some of the frequently asked questions about this process.
hidefromtoc: true
---

# Migrating to another cluster

When we are migrating your Adobe Workfront environment to a new cluster, consult this document to answer some of the frequently asked questions about this process.

## How do I request a migration to another cluster?

Workfront established very specific business reasons for which you can request your environment to be migrated to another cluster. Contact your Account Representative to see if you qualify for a migration.

## What should I know about migrating to a new cluster?

* During the migration, your production environment will be inaccessible for up to 60 minutes. 
* If you have API integrations, you may have to regenerate the API key and update it in your API integrations.   
  Any API integrations may not work after the migration without this step completed. For more information about resetting the API key in Workfront, see the section in

## What should I do to prepare for the migration?

* We recommend that your company's firewall is configured in a way that allows for Workfront to access your environment.

  If your company needs to allow specific IP addresses on your firewall configuration, ensure that the IP addresses we recommend to be accessible through your firewall are added to the allowlist in order to continue successfully using the following features after the migration:

  * emails, including POP emails 
  * SSO 
  * Document Webhooks

    For a complete list of IP addresses that need to be added to the allowlist, see [Configure your firewall's allowlist](../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).

>[!NOTE]
>
>If your organization’s Workfront instance uses SSO, ensure that all Workfront administrators can log in to Workfront using their Workfront credentials (not their SSO credentials). Your SSO login should work after the migration, but this will ensure that at least the Workfront administrators can log in, should the SSO configuration need to be reset.

* We recommend that you designate someone in your company to test important workflows in Workfront to make sure they are working correctly after the migration. 
* Notify your users that there will be a disruption in service to ensure everyone is logged out of your environment before the migration occurs. Any users logged in during the migration will be automatically logged out.

## How do I log in after the migration?

* Use your existing URL for your Production environment to log in after the migration has completed: *https://[Domain].my.workfront.com* . Replace [Domain] with your Workfront domain name. 
* If your Workfront instance has been integrated with SSO, log in with your SSO credentials. If this fails and you are a Workfront administrator, log in with your Workfront credentials and test your SSO configuration. If this is not working (this is very rare), contact our Support Team.

## What areas of functionality should I include in my testing, after the migration completes?

* Your Production environment should be accessible after the migration. If you cannot access your Production environment, contact our Support Team. 
* Ensure that your branding customizations are in place. 
* Ensure that your users are able to log in. 
* Test all important workflows. We recommend that you should test the following:

  * All day-to-day workflows for your company, including reports and dashboards 
  * Email communication from Workfront (which includes event notifications, reminder notifications, automatic reminders, if they are enabled). 
  * Any API integrations, if you have any.

* Search functionality will take some time to work properly. You should expect full search capabilities within a few hours of the migration. 
* If you find any abnormalities in your data after 24 hours from when the maintenance window closed, contact our Support Team. Documents not stored in S3 typically take the longest to sync. 
* You will need to manage your subscriptions to notifications you might be receiving from the [Workfront Status site](https://status.workfront.com/) to ensure you subscribe to your new cluster notifications.

## What about my sandbox environments?

* Your Preview environment will be available the Sunday following the migration.  
  The URL for the Preview environment will be the same: *https://[Domain].preview.workfront.com* . Replace [Domain] with your Workfront domain name. 

* Your Custom Refresh Sandbox will be reset during the migration and will be unavailable for 1-5 days while your data is fully synchronized. This delay is due to the fact that a new sandbox must be provisioned for you. Any customization, configurations, or other testing currently in your Custom Refresh Sandbox will be overwritten with a current copy of your production data.  
  The URL for the Custom Refresh Sandbox will be the same: *https://[Domain].sb01.workfront.com* . Replace [Domain] with your Workfront domain name.

## If we have more than one instance of Workfront, do they need to be migrated at the same time?

If you have more than one instance of Workfront, each with a different URL (for example, xxxx.my.workfront.com), they do not need to be migrated at the same time.

## Is there a roll-back plan if there's an issue with the migration?

In the extremely rare case that an issue would arise to require a roll-back, your data would be synchronized back to the old cluster.

## How can I ensure all my data is successfully migrated?

No data has been lost in the many hundreds of customer migrations completed thus far. If you are still concerned, you could write API calls to validate your data to your satisfaction.

## How do I get help if I have more questions?

* You can contact our Support Team, the same way you would normally contact them and open a ticket.  
  For more information about how you can open a Support ticket, see [Contact Customer Support](../../workfront-basics/tips-tricks-and-troubleshooting/contact-customer-support.md).

