---
content-type: release-notes
keywords: notes,quarterly,update,release
navigation-topic: 2021-2-release-activity
title: 21.2 Other enhancements
description: This page describes all Other enhancements made with the 21.2 release to the Preview environment. These enhancements will be made available in the Production environment the week of May 10, 2021. For a list of all changes available with the 21.2 release, see 21.2 Release overview.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: f136c08b-63c0-4e1e-a048-09eb84a0ed54
TQID: https://experienceleague.adobe.com/u9WNEgL9QU9bPkE3iBu5myxuVGl58V-6qN-zIkwhSIo
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
    internal-label: Work management
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
    internal-label: Administration
  - id: e14a7f57-c82c-4874-a495-5d036cbbdc3d
    internal-label: Resource Management
subfeature_v2:
  - id: c10f2e93-7a58-4212-aa24-684c265ebe76
    internal-label: Requests
  - id: d87de1f9-8e24-4c4d-aa4c-a403075091a1
    internal-label: Custom forms
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
---
# 21.2 Other enhancements

This page describes all Other enhancements made with the 21.2 release to the Preview environment. These enhancements will be made available in the Production environment the week of May 10, 2021. For a list of all changes available with the 21.2 release, see [21.2 Release overview](../../../product-announcements/product-releases/21.2-release-activity/21-2-release-overview.md).

## We are now officially Adobe Workfront

Workfront has rebranded to Adobe Workfront.

The most prominent areas within the Adobe Workfront application and our customer-facing websites are now updated. Other areas will be updated soon.

**Updated areas**

* Login Screen, Top Navigation, Proofing
* Layout Templates UI, Main Menu, Custom Forms Export (Only available in the new Adobe Workfront experience)
* Workfront mobile app (iOS and Android)

Areas updating soon

* Proofing apps for desktop and mobile 
* PDF exports for lists and reports 
* Favicon icon in the browser tab

**Areas updating later**

* Email notifications

## Email allowlist validation

>[!NOTE]
>
>Available only in the new Adobe Workfront experience.

If you use the email allowlist, new and updated user email addresses are now validated against the allowlist. When you add a new user or edit an existing user and enter an email domain not on the allowlist, a message notifies you that the user will not receive email messages. You can still save the user profile, but you should add the domain to the allowlist so that the user will receive emails.

For more information, see [Edit a user's profile](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

## New look and feel for object headers

>[!NOTE]
>
>This feature released to the Production environment on March 10, 2020.
>
>This feature is available only in the new Adobe Workfront experience.

To further reinforce the hierarchy of information and help users more clearly understand what page they are on, each object header now has:

* Colorful, more modern icons for each object type
* The object type listed above the object's name
* An updated font style and text size
* Other minor style changes

Previously, there was no icon and a badge with the object name appeared to the right of the object title.

The page headers of areas in the new Workfront experience—such as Enhanced analytics, Resource Management, and others—also have this updated look and feel.

To learn more about the new object headers in the new Workfront experience, see [New object headers](../../../workfront-basics/the-new-workfront-experience/new-object-headers.md).

![Object header](assets/product-announcement-object-header-350x179.png)

## Updates to object status search responses

Workfront now stores object statuses in a new way.

These changes do not affect how status search requests are made. However, API requests containing an object status search will return an incomplete list of group statuses.

For more information, see [Core API changes: Status search responses](../../../wf-api/api/api-changes-search.md) .

## Event subscription payloads updated to include all fields ending in ID

All event subscription payloads now contain every field that ends in "ID".

It's important to note that each object has its own unique set of associated fields, which includes a unique set of associated fields that end in ID. This means that while each payload contains all of that object's associated fields that end in ID, each object has a different set of fields that end in ID.

## Blueprints beta now available in Preview

>[!NOTE]
>
>This functionality will not be generally available on the Production environment until the 21.3 release, later this year. Available only in the new Adobe Workfront experience.

Blueprints provides basic building blocks to help you create a work management system that grows with you. System administrators can browse the blueprints catalog and install ready-to-use project templates.

For more information, see [Blueprints](../../../administration-and-setup/blueprints/blueprints.md).
