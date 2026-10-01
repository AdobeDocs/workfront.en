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

{{highlighted-preview}}

Custom localization allows you to <span class="preview"> use AI</span> to define custom terms and phrases in different languages. Workfront then displays these terms in the language set in the user's Adobe Identity Management (IMS) settings. 

For example, label "Target Audience" can be localized to the German word "Zielgruppe." Any user with German selected as their browser's main language sees the word "Zielgruppe" as a label for any fields labeled "Target Audience" in English.

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
1. (Optional) To translate the word into additional languages, add the translation into the appropriate language column.
1. (Optional) To reorder language columns, click the header of a column you want to move and drag it to the desired location.
1. (Optional) To delete translations for a term, click the checkbox next to the term, then click **Delete** in the blue bar at the bottom of the page.

<div class="preview">

## Localize untranslated custom text using AI translations

You can use AI to localize custom text. You select the term and the languages, and can approve the translations before they are applied.

1. Click the **[!UICONTROL Main Menu]** icon ![Main Menu](/help/_includes/assets/main-menu-icon.png) in the upper-right corner of Adobe Workfront, or (if available), click the **[!UICONTROL Main Menu]** icon ![Main Menu](/help/_includes/assets/main-menu-icon-left-nav.png) in the upper-left corner, then click **[!UICONTROL Setup]** ![Setup icon](/help/_includes/assets/gear-icon-setup.png).
1. In the Setup area, click **Localization** in the left navigation panel.
1. In the Localization area, select the **Untranslated custom text** tab.

   A list of untranslated custom text appears. This includes text such as field labels and custom rule messages.

1. Select one or more terms that you want to localize.
1. In the blue bar at the bottom of the screen, select **Translate with AI**.

   The Generate translations window opens.

1. Click the languages that you want to translate the term or terms into. To quickly select all languages, click **Select all**.
1. (Optional) To provide more specific guidance for the translation, enter instructions into the "Instructions for AI" field.
1. Click **Generate**.

   AI begins to generate translations.

   The Review translations window opens.

1. (Optional) To adjust translations, or to add your own translation, click into the appropriate square of the table, and type the desired translation.
1. Click **Save**.

## Translate a localized term into additional languages 

You can translate a previously localized term into new languages using AI, or provide your own translation.

1. Click the **[!UICONTROL Main Menu]** icon ![Main Menu](/help/_includes/assets/main-menu-icon.png) in the upper-right corner of Adobe Workfront, or (if available), click the **[!UICONTROL Main Menu]** icon ![Main Menu](/help/_includes/assets/main-menu-icon-left-nav.png) in the upper-left corner, then click **[!UICONTROL Setup]** ![Setup icon](/help/_includes/assets/gear-icon-setup.png).
1. In the Setup area, click **Localization** in the left navigation panel.
1. In the Localization area, select the **Translations** tab.

   A list of previously translated terms and their translations displays.

1. (Optional) To edit or directly enter a translation, click on the appropriate box in the table and type in the desired translation.
1. Select the terms that you want to generate additional translations for by clicking the checkboxes next to those terms.
1. In the blue bar at the bottom of the page, click **Fill in with AI**.


   The Generate translations window opens.

1. Click the languages that you want to translate the term or terms into. To quickly select all languages, click **Select all**.
1. (Optional) To provide more specific guidance for the translation, enter instructions into the "Instructions for AI" field.
1. Click **Generate**.

   AI begins to generate translations.

   The Review translations window opens.

1. (Optional) To adjust translations, or to add your own translation, click into the appropriate square of the table, and type the desired translation.
1. Click **Save**.
1. (Optional) To delete all translations for a term, click the checkbox next to the term, then click **Delete** in the blue bar at the bottom of the page.


</div>
