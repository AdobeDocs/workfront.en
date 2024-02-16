---
product-previous: mobile
content-type: release-notes
navigation-topic: 2019-3-release-activity
title: 2019.3 Integration and mobile enhancements
description: This page describes all changes integration and mobile enhancements made with the 2019.3 release. It was be made available in the Production environment the week of August 19, 2019.
author: Luke
feature: Product Announcements, Workfront Integrations and Apps
recommendations: noDisplay, noCatalog
exl-id: 15e03405-63ff-48ea-b873-cf44f1f46282
---
# 2019.3 Integration and mobile enhancements

This page describes all changes integration and mobile enhancements made with the 2019.3 release. It was be made available in the Production environment the week of August 19, 2019.

For a list of all changes made in 2019.3, see [2019.3 release activity overview](../../../../product-announcements/product-releases/quarterly-release-archive/2019.3-release-activity/2019-3-release-activity-overview.md).

## Support of shared items in the MS OneDrive integration

Now you can link your shared OneDrive files and folders to Workfront objects. Conversely, you can upload files in Workfront to shared folders in OneDrive.

For more information, see the sections [Link an external document to Workfront](../../../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md#linking-existing-documents), [Link one or more external folders](../../../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md#linking-a-folder), and [Update and link a document from Workfront to an external cloud provider](../../../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md#sending-documents) in the article [Link documents from external applications](../../../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md).

For information, see the section [Link an external document to Workfront](../../../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md#linking-existing-documents) in the article [Link documents from external applications](../../../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md).

## Domain specification required for all Workfront logins

All Workfront logins now require the user to specify the domain if the domain is not already specified in the Workfront URL. Requiring this information makes your Workfront instance more secure. In addition, if your implementation of Workfront has multiple instances, this enhancement allows you to add the same user to each instance of Workfront within your implementation.

This change can affect both user logins and API&nbsp;integrations:

* **User logins**

  If your company domain is not included in the Workfront URL, you now see a new Domain field on the login screen in addition to the Username and Password fields.

  For most customers, no change is required because the domain information is already included in the Workfront URL. For example, "*domain*.my.workfront.com."

* **API integrations**

  If you have any API code going to an address that does not include your domain name, that API code will no longer work.

For more information, see [Log in to Adobe Workfront](../../../../workfront-basics/manage-your-account-and-profile/managing-your-workfront-account/log-in-to-workfront.md).

## Convert tasks and issues to projects using the mobile app on iOS

You can now convert individual tasks and issues to projects in the Workfront mobile app on iOS.

## Log in to the mobile app with fingerprint or face ID

Depending on your device, you can choose to log in to the Workfront mobile app using fingerprint or face ID technology. When you log in to the mobile app, it will ask you if you'd like to log in using whichever authentication method your phone supports.

For more information on how to manage this feature, see [Adobe Workfront for iOS](../../../../workfront-basics/mobile-apps/using-the-workfront-mobile-app/workfront-for-ios.md) or [Adobe Workfront for Android](../../../../workfront-basics/mobile-apps/using-the-workfront-mobile-app/workfront-for-android.md).

## New setting to automatically log users out on mobile

In order to make the Workfront mobile app more secure for you and your company, users will be logged out automatically after 15 days of inactivity. Workfront administrators can customize this time limit in the Web application under Setup > System > Preferences.

For more information, see [Configure system security preferences](../../../../administration-and-setup/manage-workfront/security/configure-security-preferences.md).

## Mobile App Requires Domain When Logging In

As a security improvement, the Workfront Mobile App now requires you to provide your domain if you do not log in with Single Sign-On credentials.

>[!NOTE]
>
>iOS availability:&nbsp;June 12, 2019
>
>Production availability:&nbsp;June 17, 2019

## Delete objects using the Mobile app on iOS

>[!NOTE]
>
>This feature was made available in the app stores for iOS&nbsp;the week of August 19, 2019.

You can now delete objects like tasks, issues, and timesheets in the iOS&nbsp;mobile app. You must have the correct permissions on the object to delete it.

## Filter by Dead Projects in the Mobile app

>[!NOTE]
>
>This feature will be available in the app stores for both iOS&nbsp;and Android the week of August 19, 2019.

We've added Dead Projects as a filter option on the Projects tab in the Mobile app.

## Reset your password using the Mobile app

You can use the Workfront Mobile app to reset your password if you've forgotten it. Tap Forgot Password? and follow the prompts on the screen. You cannot reset your SSO password on the Mobile app.

## New look and feel for Mobile

We've added the following look and feel improvements to enhance your experience in the Workfront Mobile app.

* Moved the following from the top bar of the Details page to more prominent areas on the screen:

   * The plus icon is now in the bottom-left corner of the screen
   * The check mark to start working on an item is now a Work On It button in the top-middle of the screen

* You can now view attached custom forms by tapping Show More at the bottom of the Details page.
* Changed the look of the pages you use to submit tasks, issues, and requests.

