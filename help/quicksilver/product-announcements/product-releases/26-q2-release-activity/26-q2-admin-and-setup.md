---
title: Second Quarter 2026 Administrator enhancements
description: Second Quarter 2026 Administrator enhancements
author: Becky
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: ce152c48-ed72-47ed-b1c5-940c93b4a9ec
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/EqRUPqeqy6fSLryuWDtQGaypBlXmSJiaErDZymB95is
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
    internal-label: Administration
subfeature_v2:
  - id: b04e3dc0-3a59-45b1-aa02-b0b6d5f87eff
    internal-label: Approvals
  - id: d87de1f9-8e24-4c4d-aa4c-a403075091a1
    internal-label: Custom forms
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
---
# Second Quarter 2026 Administrator enhancements

This page describes Administrator enhancements made with the Second Quarter 2026 release to the Preview environment. These enhancements will be made available in the Production environment as noted.

For a list of all changes available at this point in the Second Quarter 2026 release cycle, see [Second Quarter 2026 release overview](/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-q1-release-overview.md).

## Content Review AI Collaborator now available

>[!NOTE]
>
>Preview: April 2, 2026
>Production fast release: April 15, 2026
>Production for everyone: April 16, 2026 

To make it easier for you to benefit from AI in your day-to-day work, we've created the Content Review AI Collaborator. The Collaborator is a way to onboard AI agents into your projects and tasks. You can configure an AI Collaborator with brand guidelines, then assign it to a task as you would a user.

Currently, Content Review is the only available AI Collaborator. More AI Collaborator capabilities will be available in the future.

For more information, see [Configure AI Collaborators](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/configure-ai-collaborators.md).

## Custom quarters are now available as a separate page in Setup

>[!NOTE]
>
>Preview: March 5, 2026
>Production fast release: April 15, 2026
>Production for everyone: April 16, 2026 

We have moved the Custom Quarter area from the Project Preferences section. It is now a standalone section in Setup.  
This update includes the following: 

* The Custom Quarters area is removed from the Project Preferences section in Setup 
* The Custom Quarters section is added to the Setup left panel. The functionality remains the same.  
* The Custom Quarters section has been removed from the Project Preferences section of a group. Group administrators no longer have visibility into the Custom Quarters setup anymore.  

For information, see [Enable custom quarters](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-custom-quarters-projects.md).

## Collapse custom form section by default

>[!NOTE]
>
>Preview: February 26, 2026
>Production fast release: March 12, 2026
>Production for everyone: April 16, 2026

By default, all sections on a custom form are expanded when the form itself is expanded. A new option on the custom form designer allows you to mark a section to be collapsed by default when a user opens the form. This option is applied at the section level, not on fields.

For more information, see [Organize and preview a form](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/organize-a-form.md).

## Rich Text field replacing Text with Formatting field type

>[!NOTE]
>
>Preview: January 29, 2026
>Production fast release: February 12, 2026
>Production for everyone: TBD
>
>This feature has been temporarily removed from the Production environment on February 13, 2026.

The new **Rich text** field type in custom forms is a robust text editor, with formatting options such as superscript and subscript, headings, and tables, in addition to the traditional options of bold, italics, underline, bullets, numbering, hyperlinks, and block quotes. The character limit remains 15,000.

The Rich text field type is replacing the Text with formatting field type. You can quickly convert existing Text with formatting fields to Rich text, by clicking the button in the field options on the right. When you convert, historical data remains on the field and it is used the same way in reports.

For more information, see [Create a custom form](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

## New IP addresses for Workfront email notifications

We are updating the IP addresses used to send email notifications from Workfront. If your organization maintains an email or firewall allowlist, you must add the new IP addresses below to ensure continued delivery of Workfront notifications.

These updates apply to all outbound emails generated by the Workfront application, including approvals, reminders, proof notifications, and other system messages.

US:

* 206.55.149.212
* 206.55.149.214
* 206.55.149.215
* 206.55.149.213
* 206.55.149.211

EU:

* 24.110.76.224
* 24.110.76.223

For more information, see [Configure your firewall's allowlist](/help/quicksilver/administration-and-setup/get-started-wf-administration/configure-your-firewall.md).
