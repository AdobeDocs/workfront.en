---
user-type: administrator
product-area: system-administration;setup
title: Configure Custom Localization
description: Custom localization allows you to define custom terms and phrases in different languages. Workfront then displays these terms in the language set in the browser settings.
author: Becky
feature: System Setup and Administration
role: Admin
---
# Configure custom localization

Custom localization allows you to define custom terms and phrases in different languages. Workfront then displays these terms in the language set in the browser settings.

For example, you can set the label "Target Audience" to translate to the German word "Zielgruppe." Any user with German selected as their browser's main language sees the word "Zielgruppe" as a label for any fields labeled "Target Audience" in English.

You can configure translations to multiple languages. Currently available languages include:

* Chinese (Traditional)
* Chinese (Simplified)
* French
* German
* Italian
* Japanese
* Korean
* Portuguese (Brazil) 
* Spanish

## Access requirements

+++ Expand to view access requirements for the functionality in this article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront package</td> 
   <td> <p>Workflow Prime or higher </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license</td> 
   <td> <p>Standard</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>You must be a Workfront administrator to configure translations.</p>  </td> 
  </tr>
 </tbody> 
</table>

For information, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md). 

+++

## Considerations when setting localization

Consider the following when configuring localization:

* You can configure a term to translate into multiple languages.
* Localization applies to custom field labels (including when used as a column header) and tooltips.
* Custom localization can apply to messages generated from Business Rules, but must be enabled in the Business Rule.

## Configure translations

Translations are configured in the Setup area.

1. Click the **[!UICONTROL Main Menu]** icon ![Main Menu](/help/_includes/assets/main-menu-icon.png) in the upper-right corner of Adobe Workfront, or (if available), click the **[!UICONTROL Main Menu]** icon ![Main Menu](/help/_includes/assets/main-menu-icon-left-nav.png) in the upper-left corner, then click **[!UICONTROL Setup]** ![Setup icon](/help/_includes/assets/gear-icon-setup.png).
1. In the Setup area, click **Localization** in the left navigation panel.
1. To add a new translation, click **New row**.
1. In the **English** column, enter the English term that should be translated.
1. In the column for the language that you want the term to be translated, enter the term in the target language.
1. To translate the word into additional languages, add the translation into the appropriate language column.
1. To reorder language columns, click the header of a column you want to move and drag it to the desired location.

## Enable localization in a Business Rule

You must enable translation of a business rule message in the business rule. If translation is not enabled, the message appears to the reader in English, even if the message text is in the Localization list and the user's browser is set to the appropriate language.

1. Begin configuring a Business Rule.
1. When configuring the rule, insert the word TRANSLATE before the message, and enclose the message in parentheses.

>[!BEGINSHADEBOX]

Example:

This example assumes that the message "You cannot edit completed projects" is included in the localization area of Setup, and that the user's browser is set to the localized language.

* `IF({status} = "CPL", "You cannot edit completed projects.") `
The message appears in English.
* `IF({status} = "CPL", TRANSLATE("You cannot edit completed projects."))`
The message appears in the localized language.

>[!ENDSHADEBOX]
