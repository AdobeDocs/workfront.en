---
user-type: administrator
product-area: system-administration;setup
title: Configure Custom Localization
description: Custom localization allows you to define custom terms and phrases in different languages. Workfront then displays these terms in the language set in the browser settings.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: bdc6d5ee-2037-4d0b-bf18-3e6cc9cb078e
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: d5896d07-2812-5418-8b18-8957a0d7f0fb
    internal-label: System Setup and Administration
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
    internal-label: Admin
---
# Configure custom localization

Custom localization allows you to define custom terms and phrases in different languages. Workfront then displays these terms in the language set in the user's Adobe Identity Management (IMS) settings. 

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

   For instructions, see [Enable localization in a Business Rule](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/business-rules.md#using-custom-localization-with-business-rules) in the article Create and edit business rules.

## Configure translations

Translations are configured in the Setup area.

1. Click the **[!UICONTROL Main Menu]** icon ![Main Menu](/help/_includes/assets/main-menu-icon.png) in the upper-right corner of Adobe Workfront, or (if available), click the **[!UICONTROL Main Menu]** icon ![Main Menu](/help/_includes/assets/main-menu-icon-left-nav.png) in the upper-left corner, then click **[!UICONTROL Setup]** ![Setup icon](/help/_includes/assets/gear-icon-setup.png).
1. In the Setup area, click **Localization** in the left navigation panel.
1. To add a new translation, click **New row**.
1. In the **English** column, enter the English term that should be translated.
1. In the column for the language that you want the term to be translated, enter the term in the target language.
1. To translate the word into additional languages, add the translation into the appropriate language column.
1. To reorder language columns, click the header of a column you want to move and drag it to the desired location.
