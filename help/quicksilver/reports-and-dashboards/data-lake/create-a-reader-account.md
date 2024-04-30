---
content-type: reference
product-area: reports and dashboards
navigation-topic: data lake
title: Create a  reader (service) account for Snowflake
description: In order to access the data in the Workfront Data Lake, you must first create a reader account for Snowflake.
author: Nolan
feature: Reports and Dashboards
recommendations: noDisplay, noCatalog
exl-id: 70d83a10-f926-4229-ac10-7659f2ca5e7a
---
# Create a reader (service) account for Snowflake

In order to access Workfront data lake data, you must first create a Snowflake reader (or service) account for each new connection. After creating a connection, you can find its associated URL and username by clicking on it on the **Data access** page (**Main menu** > **Setup** > **System** > **Data access**) under the **Existing Connections** tab.

For information on using a newly created connection with an external product, see [Establish a connection to Workfront data lake](/help/quicksilver/reports-and-dashboards/data-lake/share-data-externally.md).

## Access requirements

You must have the following access to perform the steps in this article: 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan</td> 
   <td>TBD</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license</td> 
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>You must be a Workfront administrator.</p></td> 
  </tr> 
 </tbody> 
</table>

For more detail about the information in this table, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Create a reader account

1. Click the **[!UICONTROL Main Menu]** icon ![Main Menu](/help/_includes/assets/main-menu-icon.png) in the upper-right corner of Adobe Workfront, or (if available), click the **[!UICONTROL Main Menu]** icon ![Main Menu](/help/_includes/assets/main-menu-icon-left-nav.png) in the upper-left corner, then click **Setup**.

1. In the left panel, click **System** > **Data Access**.

1. Click **Create New Connection**

1. In the window that appears, enter a name for your connection in **Connection reference description** and a username in **Connection user**, then click **Generate Connection**.

    ![Create reader account](/help/quicksilver/reports-and-dashboards/data-lake/assets/new-reader-connection.png) {width="500"}

1. A **Default password** will be generated, as well as a URL where your data can be viewed through Snowflake. You will need to use the password in conjunction with the username you chose to sign in to Snowflake for the first time, so ensure that you keep a record of it as well as the URL. Check the box claiming you have done so, then click **Close**.

    ![Default account password](/help/quicksilver/reports-and-dashboards/data-lake/assets/default-password-reader-account.png) {width="500"}

1. Open Snowflake using a browser to navigate to the URL from the previous step, enter the username you selected and the default password from the previous step, then click **Sign in**.

1. After successfully signing in for the first time, you will be prompted to choose a new password. Enter a password of your choice in both the **New password** and **Confirm password** fields, then click **Submit**.

    ![Reset Snowflake password](/help/quicksilver/reports-and-dashboards/data-lake/assets/reset-snowflake-password.png) {width="300"}

1. You may now use your username and new password to access your Workfront data lake in Snowflake or the business visualization tool of your choice.

## Revoke a reader account

1. Click the **[!UICONTROL Main Menu]** icon ![Main Menu](/help/_includes/assets/main-menu-icon.png) in the upper-right corner of Adobe Workfront, or (if available), click the **[!UICONTROL Main Menu]** icon ![Main Menu](/help/_includes/assets/main-menu-icon-left-nav.png) in the upper-left corner, then click **Setup**.

1. In the left panel, click **System** > **Data Access**.

1. Click on the trashcan icon ![Delete icon](/help/quicksilver/reports-and-dashboards/data-lake/assets/delete.png) to the right of the account you would like to revoke.

1. In the window that appears, check the box to confirm and then click **Delete**.
