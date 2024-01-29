---
title: other updates during the 22.3 release timeframe
description: other updates during the 22.3 release timeframe
author: Luke
draft: Probably
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 88d4c34e-9a3a-489d-ac97-2d81903104d8
---
# 22.3 Other enhancements

This page describes all other enhancements made with the 22.3 release to the Preview environment. These enhancements were made available in the Production environment the week of July 11, 2022. For a list of all changes available with the 22.3 release, see [22.3 Release overview](../../../product-announcements/product-releases/22.3-release-activity/22-3-release-overview.md).

## Updated timesheets

We are continuing to improve and update your experience when working with timesheets. The following are some of the features included with this update:

*   A new look and feel to match the new Workfront experience.
    
*   Autosave functionality to automatically save your logged hours and hour comments the second you add them.
    
*   A more intuitive page layout to match other object pages. For example, we have added a left panel to the timesheet. The timesheet updates are now displayed in the Updates section in the left panel. You can also delete a timesheet from the timesheet page as well as add the timesheet to your Favorites list.
    
*   A better experience when searching for and adding projects, tasks, or issues to the timesheet. This matches the experience in all other lists in Workfront.
    
*   The Summary panel is available for tasks and issues to add comments or update information right from the timesheet.
    

With the current update, we have also deprecated the following features:

*   Creating a task from an update has been removed. This feature has been removed since the 2018.2 release from the Updates areas of all other objects, but it was still available in the timesheet update stream.
    
*   The "Add expenses from a timesheet. "preference has been removed from the Timesheet & Hours Preferences area of Setup and you can no longer log expenses from the timesheet. You can still log expenses from the task and project pages.
    

For more information, see the following articles:

*   [Understand the Timesheet layout](/help/quicksilver/timesheets/timesheets/timesheet-layout.md)
    
*   [Configure timesheet and hour preferences](/help/quicksilver/administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md)
    

## Enhancements to left navigation panel

We have made several enhancements to the left navigation panel in Adobe Workfront.

*   The look and feel of the left navigation panel was updated to Adobe design standards, including colors and fonts.
    
*   The "Add custom section" link at the bottom of the panel has been renamed "Add dashboard" to better explain its function.

## Enable automatic refresh token rotation in your custom OAuth2 applications

To allow you more control over the security of your custom OAuth2 applications, we've added to option to enable refresh token rotation. When this option is enabled, every time a refresh token is used, your application automatically creates and sends a new refresh token, and disables the old one.

Your application must store the new refresh token after every refresh. Workfront does not store this refresh token.

Previously, refresh tokens expired after a set amount of time configured in the custom OAuth2 application settings.

For more information, see [Create OAuth2 applications for Workfront integrations](/help/quicksilver/administration-and-setup/configure-integrations/create-oauth-application.md).

## Use PKCE in your custom OAuth2 integrations for Single-page web applications

You can now create Single-page web applications in your custom integrations using PKCE. PKCE is a secure authorization flow that works well with dynamically refreshing applications such as mobile apps, but is valuable across all OAuth2 clients. Instead of a static client secret, PKCE uses a dynamically generated string, eliminating the risk of a leaked client secret.

Previously, the available options for custom OAuth2 applications used either a user's name and password, or a client secret.

For more information, see [Create OAuth2 applications for Workfront integrations](/help/quicksilver/administration-and-setup/configure-integrations/create-oauth-application.md).
