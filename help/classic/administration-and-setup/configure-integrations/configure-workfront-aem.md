---
filename: configure-workfront-aem
title: Configure Workfront with Adobe Experience Manager
user-type: administrator
product-area: system-administration;workfront-integrations;setup
navigation-topic: administrator-integrations
title: Configure Workfront with Adobe Experience Manager legacy connector
description: As an Adobe Workfront administrator, you can integrate Workfront with Adobe Experience Manager (AEM) Assets and provide your organization with a comprehensive content management solution for the creation, sharing, and maintenance of assets within your workflow.
---

# Configure Workfront with Adobe Experience Manager legacy connector

>[!IMPORTANT]
>
>You're currently viewing the Adobe Workfront Classic version of this document. Adobe Workfront Classic is no longer supported. All Adobe Workfront Classic functionality, along with this documentation, will be removed in July 2022. Please transition to the the new Adobe Workfront experienceas soon as possible, and switch to the new Adobe Workfront experience version of this document.

As an Adobe Workfront administrator, you can integrate Workfront with Adobe Experience Manager (AEM)&nbsp;Assets and provide your organization with a comprehensive content management solution for the creation,&nbsp;sharing, and maintenance of assets within your workflow.&nbsp;&nbsp;

## Access requirements

You must have the following access to perform the steps in this article:

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Plan</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>You must be a Workfront administrator. For information on Workfront administrators, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Grant a user full administrative access</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your Workfront administrator.

## Workfront for AEM Assets

The Workfront for AEM Assets connector allows your organization to do the following:

* Collaborate and manage creative content by linking AEM assets and folders to projects, tasks, issues, and requests in Workfront.

  For more information about configuring documentation integrations with third-party applications, see&nbsp; [Configure document integrations](../../administration-and-setup/configure-integrations/configure-document-integrations.md).

* Integrate with the AEM Digital Asset Management (DAM) repository, allowing you to use Workfront to manage and share digital assets stored in the DAM.

  For more information about linking documents and asset folders, see &nbsp; [Link documents from external applications](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md).

* Combine and apply metadata from both applications to an asset.
* View an all-inclusive communication stream for an asset.&nbsp;Updates and comments made to an asset either in Workfront or AEM Assets are synchronized to the&nbsp;other application, establishing a comprehensive history of communications made to the&nbsp;asset.

  For more information about making comments in Workfront, see [Add an update to a document](../../documents/managing-documents/add-update-documents.md).

## Prerequisites for installing the AEM Assets connector

Before you can install the Workfront connector for AEM Assets, ensure that the following prerequisites are met:

