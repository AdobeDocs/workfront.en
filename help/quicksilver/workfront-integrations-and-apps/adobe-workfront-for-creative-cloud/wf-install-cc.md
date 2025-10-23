---
product-area: workfront-integrations;setup
navigation-topic: adobe-workfront-for-creative-cloud
title: Install and open [!DNL Adobe Workfront for design and video]
description: You can install [!DNL Adobe Workfront for design and video] from the Adobe Marketplace.
author: Courtney
feature: Workfront Integrations and Apps, Digital Content and Documents
exl-id: f4fbae93-b54b-4d08-82c3-72a9a760c317
---
# Install and open [!DNL Adobe Workfront for design and video]

You can install [!DNL Adobe Workfront for design and video] from the [!DNL Adobe Marketplace]. This plugin supports the following Creative Cloud applications: 

{{cc-plugin-app-list}} 

[!DNL Adobe Workfront for design and video] supports the following languages:

* English
* French
* German
* Italian
* Spanish
* Japanese
* Portuguese 
* Simplified Chinese
* Traditional Chinese
* Korean 

>[!NOTE]
>
>There are separate installation instructions for [!DNL Photoshop] and [!DNL XD]. For more information, see [Install [!DNL Adobe Workfront for Photoshop]](/help/quicksilver/workfront-integrations-and-apps/adobe-workfront-for-creative-cloud/wf-cc-install-ps.md) and [Install [!DNL Adobe Workfront for XD]](/help/quicksilver/workfront-integrations-and-apps/adobe-workfront-for-creative-cloud/wf-adobe-xd-install.md).


## Access requirements

+++ Expand to view access requirements for the functionality in this article.

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
 <!-- <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] package/td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] license*</td> 
   <td>
   <p>Standard</p>
    <p>Work or higher</p> </td> 
  </tr> -->
  <tr> 
   <td role="rowheader">Additional products</td> 
   <td><p>You must have an [!DNL Adobe Creative Cloud] license in addition to a [!DNL Workfront] license.</p></td> 
  </tr> 
 </tbody> 
</table>

For information, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md). 

+++

## Prerequisites

* You must install the [!DNL Creative Cloud] app you wish to use before installing the Workfront plugin for that app. 

## Install [!DNL Workfront for design and video] for your organization

If you are an [!DNL Adobe Admin Console] administrator, you can include [!DNL Adobe Workfront for design and video] in [!DNL Creative Cloud] deployment packages. For more information, see [Including plugins in your package](https://helpx.adobe.com/in/enterprise/using/manage-extensions.html).

[View a video tutorial here](https://www.youtube.com/watch?v=zzvXNLIBzrc){target=_blank}.

[!DNL Adobe Admin Console] administrators can also create plugin-only packages for distribution to users. For more information, see [Create [!UICONTROL [!DNL Adobe Workfront] for [!DNL Creative Cloud]] packages for your users in the [!DNL Adobe Admin Console]](/help/quicksilver/administration-and-setup/configure-integrations/create-plugin-only-packages.md)

## Install [!DNL Workfront for design and video] individually

You can install [!DNL Adobe Workfront for design and video] for yourself from the [!DNL Adobe Exchange].

1. Go to the [Adobe Workfront for Design and Video install page](https://adobe.com/go/cc_plugins_discover_plugin?pluginId=108938&workflow=share) on the Adobe Exchange.
1. In the dialog that appears, click **Open [!DNL Adobe Creative Cloud] desktop app**.
1. Once [!DNL Adobe Creative Cloud] plugin manager opens, click **[!UICONTROL Install]**.
1. Read the information in the dialog box, then click **[!UICONTROL OK]**.
1. Once [!DNL Workfront for design and video] in installed, open the [!DNL Creative Cloud] app you need and locate the [!DNL Workfront] plugin in the plugin panel.

1. Continue to the following section for information on how to open [!DNL Workfront for design and video].

## Open [!DNL Adobe Workfront for design and video]

1. Open the Creative Cloud plugin you wish to use.

1. Create a new project, or open an existing one.  

1. In the top menu, click **Windows** > **Extensions** > **Adobe Workfront Menu**.

   >[!NOTE]
   >
   >If you're using Premiere Pro, you must have a project open to access this menu. 

   ![Workfront menu](assets/adobe-workfront-menu.png)


   >[!TIP]
   >
   >If you don't see [!DNL Adobe Workfront for design and video] after opening it from the Extensions menu, it could be behind the Creative Cloud app. Try minimizing the app to find the plugin. 

1. Continue to the following section for information on how to log in to [!DNL Adobe Workfront for design and video].


## Log In to [!DNL Adobe Workfront for design and video]

1. From the **[!UICONTROL Plugins]** menu at the top of the screen, select **[!UICONTROL Plugin Panel]**.
1. Select **[!DNL Adobe Workfront for design and video]**.
1. Enter your domain, then click **[!UICONTROL Log in]**. A browser page opens.

   >[!TIP]
   >
   >* To find your domain, open a browser, navigate to your [!DNL Workfront] instance, and copy the first part of the URL:  
   >
   >![Locate domain](assets/domain-350x50.png)   
   >
   >* If your Workfront instance is integrated with Experience Cloud, ask your admin to provide you with the Workfront domain found under Product > Workfront in the Admin Console.

1. In the browser, enter your [!DNL Workfront] credentials, then click **[!UICONTROL Log in]**. If your company uses a single sign-on (SSO), you'll be directed to your SSO provider's page to log in.

   >[!NOTE]
   >
   >You may not be prompted to enter your [!DNL Workfront] credentials if you logged in recently.

1. Follow the prompts to log in to [!DNL Workfront].

   >[!NOTE]
   >
   >* [!DNL Workfront] connects to [!DNL Adobe Creative Cloud] using OAuth 2.0, a secure standard used by most web-based integrations for the authentication and authorization of users.
   >* When you are prompted to enter the [domain or host] of your [!DNL Workfront] account, type it using this format: *yourCompany'sDomain.my.workfront.com*. Your company's domain is usually the name of your company.  

1. Click **[!UICONTROL Allow Access]** to finish logging in.
1. Go back to [!DNL Adobe Photoshop] to see your work.

### Troubleshooting log in errors

**"Something went wrong" error displays when trying to log in**


You can't use a URL that starts with `experience.adobe.com` to log into the plugin. 

![log in error](assets/plugin-log-in-error.png) ![domain](assets/incorrect-domain.png)


To fix this issue, 

1. Delete the folder that stores the domain for the plugin.

   >[!TIP]
   >
   >On a Mac, Go to Finder, press **Command+Shift+.** to display hidden folders, navigate to **/Users//Library/Application Support**, then delete the **Workfront** folder.


1. Navigate back to the plugin and enter your Workfront domain. The domain must be `company-name.my.workfront.com` and not `experience.adobe.com`.

   To [find your Workfront domain](/help/quicksilver/wf-api/tips-tricks-and-troubleshooting/locate-domain-for-api.md) if you are on the Adobe Unified Experience, go to Setup, Customer info.
