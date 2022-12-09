---
product-area: workfront-navigation
navigation-topic: workfront-navigation
title: Adobe Unified Experience for FAQ
description: A few features are different between Workfront and Adobe Experience Cloud, and you might have some questions as your Workfront instance is migrated to the unified experience.
author: Lisa
feature: Get Started with Workfront
exl-id: b9076fe0-26d7-4f33-80a4-564875ea13ba
---
# Adobe Unified Experience FAQ

The Adobe Unified Experience for Workfront allows you to manage all of your Adobe applications in one place with a single login. The Adobe navigation area is integrated seamlessly with Workfront. A few features are different, and you might have some questions as your Workfront instance is migrated to the unified experience.

For information about how to log in to the Adobe Unified Experience, see [Adobe Unified Experience for Workfront](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md).

## Comparison of Adobe Unified Experience and Workfront only experience

Only customers using the Adobe Business Platform / Adobe Admin Console can access the Adobe Unified Experience. Customers who have not yet migrated will see the Workfront only experience, without the ability to switch between Adobe applications.

This table describes some features that differ between the two experiences.

| Adobe Unified Experience | Workfront only experience |
| ---- | ----|
| Workfront Main Menu is on the left ![Main Menu](assets/main-menu-icon-left-nav.png) | Workfront Main Menu is on the right ![Main Menu](assets/main-menu-icon.png) |
| A single login URL is available for all Adobe Experience Cloud applications | Log in to Workfront with a custom Workfront URL |
| An "organization switcher" allows you to move between Workfront organizations and environments | The "organization switcher" is not available |
| Navigation includes a top level navigation area for Adobe products, Adobe notifications, help, and your user profile, in addition to the Workfront navigation bar | Navigation includes the Workfront navigation bar only |
| Help is accessible via the Main Menu and top navigation area | Help is accessible via the Main Menu and Workfront navigation bar |

{style="table-layout:auto"}

## Frequently asked questions

**How can I learn more about the Adobe Admin Console?**

For information about the Admin Console, review these articles:

* [Prepare for the Adobe Admin Console](/help/quicksilver/administration-and-setup/adobe-admin-console/prep-for-admin-console.md)
* [Platform-based administration differences (Adobe Workfront/Adobe Business Platform)](/help/quicksilver/administration-and-setup/get-started-wf-administration/actions-in-admin-console.md)
* [Adobe Admin Console overview](https://helpx.adobe.com/enterprise/using/admin-console.html)

**What do I as a customer need to do to facilitate the migration?**

Existing customers will be contacted to schedule migrations. The migration team support colleagues will walk customers through the process, advise on Admin Console setup, and provide links to documentation needed to make the move as simple and hassle-free as possible.

* [Adobe Workfront Support overview](https://experienceleague.adobe.com/docs/customer-one/using/workfront/overview.html)
* [Workfront Admin Console information](https://experienceleague.adobe.com/docs/customer-one/using/workfront/landing.html)
* [Adobe Business Platform and Admin Console FAQ](https://experienceleague.adobe.com/docs/customer-one/using/workfront/faq.html)

**How are you handling Adobe Admin Console for companies that already have this enabled for federated IDs differently than Workfront SSO is set up?**

Adobe Admin Console has the option to include Workfront, replacing SSO with IMS. All user provisioning happens in the Admin Console, and users will see the Adobe login screen to get to Experience Cloud where they will see Workfront as an option (if they are granted access to it).

**How does this impact customers that already have the AEM admin panel for Adobe Assets – but the SSO is configured differently than Workfront?**

Once Workfront is added as an Admin Console application, you should not have to do anything else for Workfront to leverage the existing SSO setup you have for Adobe Assets.

**How does this affect those that are set up with SSO?**

SSO is set up in the Admin Console and inherited by the Workfront application.

**Is SSO with our internal Active Directory going to be an option with IMS?**

IMS is a replacement for SSO and functions mostly the same. All user permissions are granted and provisioned in Adobe Admin Console, and the user will see the Adobe login screen where they can choose "Personal Account" or "Company Account" to log in (if you have Active Directory, most will log in with a company account).

**For those that are not using SSO, does the Workfront login URL change?**

The login URL will change; however, the old URL will redirect to the new login URL, so you should retrain your users where to go.

**Will aliases we have set up still work, or are the Workfront links changing with this migration?**

Workfront redirects/aliases are available to get to the homepage.

**Will there be a time when the redirects are disabled? Or will we always be able to type in my.company.workfront.com?**

You'll always be able to use any custom URLs. After you click any of those links, it will direct you to Workfront and show a different URL. However, it is a better experience to log in to experience.adobe.com, and bookmark links from within Experience Cloud. Less redirecting equals less lag time/loading time.

**Will direct links to request queues be broken?**

All direct links should redirect to the new URL patterns. However, if you have distributed links to people, you should send an update to leverage the direct link and prevent delays in getting to the expected page.

**Will we migrate to Experience Cloud globally or can we select for certain users (not all our users even use other Adobe products)?**

The entire Workfront customer account will be migrated. It cannot be done on a user-by-user basis.

**Will all Workfront users have to log in via Experience Cloud? Or just administrators?**

Yes, all users will log in via Experience Cloud. The IMS login will replace SSO. It's a very similar experience, just a different login screen.

**Will users have to link their Adobe accounts to their Workfront accounts if they already have both?**

Yes, there is a process for this, and more details will be provided when it's time for your organization to move to IMS.

**What happens to the Workfront users who don't have an Adobe account?**

Users who haven't been granted access in Adobe Admin Console to get into Workfront must create a "personal account" or an Adobe ID account to be able to log in. This sends an email to the administrator to approve or reject their request, and it additionally enables the admin to configure what type of access that user has. When they log in, they will go to experience.adobe.com, enter their email address, and choose Personal Account. From there, they will be able to access Workfront.

**What if we don't have any Adobe products other than Workfront?**

It is still recommended that your organization migrate to the Adobe Unified Experience. You will receive an Adobe ID along with the benefits listed above.

**We have external users included in our Workfront instance. We wouldn't want them to have access to any other products included in Adobe. How would we limit their access within the console?**

Admin Console gives admins a lot of control over what users can and cannot access. Whenever an external user wants access, they need to create an Adobe ID, which sends an email to the administrator. The administrator can then accept or reject access to a product and define what they can/cannot access for products owned by that organization. Then, the Workfront System Administrator can go into the Users area of Workfront to make any more granular permissions for the external user.

**Group Admins are used to create people in Workfront. With the move to Experience Cloud, will group admins still be able to create people?**

Yes, user creation is still possible through Workfront. Those users can be added to Experience Cloud automatically. You can also set up your group admins as product owners in the Admin Console to allow them to assign Workfront to users.

**What is the deadline to switch over to Experience Cloud?**

There is no deadline currently to move to Adobe Experience Cloud. We're working with customers to let them choose when they're ready to make the move.

**Will our support team need to do anything for this change?**

If the support team is responsible for creating new users, then they will need to become familiar with the Admin Console interfaces used to create users and assign an entitlement to Workfront. Otherwise, there is likely no significant change for your internal support team.

**How does this impact integrations we have through the API function?**

The existing URL path will continue to be available for API traffic. You should not need to do anything to update the endpoints in your integrations. However, direct login through username and password will not be supported – you must use an API key, with the exception being Workfront Fusion connectors.

**What about Creative Cloud users? How does the migration affect them? Are there any advantages for them?**

There is no impact to Creative Cloud users with the migration to Adobe Unified Experience.

**Will logins change for Workfront mobile users?**

Workfront mobile users should not be affected by the migration to Adobe Unified Experience.
