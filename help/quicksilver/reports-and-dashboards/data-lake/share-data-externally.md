---
content-type: overview;reference
product-area: reports and dashboards
navigation-topic: data connect
title: Establish a connection to Workfront Data Connect
description: Workfront Data Connect allows you to use your organization's Workfront data with business intelligence tools or store it in an external data warehouse.
author: Courtney
feature: Reports and Dashboards
exl-id: 8348f5ff-c1f8-4608-b683-15f6407c6128
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/pPk3qt9-o3QhAajyI4eGhwe0J2tRphXDstrJxmdW8Ww
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
    internal-label: Administration
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
    internal-label: Reporting
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
---
# Establish a connection to Workfront Data Connect

Workfront Data Connect allows you to use your organization's Workfront data with business intelligence tools or store it in an external data warehouse.

In order connect your Data Connect data lake with an external product, you must first create a connection as described in [Create a reader account or connection for Snowflake](/help/quicksilver/reports-and-dashboards/data-lake/create-a-reader-account.md). Then, you must add any required IPs to the allowlist as described in [Add IPs to the allowlist](#add-ips-to-the-allowlist) below.

Most products will require the following information about your data lake to establish a connection:

| Field name    | Value       |
|---------------|-------------|
| Server    | The URL for the connection, without the `https://` portion (found on the **Data Connect** page in Workfront*) |
| Port      | `443`         |
| Database  | `WORKFRONT`   |
| Warehouse | `READER_WH`   |
| Schema    | `WF`          |
| Role      | `READER_ROLE` |
| Username  | The username chosen when creating the connection (found on the **Data Connect** page in Workfront*) |
| Password  | The password chosen upon first Snowflake login* |

*For information on where to find the **Data Connect** page containing your connections, see [Create a reader account or connection for Snowflake](/help/quicksilver/reports-and-dashboards/data-lake/create-a-reader-account.md).

>[!IMPORTANT]
>
>Once one entry is added to the IP allowlist, all other IP addresses are no longer permitted. Ensure you have input all required IP addresses—for both the building and reading experiences of your visualization tool—before attempting to use the tool. If not, you may encounter an error regarding invalid credentials.
>
>If you don't have any IP addresses included in your allowlist but are still having trouble connecting to a BI tool, check the proxy server configuration for the BI tool.

## Access requirements

+++ Expand to view access requirements. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront package</td> 
   <td><p>Ultimate</p>
    <p>Workflow Ultimate</p>
   </td>
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license</td> 
   <td>
   <p>Standard</p>
   <p>Plan</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>You must be a Workfront administrator</p></td> 
  </tr> 
 </tbody> 
</table>

For more detail about the information in this table, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Add IPs to the allowlist

1. Click the **[!UICONTROL Main Menu]** icon ![Main Menu](/help/_includes/assets/main-menu-icon.png) in the upper-right corner of Adobe Workfront, or (if available), click the **[!UICONTROL Main Menu]** icon ![Main Menu](/help/_includes/assets/main-menu-icon-left-nav.png) in the upper-left corner, then click **Setup**.

1. In the left panel, click **System** > **Data Connect**.

1. Click on the **Allowed IPs** tab, then click on the **Add an IP Address to your Allowlist** button.

1. Enter a name for the IP address in **IP Address description** and enter the IP address (or CIDR block) for the tool you would like to use in **IP Address**, then click **Add IP to Allowlist**.

    ![Add IP address](/help/quicksilver/reports-and-dashboards/data-lake/assets/add-IP-allowlist.png) {width="500"}

## Find Azure IP ranges for Microsoft Power BI

Microsoft Power BI traffic to Data Connect doesn't come from a single fixed address. Microsoft publishes the IP ranges as CIDR blocks in a large JSON file. This section explains how to find the blocks for the regions you actually use.

### Official Microsoft source for Azure IP ranges and service tags

Microsoft publishes the list on the [Azure IP Ranges and Service Tags – Public Cloud download page](https://www.microsoft.com/en-us/download/details.aspx?id=56519). Download the current JSON file (the filename is typically similar to `ServiceTags_Public_YYYYMMDD.json`). Refresh your allowlist when Microsoft updates this file, or when connectivity issues appear after a Microsoft change.

>[!NOTE]
>
>The JSON file is very large, often well over 100,000 lines. That is expected. The sections you need are small; you don't need to read the entire file by hand.

### Power BI vs. Power Query Online

Customers sometimes report "Power BI" when the traffic actually comes from Power Query components that Microsoft treats as a separate Azure service in the service tag list.

| If your users… | Look for this service tag in the JSON |
|----------------|---------------------------------------|
| Use the Power BI service, datasets hosted in Azure, or gateways in the cloud context | `PowerBI` (global or regional entries such as `PowerBI.EastUS`) |
| Use Power Query Online, cloud dataflows, and similar experiences | `PowerQueryOnline` (global or regional entries such as `PowerQueryOnline.EastUS`) |

If your organization uses both experiences, add CIDR blocks from both `PowerBI` and `PowerQueryOnline` for the same regions. If you only add one, some users may still be blocked while others succeed.

### Choose regional tags, not the global aggregate

The JSON file contains a single all-regions entry for `PowerBI` (and similarly for `PowerQueryOnline`) that aggregates many regions and can contain hundreds of CIDR blocks, plus many smaller regional entries such as `PowerBI.WestUS`, `PowerBI.WestUS2`, and `PowerBI.WestUS3`. Each regional object lists only the prefixes for that region, typically dozens of lines at most. We don't recommend adding the global entry unless you have a documented requirement to allow every Azure region. For most Data Connect customers, regional entries are the right default. Add the regions where your Power BI tenants and users actually run, plus a small buffer for redundancy (for example, a secondary disaster-recovery region your company uses).

### Choose your regions

Microsoft's region names in the file look like `EastUS`, `WestEurope`, `GermanyWestCentral`, and so on. Use the regions where your Power BI capacity and users are hosted, not where your office is, although they often align.

| Scenario | What to add first |
|----------|-------------------|
| United States usage | Start with the US regions you know your tenant uses (examples: `EastUS`, `EastUS2`, `WestUS`, `WestUS2`, `WestUS3`, `CentralUS`, `SouthCentralUS`). You don't need every US region unless your Microsoft administrator confirms multi-region hosting. |
| European Union or UK usage | Start with the regions your tenant uses (examples: `WestEurope`, `NorthEurope`, `FranceCentral`, `GermanyWestCentral`, `SwedenCentral`, `UKSouth`). Add more only if users span additional Microsoft regions. |
| Asia Pacific usage | Add the regions confirmed by your Power BI or Azure administrator (examples: `SoutheastAsia`, `EastAsia`, `AustraliaEast`). |
| Multiple geographies | Add both sets of regional tags (for example, EU and US) for each service (`PowerBI` and `PowerQueryOnline` if both are in use). |
| Unknown region | Ask your Microsoft 365 or Power BI administrator which Azure regions host your Power BI resources, or review your Power BI Admin tenant settings. If you must unblock quickly for testing, add one known region pair (for example, `EastUS` and `WestUS`) and monitor, then narrow the list once you confirm. |

### Find IP ranges and add them to the allowlist

To collect IP ranges from Microsoft and add them to your Workfront allowlist:

1. Open the [Azure IP Ranges and Service Tags – Public Cloud download page](https://www.microsoft.com/en-us/download/details.aspx?id=56519), download the Service Tags JSON file, and save it locally (for example, `Downloads\ServiceTags_Public_YYYYMMDD.json`).

1. Open the file in any editor that handles large JSON well, such as Visual Studio Code.

1. Use your editor's Find feature (`Ctrl+F` on Windows or `Cmd+F` on macOS) to locate JSON objects whose `"name"` field equals a service tag such as `PowerBI.EastUS` or `PowerQueryOnline.WestEurope`. Useful searches:

    * `"name": "PowerBI.WestUS"` — jump to West US Power BI.
    * `"name": "PowerQueryOnline.WestUS"` — jump to West US Power Query Online.
    * `PowerBI.` — list all Power BI regional tags, then refine to your region name.

1. Under each matching object, find the array named `addressPrefixes`. Each string in that array is a CIDR block (for example, `20.59.79.96/27` or an IPv6 prefix). These are the values you'll add to your Workfront allowlist.

1. Add each CIDR to the Workfront allowlist as described in [Add IPs to the allowlist](#add-ips-to-the-allowlist) in this article. Allow a few minutes for policy propagation if your environment caches rules.

1. From Power BI or Power Query Online, run a small test query against Data Connect to validate the connection. If it fails, capture the approximate time and ask your network team whether denies align with missing ranges. Re-check whether you missed `PowerQueryOnline` when only `PowerBI` was added, which is a common gap.

For example, if your Microsoft administrator confirms that your Power BI workloads use West US, West US 2, and West US 3, and your users use both Power BI and Power Query Online, you would open six objects: `PowerBI.WestUS`, `PowerBI.WestUS2`, `PowerBI.WestUS3`, and the matching `PowerQueryOnline.<Region>` for each, then copy `addressPrefixes` from all six.

### JSON structure reference

Each service tag block looks conceptually like the following. Real files include more metadata.

```json
{
  "name": "PowerBI.WestUS2",
  "id": "PowerBI.WestUS2",
  "properties": {
    "region": "westus2",
    "systemService": "PowerBI",
    "addressPrefixes": [
      "203.0.113.0/24",
      "2001:db8::/32"
    ],
    "networkFeatures": ["API", "NSG", "UDR", "FW"]
  }
}
```

The `addressPrefixes` array contains the CIDR blocks you'll add to Workfront. Other fields are for Azure networking scenarios and don't apply here.

### Maintain the allowlist

* Microsoft changes IP ranges over time. When Microsoft publishes an updated JSON file, refresh or compare your allowlist periodically, especially after a connectivity incident.
* If your environment supports IPv6 to Snowflake and Microsoft lists IPv6 prefixes, include them if your security policy allows IPv6. Otherwise, coordinate with your network team.

## Remove an IP address from the allowlist

1. Click the **[!UICONTROL Main Menu]** icon ![Main Menu](/help/_includes/assets/main-menu-icon.png) in the upper-right corner of Adobe Workfront, or (if available), click the **[!UICONTROL Main Menu]** icon ![Main Menu](/help/_includes/assets/main-menu-icon-left-nav.png) in the upper-left corner, then click **Setup**.

1. In the left panel, click **System** > **Data Connect**.

1. Click on the **Allowed IPs** tab, then click on the trashcan icon ![Delete icon](/help/quicksilver/reports-and-dashboards/data-lake/assets/delete.png) to the right of the IP address you would like to remove.

1. In the window that appears, check the box to confirm and then click **Delete**.

## Share data with Business intelligence tools

A number of common business intelligence tools are listed below; visit their documentation sites to learn more about connecting to your data lake.

* Tableau
* Power BI
* Domo
* SAP HANA

## Store data in an external data warehouse

A number of common data warehouses are listed below; visit their documentation sites to learn more about connecting to your data lake.

* Databricks
* AWS Redshift
