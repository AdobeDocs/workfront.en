---
title: Create custom applications for Workfront with Adobe App Builder
description: Workfront UI Extensions, powered by Adobe App Builder, allow customers and partners to create customized user experiences.
author: Courtney
feature: Digital Content and Documents
---

# Create custom applications for Workfront with Adobe App Builder

Workfront UI Extensions, powered by Adobe App Builder, allow customers and partners to create customized user experiences. These tools enhance efficiency, deliver seamless, connected experiences, and significantly improve user satisfaction, and help enterprises realize their unique vision.

For example, without Workfront UI Extensions, a project manager might need to switch between Workfront and a separate time-tracking system to log hours. With UI Extensions, time-tracking can be integrated directly in the Workfront experience, streamlining workflow and saving time. Additionally, you can add custom components to improve usability, automate repetitive tasks, and enhance content management with features like metadata tagging and content previews. Adobe App Builder also offers scalability and robust identity management (IMS), ensuring secure and efficient customization at any scale.

Workfront UI extensions offer several key benefits:

* Precise customization: Standard software interfaces often fall short of meeting all business requirements. UI extensions allow developers to modify and extend the default user interface to address specific business needs.
* System integration: UI extensions facilitate the integration of other systems ensuring seamless workflows and data consistency.
* Scalability: As businesses grow, UI extensions can be developed to add new functionalities without the need for a complete system overhaul.
* Reduced development time: Pre-built extension points and tools significantly reduce the time and effort required to implement custom features.
* Enhanced user adoption: An optimized user experience can significantly boost software adoption. Custom UI elements designed to match user preferences can enhance adoption rates and overall satisfaction.
* Leveraging Workfront UI Extensions, businesses can create tailored user experiences that drive efficiency, integration, and user satisfaction.

After an application is created in the Adobe App Builder, a Workfront administrator can add it to the Workfront Main Menu and left navigation panel using layout templates. A user with the layout template who clicks on the application will see the application embedded in Workfront, instead of having to open it separately.

This article describes how to access the App Builder and use a template to create an application.

For information about adding a custom application to layout templates, see [Customize the main menu using a layout template](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-main-menu.md) and [Customize the left panel using a layout template](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-left-panel.md).

## Prerequisites  

You must have the following:  

* An IMS-enabled Workfront account  
* A dev machine with node v18 and npm

## Access Adobe App Builder  

To create UI extensions, you must have access to the Adobe App Builder in the Adobe Developer Console.  

Additional instructions are available on the [Adobe Developer site](https://developer.adobe.com/uix/docs/guides/get-access/).

### Add developers to the Adobe Admin Console  

>[!IMPORTANT]
>
>Make sure you have selected the right IMS organization for all of the following steps. If you belong to multiple organizations, it's possible to select the wrong one. Make sure you are acting under the right organization, which is usually listed in the top-right corner. 

1. Navigate to Production: https://adminconsole.adobe.com/  

1. In the **Users** section, click **Developers** > **Add developers**.

    ![add users in the admin console](assets/manage-users-admin-console.png)

    >[!NOTE]
    >
    >If you do not see an option to manage developers, you do not have a product that allows developer access.  

1. Add the user's email. It should search existing users that have already been added from within the admin console.  

1. Add necessary products to the developer profile and click **Save**.  
    ![add developers](assets/add-developer.png)

### Get access to App Builder  

Organizations must work with their account managers to purchase App Builder.  

To test AppBuilder integration, you can request a free trial for your IMS organization here: https://developer.adobe.com/app-builder/trial/#  

If AppBuilder is configured properly, you should see Create project from template as part of creating a new project.

## Create a new project in the Adobe Developer Console  

You must use the Adobe Developer Console to build your UI extension.  

Additional instructions are available on the [Adobe Developer site](https://developer.adobe.com/uix/docs/guides/creating-project-in-dev-console/).

1. Sign in to the Adobe Developer Console with your Adobe ID.  

1. Choose your account, and your profile or organization.  

1. Click **Create project from template** in the Quick Start area, or click **Create new project > Project from template**.

    >[!IMPORTANT]
    >
    >If you do not see the option to create a project from a template, then you are misconfigured in the admin console and do not have access to the app builder catalog. This option only shows when you have access to AppBuilder.

    ![Create from template](assets/create-from-template.png)

1. Select **App Builder**.  

1. Enter a **Project title** and **App name**. Both have defaults, but it will be easier to identify the project you want later if you customize the value.  

1. Leave **Include runtime** selected.  

1. Click **Save**.  

## Use Adobe IO (aio) CLI

Adobe provides an open source CLI that you can use to create the App Builder application.  

Additional instructions are available on GitHub and the Adobe Developer site: 

* https://github.com/adobe/aio-cli   
* https://developer.adobe.com/app-builder/docs/getting_started/first_app/

1. To install the tool, (make sure you are on node v18 first) run: `npm install -g @adobe/aio-cli`.
1. Launch your terminal and log in to AIO with the command: `aio login`. If you have issues logging into the correct IMS org, try `aio login -f` to force a login prompt. Use `aio where` to see which organization you are logged into the correct IMS org. for more details, use `aio config`.
1. Begin setting up your app by running: `aio app init example-app` be sure to replace "example-app" with your app name. If you are not sure of app names, you can see a list of app names with the command `aio console project list`.
1. Select your Organization and Project from the provided options.
    ![command result](assets/1-command-result.png)
    ![Select a project](assets/2-select-a-project.png)

1. Browse all available templates and choose the **@adobe/workfront-ui-ext-tpl** for your project.
    ![Choose a template](assets/3-choose-template.png)
1. Select and enter the project name you created in the Adobe Developer Console.
    ![select and enter project name](assets/4-select-and-enter-project-name.png)

1. Answer the prompts for the application:  

    * Name the extension.  
    * Provide a descriptive summary of the extension's functionality.  
    * Select an initial version number to start with.  
    * The template will create the code for a primary navigation button if you select "Add a custom button to Main Menu Item" when prompted for "What would you like to do next?".

    ![select done](assets/5-select-done.png)

1. Confirm completion by selecting I'm done. The code generation from the template is in process.
    ![generation in process](assets/6-generation-in-process.png)
1. Wait until you see a message that the app initialization is finished. Then you can open the project in an IDE (VSCode is recommended) and access the src folder.  

    For more information on the folders and files in your project, see the [Adobe developer site](https://developer.adobe.com/app-builder/docs/getting_started/first_app/#5-anatomy-of-an-appbuilder-application).