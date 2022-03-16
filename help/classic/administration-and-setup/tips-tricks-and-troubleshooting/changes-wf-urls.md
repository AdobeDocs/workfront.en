---
filename: changes-wf-urls
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: Changes to Adobe Workfront URLs
description: In an effort to update our platform to match our new brand and streamline the way our customers access their Adobe Workfront systems, we added simplified URLs for all customers to access their Workfront instances.
---

# Changes to Adobe Workfront URLs

In an effort to update our platform to match our new brand and streamline the way our customers access their Adobe Workfront systems, we added simplified URLs for all customers to access their Workfront instances.

AtTask became Workfront in 2015. All customers’ system access URLs (usually&nbsp;*domain*.attask-ondemand.com) must be updated to match our current name and brand. You should be accessing Workfront via the URL:&nbsp; *domain*.my.workfront.com .&nbsp;

>[!NOTE]
>
>For a time, both the old and new URLs were active in order to make your transition smooth. The old access URLs were replaced on May 15, 2019.&nbsp;

If you&nbsp;use a SAML SSO solution to help your&nbsp;users access Workfront, you should have completed additional steps to ensure your&nbsp;custom metadata is retained during the transition. If you use&nbsp;the Workfront APIs, you should have updated them with the new access URLs to avoid service interruptions when the final transition was made in May 2019. For more information about updating SAML 2.0 metadata, see [Update SAML 2.0 metadata in your identity provider](../../administration-and-setup/add-users/single-sign-on/update-saml-2-metadata-ip.md).

You and your teams should be using the new URLs to access Workfront.<![CDATA[    ]]>

>[!NOTE]
>
>All emails are linked to&nbsp;*yourdomain.my.workfront.com*. When you click on any link inside an email notification, you must log in a second time if you are logged in to&nbsp; *yourdomain.attask-ondemand.com*.

The Custom Preview sandbox URLs we also updated. The Sandbox URLs transitioned from&nbsp;*domain*.cr1.attasksandbox.com,&nbsp;*domain*.cr2.attasksandbox.com, etc., to&nbsp; *domain*.sb01.workfront.com ,&nbsp; *domain*.sb02.workfront.com , etc.

Summary of URL changes:

* *domain*.attask-ondemand.com

`is now…`

*domain*.my.workfront.com

* *domain*.cr1.attasksandbox.com&nbsp;and&nbsp;*domain*.cr2.attasksandbox.com

`is now…`

*domain*.sb01.workfront.com&nbsp; and&nbsp;*domain*.sb02.workfront.com

As always, if you have any issues or questions about this change, please feel free to contact Workfront Support.

<!--
Phases and Timeframe of Changes Phase 1, Automatic Redirect (May 15 - June 12, 2019, depending on cluster) Users who access the *.attask-ondemand.com are automatically redirected to the *.my.workfront.com domain. Schedule by cluster Cluster 1 - May 29 Cluster 2 - June 5 Cluster 3 - May 22 Cluster 4 - May 15 Cluster 5 - June 12 Cluster 6 - May 22 Phase 2, Information Page with Link (July 17, 2019 for all clusters) Users who access the *.attask-ondemand.com domain see an information page explaining this change and contains a link to the *.my.workfront.com domain. Phase 3, Removed Access to the Old URL (August 21, 2019 for all clusters) Users who access the *.attask-ondemand.com domain see a "site has moved" page and explains that the site is now accessed by the my.workfront.com domain.
-->

## Updating SSO Custom Metadata

If you use a SAML SSO solution to help your users access Workfront, you should have completed additional steps to ensure your custom metadata was retained. If you use the Workfront APIs, you should have updated them with the new access URLs to avoid service interruptions when the final transition was made on May 15, 2019. For more information about updating SAML 2.0 metadata, see [Update SAML 2.0 metadata in your identity provider](../../administration-and-setup/add-users/single-sign-on/update-saml-2-metadata-ip.md).