* AEM Assets installed and configured, version 6.5 or later. For information about installing AEM Assets, see the [Adobe Experience Manager documentation](https://docs.adobe.com/docs/en/aem/6-2/deploy.html).
* (Conditional) If your firewall rules don't allow traffic as expected, add your cluster's IP address and/or domain to your allowlist. For more information, see [Configure your firewall's allowlist](../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).

## Install the Workfront for AEM Assets connector package {#install-the-workfront-for-aem-assets-connector-package}

>[!IMPORTANT]
>
>The following instructions are for a Workfront with AEM Assets legacy connector which has been replaced by the [Workfront for Experience Manager enhanced connector](../../documents/workfront-and-experience-manager-integrations/workfront-for-experience-manager-enhanced-connector/workfront-for-aem-enhanced-connector.md). Please contact your Account Rep for more information.

To install the Workfront for AEM Assets connector, you must import the connector into AEM&nbsp;as a package using the CRX Package Manager.

1. On a workstation where you have already installed AEM, download the Workfront for AEM Assets Connector installation file.

   You can get&nbsp;the Workfront for AEM Assets connector from your Workfront representative.

1. Log in to AEM using an administrator account.
1. Click **Tools** > **Deployment** > **Packages**.

   The CRX Package Manager opens.

1. Click **Upload Package.**

1. In the Upload Package dialog box, browse for and select the Workfront Connector package, then click **OK**.  
   The package displays in the CRX Package Manager.

1. Click **Install.**

1. On the Package dialog box, ignore the advanced settings and click **Install**.
1. (Optional) To confirm the connector successfully installed, ensure the following statement displays in the Activity Log:  
   <pre>Package installed in <time></pre>

1. Close the CRX Package Manager.

   The connector is installed and you can now configure AEM Assets to integrate with Workfront.

1. Continue with [Configure AEM Assets to integrate with Workfront](#configure-aem-assets-to-integrate-with-workfront).

## Configure AEM Assets to integrate with Workfront {#configure-aem-assets-to-integrate-with-workfront}

After you install the connector, import the connector package to AEM and configure AEM to link with documents in Workfront.

For information on installing the connector, see&nbsp; [Install the Workfront for AEM Assets connector package](#install-the-workfront-for-aem-assets-connector-package).

* [Prerequisites](#prerequisites) 
* [Integrate AEM with Workfront](#integrate-aem-with-workfront) 
* [Configure the AEM Externalizer](#configure-the-aem-externalizer)

### Prerequisites {#prerequisites}

Before you begin, you must enable permissions for workfront-service:

1. In AEM, go to **Tools**> **Security**> **Permissions**.
1. In the top-left corner, choose **Users**in the drop-down menu and enter *workfront-service* in the **Search**field. Select the workfront-service user.
1. On the right side of the screen, select **Add ACE** to create new entries.
1. In the**Add New Entry**window, select checkbox icon in the **Path**field and choose the folder: */conf*
1. In the Privileges field enter: *jcr:read*
1. Select **Add**in the top-right corner
1. (Optional) Repeat the steps to create more entries.

### Integrate AEM with Workfront {#integrate-aem-with-workfront}

1. Log in to AEM Assets as an Administrator.
1. Click **Tools** >**Cloud Services**>**Workfront Integration Configuration** >**Global-Workfront.******

1. (Conditional) If you have not yet done so, create a Workfront cloud configuration file.

   1. Click&nbsp;&nbsp;**Create** in the upper-right corner of the Global-Workfront page.
   1. In the **Workfront URL** box, specify the URL for your Workfront instance.

      For example, https://*<account>*.my.workfront.com,&nbsp;where *<account>* is the account you use for integrations with AEM.&nbsp;
   
   1. In the**Base Folder** field, select the checkbox icon, then in the drop-down menu select the path where documents that are linked to Workfront objects are stored.
   1. In the AEM modal that appears, follow the path to the folder with the documents that are connected to Workfront objects. Choose the folder and press **Select**in the top-right corner.

      You can link to any folder beneath the root /content/dam/.
   
   1. In the **Workfront API Key** box, specify your Workfront API Key.

      To retrieve your Workfront API key:

      1. Open a browser tab, and log into your Workfront account as a Workfront administrator.
      1. In the **Global Navigation Bar**, click **Setup**.
      
      1. Click **System** >**Customer Info**.

         If you have already generated an API key, your Workfront API Key displays under the Your User's API Key label.
      
      1. (Conditional) If you have not yet generated an API key, you need to generate one:

         1. In the **API Key Settings** section, ensure that the **After Creation, API keys expire in** option is set to None.

            If you select an expiration period, the connector will stop working after the API Key expires. You will then to need to re-generate an API Key and update your Workfront configuration.
         
         1. Under the **Your User's API Key** label, click **Generate API Key**.

            An API Key for Workfront generates and displays.

      1. Copy the API Key to your clipboard.
      1. Open the browser tab for AEM Connector and in the **Workfront API Key** box, paste the API Key you copied.

   1. (Conditional) Click the **Advanced** tab in the upper-left corner of the Workfront Integration Configuration page, and select the following options if applicable:

      **Allow Collection Browsing:**Select this option if your organization allows Workfront users to link AEM Assets collections to Workfront objects.

      **User Federated ID:** Select this option if your organization is using Federated IDs or Single Sign-On (SSO) when logging into Workfront.

      **Ignore Email Domain:** Select this option if your AEM users do not use the domain name in their user ID.&nbsp;

      **Restrict Access:** Select this option to specify the appropriate Workfront IP addresses that need to be added to the allowlist. For more information about the allowlist, see [Configure your firewall's allowlist](../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).
   
   1. Click the **Basic** tab in the upper-left corner of the Workfront Integration Configuration page, and then click **Connect**.

      >[!NOTE]
      >
      >Changes may take some time to apply. Restarting the bundle may speed up the process.

1. (Conditional) If you already created a Workfront cloud configuration file, select&nbsp;**Global-Workfront**, and then in the upper-left corner, click **Properties**.

1. Generate the AEM API Key by clicking **Generate Key,** then copy the AEM API key to your clipboard.

   You will need the AEM API Key later when you configure Workfront to integrate with AEM Assets. For more information, see [Configure Workfront to integrate with AEM assets](#configure-workfront-to-integrate-with-aem-assets).

1. In the upper-right corner, click **Save**.

   The&nbsp;Global-Workfront window displays.

   ![Properties.png](assets/properties-350x117.png)

1. (Optional) Synchronize&nbsp;bi-directional communication between AEM and Workfront.

   1. Click **Global-Workfront.**
   1. In the upper-left corner of the window, click **Properties**.

      The Workfront Integration Configuration page displays.

      ![Properties2.png](assets/properties2-350x444.png)

   1. (Optional) To enable the synchronization of comments between AEM Assets and Workfront, click **Enable Comment Sync**.

      >[!IMPORTANT]
      >
      >You must enable Document Sync to synchronize the assets.

   1. (Optional) To turn off comment synchronization, click **Disable Comment Sync.**

      Or

      Delete the&nbsp;NOTE CREATE event subscription registered to your AEM instance.

      For information on event subscriptions, see [Event Subscription API](../../wf-api/general/event-subs-api.md).

1. Continue with [Configure the AEM Externalizer](#configure-the-aem-externalizer).

### Configure the AEM Externalizer {#configure-the-aem-externalizer}

The AEM Externalizer allows AEM to pass URLs in a format that can be used in Workfront. If not properly configured, Workfront cannot make calls to the AEM API, and the URLs linking AEM documents in Workfront will not work.

1. In AEM, click **Tools** > **Operations** >**Web Console**. 

1. Click **OSGI**, then click **Configuration** in the drop-down menu. 

1. In the configuration list, select**Day CQ Link Externalizer.**

   The Externalizer page displays.

1. In the **Domains** section, ensure the domain listed in the Author field is the domain name externally accessible to AEM users.

   The domain name in the author field should match the domain listed in the URL line of your AEM instance.

   ![Extenalizer.png](assets/extenalizer-350x128.png)

1. (Conditional) If necessary, update the domain in the Author field. 
1. Click **Save**.

   AEM Assets is now configured to link documents with Workfront

1. Continue with [Configure Workfront to integrate with AEM assets](#configure-workfront-to-integrate-with-aem-assets).

## Configure Workfront to integrate with AEM assets {#configure-workfront-to-integrate-with-aem-assets}

After you install the Workfront for AEM Assets Connector (as described in [Install the Workfront for AEM Assets connector package](#install-the-workfront-for-aem-assets-connector-package))&nbsp;and configure AEM Assets (as described in [Configure AEM Assets to integrate with Workfront](#configure-aem-assets-to-integrate-with-workfront)), you need to configure Workfront to link documents between&nbsp;Workfront and AEM Assets.

1. Log in to Workfront as a Workfront administrator.

   >[!TIP]
   >
   >Workfront recommends creating a Workfront administrator dedicated solely to your AEM integration. For more information about assigning the Workfront administrator access level to a user, see [Grant users administrative access to certain areas](../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md).

1. Go to the Setup area in the Global Navigation Bar, click&nbsp;**Setup.**
1. Click&nbsp;**Documents**>&nbsp;**Custom Integration.**

1. Click **Add Custom Integration**.
1. In the&nbsp;**Name** box, specify the name of the custom integration.

   This is the name users see when using the integration within Workfront; for example, you could enter *"AEM Assets"* for the name.&nbsp;

1. In the&nbsp;**Base API URL** box, specify the URL for your AEM instance.

   The base API URL consists of the URL for your AEM instance followed by the path: /bin/webhooks/api/

   ![mceclip3.png](assets/mceclip3-350x130.png)

1. In the&nbsp;**Authentication Type** drop-down menu,&nbsp;select **ApiKey.**

1. In the**API Key** box, paste the AEM API Key you copied when you configured AEM Assets.
1. Click **Save**.
1. (Optional) Ensure the integration is marked Active.  
   ![aem_custom_integration_active.png](assets/aem-custom-integration-active-350x81.png)

   Workfront is now configured to work with AEM Assets.

   In order to access assets in AEM, each Workfront user who needs to use the connector must be set up as a user in AEM. For information on creating users, see&nbsp; [Set up users to use the connector](#set-up-users-to-use-the-connector).

## Set up users to use the connector {#set-up-users-to-use-the-connector}

In order for users to access the connector, they must have a user profile in AEM and belong to a Workfront group that has Access levels that include the Create and Delete permissions.

For more information about Workfront permissions, see [Create or modify custom access levels](../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

* [Set up users in AEM assets](#set-up-users-in-aem-assets)

### Set up users in AEM assets {#set-up-users-in-aem-assets}

1. Log in to AEM Assets as a Workfront administrator.
1. Click&nbsp;**Tools** >******Security** >**Users**.

1. (Conditional) If the user does not have a user profile in AEM, create an AEM user profile.

   1. Click **Create User.**
   1. Enter the user's personal information.

      ![64NewUser.png](assets/64newuser-350x524.png)

      The only required field is the ID field.&nbsp;The user's AEM ID must match their Workfront ID, which is the user's Workfront email address.

      If you selected the&nbsp;Ignore Email Domain option when you configured AEM to integrate with Workfront, then the AEM ID will not match the Workfront email address.&nbsp;

1. (Conditional) If the user has an AEM profile, open the user's AEM profile.

   1. Click**User.**

      The User Management page displays.
   
   1. Click the user you want to add, then click **Properties**.

      The user's settings page displays.

1. Click the **Groups** tab.

   ![](assets/groupstab.png)

1. Ensure the user belongs to at least one Workfront group that has Access levels that include the Create and Delete permissions.

   1. To add the user to an existing group, begin typing the group name in the **Type Group Name** box, then select the group when it appears in the drop-down menu.

      Or

      To select a group to which the user is a member, select a group in the **Groups that this user is a member of** section.

1. Click **Save.**

