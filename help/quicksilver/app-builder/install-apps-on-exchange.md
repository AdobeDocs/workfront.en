---
title: Installing apps from Adobe Exchange
description: Workfront UI Extensions, powered by Adobe App Builder, allow customers and partners to create customized user experiences.
author: Courtney
feature: Digital Content and Documents

---

# Installing apps from Adobe Exchange

You can now install partner-built apps for Workfront directly from Adobe Exchange. This capability connects customers to a growing ecosystem of Adobe partners who deliver purpose-built tools that improve productivity, streamline operations, and extend Workfront functionality. Through Adobe Exchange, customers can discover and install apps that integrate seamlessly into Workfront using UI Extensions. 

Adobe Exchange is the central marketplace for third-party applications, extensions, and integrations across Adobe Experience Cloud—including Adobe Workfront. For Workfront customers, it's the go-to destination to discover and install apps that enhance functionality, streamline workflows, and integrate with external systems. 


## Adobe partner apps

At the heart of this innovation is the Workfront Partner Network, a growing ecosystem of technology partners—independent software vendors (ISVs) who build scalable, secure, and extensible apps using Adobe App Builder and Workfront UI Extensions. 

These partners use UI Extensions to embed their apps directly into the Workfront interface. Once installed from Adobe Exchange, Workfront administrators can add these apps to layout templates, making them visible and actionable within the Workfront experience. This seamless integration allows users to interact with partner-built tools—such as reporting utilities, automation widgets, or data connectors—without leaving Workfront. 

## Prerequisites and permissions

**App Builder Provisioning**

* Customers must have App Builder provisioned in their Adobe Admin Console. This is a prerequisite for installing apps from Adobe Exchange.

**Enterprise Org Admins or Developers**

* Can search for apps, click **Get**, and proceed with installation. 

* If the app is already acquired by someone in the org, they may see **Begin Installation** or **Manage** instead. 

**Non-Admin Users**

* May initiate acquisition but will be prompted to log in and may encounter restrictions if the app requires admin consent or special licensing.

## Acquire and install apps from Adobe Exchange

Adobe customers can browse, search, and install apps directly from the Adobe Exchange Marketplace to use within Workfront.  

Apps built with Adobe App Builder are listed as _App Builder Applications_ on Adobe Exchange. Each app listing includes documentation, screenshots, and usage instructions to help customers understand the app's value. 

To view apps for Workfront, navigate to Adobe Exchange and search for Workfront-compatible apps. You can also filter listings for Workfront App Builder apps: 

1. Click on **Experience Cloud** in the left-hand panel.
1. In the left panel, find **Product**, then select **Workfront**.
1. Expand **App Type**, then choose **App Builder**.

### Acquire apps

Apps may require purchase from Adobe Exchange or allow installation but require licensing from the app developer. 

To acquire an app

1. Click the name of the app.
1. Click the button located in the top-right corner of the app listing. 
1. Click **Yes, continue** and then accept the end-user license agreement.

### Actions for System Administrators 

When a user acquires an app from Adobe Exchange, they may see the following message: _Your system administrator must approve your acquisition before you can install and use your application._ 

This means the app requires admin-level approval before installation can proceed. System admins can find the request from the following areas:

**Notifications** 

System administrators are typically notified by email when a user in their organization acquires an app.

**Admin Console**

System administrators can log into the Admin Console at [https://adminconsole.adobe.com/](https://adminconsole.adobe.com/) and navigate to Products > App Integrations to view all acquired or requested apps. 

Once a system administrator has access to the requests, they can review and approve the application. Some apps may prompt the admin to consent to data access and assign the app to product profiles or specific users. 

Once approved, the app becomes available for installation. 

## Install apps

Once an app is acquired, it can be installed directly into Workfront. Administrators can manage installed apps through the Workfront interface, ensuring they are properly configured and accessible to users.

1. Find the app you want to install and open the Actions menu on the right side of the screen. 
1. Click View app details. 
1. Select an environment on the left side of the screen or add a new one. 
1. Click **Deploy**. 
1. 


4. Assign Installation or Usage Rights (if required) 

If your organization controls app access via product profiles or user groups, assign the app to the appropriate profile or group so users can proceed with installation and use. 

5. Install and Configure 

Admins can then: 

Click "Begin Installation" or "Manage" if the app has already been acquired 

Follow app-specific instructions provided in the Exchange listing 

In developer console? 

## Contacting App support 

Extensions installed from Adobe Exchange are supported by the app owners. From manage apps, you can click **Get support** to get help with any issues.

## Add to Layout Template 

1. In Workfront, go **to Setup** > **Layout Templates**. 

1. Select the layout template you want to modify.

1. Click **Edit** and choose the section you need.

1. Use the **Add Extension** option to insert the app into the desired location. 

1. Choose the installed extension from the list, and configure its visibility settings. 

1. Click **Save** to apply changes to the layout template.

1. Confirm that the extension appears in the Workfront interface for users assigned to that layout. 

1. Verify Access. 

1. Ensure that users have the necessary permissions via product profiles or user groups (as configured in the Admin Console). 

1. Test the extension to confirm it loads and functions as expected within the Workfront environment. 

 