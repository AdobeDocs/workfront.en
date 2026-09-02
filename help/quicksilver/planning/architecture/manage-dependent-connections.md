---
title: Manage Dependent Connections
description: As a workspace manager, you can define dependent connections when creating connection fields between record types in Adobe Workfront Planning. When adding connected fields, you can turn on a setting that indicates that the values of the connected record type depend on the values of the source record type (the one where you're adding the connection), whenever both fields appear together on a third record type.
feature: Workfront Planning
role: User
author: Alina
recommendations: noDisplay, noCatalog
---

# Manage dependent connections

<span class="preview">The information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the release to Preview, the same features are also available monthly in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

{{planning-important-intro}}

As a workspace manager, you can define dependent connections when creating connection fields between record types in Adobe Workfront Planning. 

When adding connected fields, you can turn on a setting that indicates that the values of the connected record type depend on the values of the source record type (the one where you're adding the connection), whenever both fields appear together on a third record type.

For example, you might want to ensure that a Region field only shows values tied to the selected Geo. This is configured directly in the connection field setup: when adding a connection from a Geo record type to a dependent record type (like Region), a new setting allows workspace managers to mark it as dependent on the Geo record type, using the relationships already established between those record types. 

Once configured, any record type that references both fields (such as a Campaign) will see the effect immediately: selecting a Geo value narrows the Region picker to only those Regions actually linked to that Geo. This enforces your record structure automatically, eliminating mismatched combinations and reducing manual cleanup. 

## Access requirements

+++ Expand to view the access requirements for the functionality in this article.

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
</tr> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront package</p></td> 
   <td> 
<p>To connect record types from the same workspace: </p>
<ul> 
<li><p>Any Workfront or Workflow package with any Planning package</p></li>
<p>Or</p>
<li><p>Any Planning package when purchased as a standalone product</p></li>
</ul>

<p>To connect record types from different workspaces:</p>

<ul> 

<li><p>Any Workflow and a Planning Prime or Ultimate package</p></li>
<p>Or</p>
<li><p>Any Planning Prime or Ultimate package when purchased as a standalone product</p></li>
</ul>
   </td> 
<tr> 
<td> 
   <p> Additional products</p> </td> 
   <td> 
   <p> In addition to Adobe Workfront, you must have the following, if you want to connect record types with objects from the following applications:</p>
   <ul><li><p>An Adobe Experience Manager Assets license and an integration between AEM Assets and Workfront to connect AEM assets with Planning record types.</p>
   <p>For information, see <a href="/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/workfront-for-aem-asset-essentials.md">Adobe Workfront for Experience Manager Assets and Assets Essentials: article index</a>. </p></li>
   <li><p> An Adobe GenStudio for Performance Marketing license to connect record types with GenStudio objects and Brands</p>
   <p>For information, see <a href="https://experienceleague.adobe.com/en/docs/genstudio-for-performance-marketing/user-guide/get-started">Get started with Adobe GenStudio for Performance Marketing</a>.</p></li></ul>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront license</p></td> 
   <td><p>Workflow Standard</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Planning license</p></td> 
   <td><p>Planning Standard</p>
   </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Access level configuration</p></td> 
   <td> <p>You must add both a Workflow and a Planning license type to the access level when you have both a Workflow and a Planning package</p>   
</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Object permissions</p></td> 
   <td>   <p>Manage permissions to a workspace</p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p>  </td> 
  </tr>  
</tbody> 
</table> 

 For more information about Workfront access requirements, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).   

+++

<!--
Sent a slack message to Norayr, Predator, Snowstorm, Armine for info for this section: 
-->

## Considerations for dependent connected fields


* Dependent connected fields can only be set up between record types that have an established connection field relationship. You cannot define dependency logic between unrelated record types.

* You can have a dependent connected field between record types in separate workspaces. 

* You cannot have a dependent connected field between Planning record types and Workfront or AEM object types.

* The dependency setting is configured one connection at a time, within the connection field setup itself, rather than as a global rule.

* The filtering behavior between the two connected records only activates when both the source and dependent fields are present together on a third record type. The dependency has no effect if only one of the two fields displays on a record type. 

* The dependent field's picker is limited to values already linked to the selected source value at the record level; it cannot show or suggest unlinked values.

* If the source field's value changes, the dependent field is automatically cleared rather than left in an invalid state, preventing mismatched combinations from persisting.

    You receive an inline or toast message explaining why the dependent field was cleared.

* Each dependent field can have up to 3 direct controlling fields. 

* Dependency levels are limited to 6 connections. This means that up to 7 record types can be connected. 

* For the dependency chain to work, all dependent fields must exist on the same record type at the same time. 

## Create a dependent connection

1. As a workspace manager, go to a record type in Workfront Planning and open it in the table view. 
1. Click the **+** icon in the upper-right corner of the table view to add a new field.
1. Click **New connection**, then start adding a new connection for a second record type. 

    >[!TIP]
    >
    >You can create a dependent connection only between two Planning record types. You cannot create dependent connections between record types and objects from Workfront or AEM. 
1. In the **Connection settings** section, turn on the **Make this connection dependent**.

    >[!TIP]
    >
    >Turning on the **Make this connection dependent** setting automatically turns on the **Create a corresponding field on linked record type**. There is a limit of 500 fields per record type.

    ![New connection tab with dependent connection enabled](assets/dependent-connection-enabled-setting.png)

1. Continue setting up the connection, as described in the article [Connect record types](/help/quicksilver/planning/architecture/connect-record-types.md).
1. Click **Save**. 

    The following things occur: 

    * The connection between the two record types is created and their values will depend on one another when they display together on the same record type. 
    * A corresponding field displaying the first record type is created for the second record type. 
    * When both record types are connected to a third record type, the values displayed as choices for the second connected record field are those that are connected to the first record. The values displayed as choices for the first record type are the ones connected to the second record type. 

        For information, see the section [Example of dependent connected record types](#example-of-dependent-connected-record-types) in this article.  
    * There is an indication in the column header of the connected record fields that explains that the field is in a dependent connection relationship. 

        ![Dependent icon tooltip in column header](assets/dependent-icon-tooltip-in-column-header.png)   
1. (Optional) Click **Record filtering rules** and select fields from the record type you are connecting to to narrow down the options for that field's values, then click **Done**.

    When the two fields are present on a third record type, the options for the connected field record type will be limited by the filter you select. 
1. (Optional and recommended) Go to a third record type and add both the first and second record type as connected record fields. 

    ![Dependent connected field indicator on a third record type](assets/dependent-connected-field-indicator-on-a-third-record-type.png)

## Example of dependent connected record types

This section provides a simple example of how you can set up dependent record types and how they work for a third record type. 

1. In a workspace that you can manage, create the following record types:

    * Campaign
    * Countries
    * Continents

1. In the **Countries** record type, add the following records:

    * France
    * United States
    * Japan
1. In the **Continents** record type, add the following records: 

    * Europe
    * America
    * Asia

1. From the **Countries** record type, create a connected dependent field for **Continents**. 

    This adds the following connected record fields:

    * The **Countries** connected record field for the **Continents** record type.
    * The **Continents** connected record field for the **Countries** record type. 

1. Do one of the following:

    * From the **Countries** record type table view, add the following values for the Continents connected record field: 

        * Europe for France
        * America for United States
        * Asia for Japan
    * From the **Continents** record type table view, add the following values for the **Countries** connected record field:

        * France for Europe
        * United States for America
        * Japan for Asia
1. Add the **Countries** and **Continents** connected fields to the **Campaign** record type table view. 
1. Select **Japan** for the **Countries** field on the **Campaign** record type. Notice that the only value available for the **Continents** connected field on the campaign is **Asia**. 

    Or

    Select **Europe** for the **Continents** field on the Campaign record type. 

    Notice that the only value available for the **Countries** connected field on the campaign is **France**. 



