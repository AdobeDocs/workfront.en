---
content-type: reference
navigation-topic: get-started-with-workfront
title: Supported languages in Adobe Workfront
description: You can change the language in which you display Adobe Workfront and emails coming from Workfront, by adjusting the language preferences on your browser and your default Email Locale within Workfront.
feature: Get Started with Workfront
author: Caroline
exl-id: 0b76175f-5fe2-49df-b605-68e6e66b4366
---
# Supported languages in Adobe Workfront

You can change the language in which you display Adobe Workfront and emails coming from Workfront, by adjusting the language preferences on your browser (if not on IMS) or your Adobe Experience Cloud profile language preferences (if on IMS) and your default Email Locale within Workfront.

Workfront terminology is updated for the supported languages with every Workfront update.

Workfront supports the following languages:

* English (en-US)
* French (fr-FR)
* German (de-DE)
* Japanese (ja)
* Spanish (es)
* Italian (it_IT)
* Portuguese (pt-BR)
* Korean (ko)
* Chinese - Simplified (zh-CN)
* Chinese - Traditional (zh-TW)

The language used to view Workfront in your browser is controlled by your browser language settings if your organization is not on IMS, or by your Adobe Experience Cloud profile language if your organization is not on IMS. In either case, ensure you select a language which is listed in the supported languages list.

To display outgoing emails in any of the supported languages, modify your User Email Locale or Customer Info settings in Workfront.  
You must be a Workfront administrator to modify the Customer Info settings.  
For more information about changing the Customer Info and User Email Locale, see [Change the Workfront and User Email Locales](#change-the-workfront-and-user-locales).

You can contract a third party to have the Workfront interface and the outgoing emails from Workfront translated in other languages. These translations are not supported by Workfront and any language outside of the ones listed above are unsupported.

>[!NOTE]
>
>Portions of the interface might still be untranslated for the following:  
>
>* When using an unsupported language, the interface displays in English
>* The Help menu, as well as the help content accessed from that menu, displays in English
>* User-entered text remains in the original language entered. This can include, but is not limited to:
>
>   * Project names
>   * Task names
>   * Issue names
>   * Portfolio names
>   * Program names
>   * Approval names
>   * Descriptions
>   * Custom Form names
>   * Hour Types names
>   * Expense Types
>   * Milestones
>   * Custom tabs
>   * Statuses
>   * Report names
>

## Supported language discrepancies when using proofing

The Web Proofing Viewer within Workfront supports most languages that are supported in Workfront.

The following languages are not supported in the proofing tool:

* Chinese - Simplified (zh-CN)
* Chinese - Traditional (zh-TW)
* Portuguese (pt-BR)

Your company must purchase a proofing license for you to access the Web Proofing Viewer.

For more information about proofing, see [Proofing](../review-and-approve-work/proofing/proofing.md).

When viewing Workfront in a language not supported in the proofing tool, the Web Proofing Viewer displays in English.

If you use Workfront Proof (the standalone proofing tool) in a language that is not supported in Workfront, the Web Proofing Viewer within Workfront displays in English.  
For more information about the languages supported in Workfront Proof, see [Language Settings in Workfront Proof](../workfront-proof/wp-getstarted/system-information/language-settings.md).

## Supported language in Adobe Workfront Fusion

Currently, Workfront Fusion supports only English.

* All content in Workfront Fusion, as well as any help content related to Workfront Fusion, displays in English.
* Workfront Fusion does not support the use of non-English text characters in user-entered fields.

Your company must purchase a Workfront Fusion license for you to access Workfront Fusion.   
For more information about Workfront Fusion, see [Adobe Workfront Fusion overview](../workfront-fusion/get-started/workfront-fusion-overview.md).

## Change the language

You can change the language in which you view Workfront and the language of the outgoing emails by modifying the following settings:

* The language on your browser (for users not on IMS)
* The primary and secondary language of your AEM profile (for users on IMS)
* The Customer Info and User Email Locale settings in your Workfront account.

In order to see all available translations for your chosen language, both the Workfront locale and browser locale should be set to the same language.

* [Change the browser language](#change-the-browser-language)
* [Change the Adobe Experience Cloud language](#change-the-adobe-experience-cloud-language)
* [Change the Workfront and User Email Locales](#change-the-workfront-and-user-locales)

### Change the browser language {#change-the-browser-language}

If your organization is not on IMS, when you change the browser language, your Workfront interface displays in that language.   
For more information about what languages are supported by Workfront, see [Supported languages in Adobe Workfront](#supported-languages).

The browser language must be changed on an individual user basis.

See the "Help" menu for your browser for specific information about how to change the language of your browser.

## Change the Adobe Experience Cloud language

If your organization is on IMS, your Adobe Experience Cloud profile language determines the language that displays in Workfront. 

1. Click your profile picture at the far right end of the Adobe Experience Cloud toolbar, then click **Preferences**. The Adobe Experience Cloud toolbar is directly above the main Workfront toolbar.

1. Under **Profile** beneath your name and email address, click the name of the currently selected language.

1. Select your preferred languages in the dropdowns **First language** and **Second language**. The first language is your default language choice, while the second language will be displayed only if the first language is not supported by a specific application. 

### Change the Workfront and User Email Locales {#change-the-workfront-and-user-locales}

* [Change the default Workfront Email Locale](#change-the-workfront-locale) 
* [Change the User Email Locale](#change-the-user-locale)

### Change the default Workfront Email Locale {#change-the-workfront-locale}

When changing the default Workfront Email Locale, you modify the language, date, and number format used in outgoing messages for all Workfront users. These settings become the default for every new user you create.

To change the default Workfront Email Locale:

1. Log in to Workfront as the Workfront administrator.
1. Click the **Main Menu** icon ![](assets/main-menu-icon.png) in the upper-right corner of Adobe Workfront, then click **Setup** ![](assets/gear-icon-settings.png).

1. Click **System** > **Customer Info.**

1. In the **Basic Info** section, click the **Default Email Locale** drop-down list to select the language that you want Workfront emails to display in.

1. Click **Save**.

### Change the User Email Locale {#change-the-user-locale}

When changing your User Email Locale, you modify the language, date, and number format used in your outgoing messages. These settings override the system settings selected in the Customer Info area of Setup.

To change your User Email Locale:

1. Click the **Main Menu** icon ![](assets/main-menu-icon.png) in the upper-right corner of Adobe Workfront, then click your user profile picture.

1. Click the More menu ![](assets/more-icon.png), then click **Edit**.

1. In the **Preferences** section, click the **Email Locale** drop-down list to select the language that you want Workfront emails to display in.

1. Click **Save Changes**.
