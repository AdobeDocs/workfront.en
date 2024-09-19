---
content-type: overview;reference
product-area: reports and dashboards
navigation-topic: data connect
title: Establish a connection to Workfront data lake
description: Workfront data lake allows you to use your organization's Workfront data with popular business intelligence tools or store it in an external data warehouse.
author: Nolan
feature: Reports and Dashboards
recommendations: noDisplay, noCatalog
exl-id: 8348f5ff-c1f8-4608-b683-15f6407c6128
---
# Establish a connection to Workfront Data Connect

Workfront Data Connect allows you to use your organization's Workfront data with business intelligence tools or store it in an external data warehouse.

In order connect your Data Connect data lake with an external product, you must first add any required IPs to the allowlist as described in [Add IPs to the allowlist](#add-ips-to-the-allowlist) below. Additionally, most products will require additional information about your data lake to establish a connection:

| Field name    | Value       |
|---------------|-------------|
| Server    | The URL for the connection, without the `https://` portion (found on the **Data access** page in Workfront*) |
| Port      | `443`         |
| Database  | `WORKFRONT`   |
| Warehouse | `READER_WH`   |
| Schema    | `WF`          |
| Role      | `READER_ROLE` |
| Username  | The username chosen when creating the connection (found on the **Data access** page in Workfront*) |
| Password  | The password chosen upon first Snowflake login* |

*For information on where to find the **Data access** page containing your Data Connect connections, see [Create a reader (service) account for Snowflake](/help/quicksilver/reports-and-dashboards/data-lake/create-a-reader-account.md).

>[!IMPORTANT]
>
>Once one entry is added to the IP allowlist, all other IP addresses are no longer permitted. Ensure you have input all required IP addresses—for both the building and reading experiences of your visualization tool—before attempting to use the tool. If not, you may encounter an error regarding invalid credentials.
>
>If you don't have any IP addresses included in your allowlist but are still having trouble connecting to a BI tool, check the proxy server configuration for the BI tool.

## Add IPs to the allowlist

1. Click the **[!UICONTROL Main Menu]** icon ![Main Menu](/help/_includes/assets/main-menu-icon.png) in the upper-right corner of Adobe Workfront, or (if available), click the **[!UICONTROL Main Menu]** icon ![Main Menu](/help/_includes/assets/main-menu-icon-left-nav.png) in the upper-left corner, then click **Setup**.

1. In the left panel, click **System** > **Data Access**.

1. Click on the **Allowed IPs** tab, then click on the **Add an IP Address to your Allowlist** button.

1. Enter a name for the IP address in **IP Address description** and enter the IP address (or CIDR block) for the tool you would like to use in **IP Address**, then click **Add IP to Allowlist**.

    ![Add IP address](/help/quicksilver/reports-and-dashboards/data-lake/assets/add-IP-allowlist.png) {width="500"}

## Remove an IP address from the allowlist

1. Click the **[!UICONTROL Main Menu]** icon ![Main Menu](/help/_includes/assets/main-menu-icon.png) in the upper-right corner of Adobe Workfront, or (if available), click the **[!UICONTROL Main Menu]** icon ![Main Menu](/help/_includes/assets/main-menu-icon-left-nav.png) in the upper-left corner, then click **Setup**.

1. In the left panel, click **System** > **Data Access**.

1. Click on the **Allowed IPs** tab, then click on the trashcan icon ![Delete icon](/help/quicksilver/reports-and-dashboards/data-lake/assets/delete.png) to the right of the IP address you would like to remove.

1. In the window that appears, check the box to confirm and then click **Delete**.

## Share data with Business intelligence tools

A number of common business intelligence tools are listed below; the links will take you to the service's documentation site to learn more about connecting to your data lake.

* [Tableau](https://help.tableau.com/current/pro/desktop/en-us/basicconnectoverview.htm)
* [Power BI](https://learn.microsoft.com/power-query/connectors/snowflake)
* [Domo](https://www.domo.com/appstore/connector/snowflake-connector/overview)
* SAP HANA

## Store data in an external data warehouse

A number of common data warehouses are listed below; the links will take you to each service's documentation site where you can learn more about connecting to your data lake.

* [Databricks](https://docs.databricks.com/en/connect/index.html)
* [AWS Redshift](https://docs.aws.amazon.com/redshift/latest/gsg/federated-query.html)
