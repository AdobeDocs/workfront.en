---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: "Grouping: Indicate Whether the Results of a Grouping Should Be Collapsed or Expanded Using Text Mode"
description: "Grouping: indicate whether the results of a grouping should be collapsed or expanded using text mode"
author: Courtney
feature: Reports and Dashboards
exl-id: 2880e06f-34f3-47b1-9462-5a15a20d6fee
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/L9BiFaO82lbKPFzZQu5yhpHET9TtLHDGv733ncEkMd8
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
# Grouping: indicate whether the results of a grouping should be collapsed or expanded using text mode

<!--Audited: 10/2024-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: this article: NWE only; not possible in classic) </p>
-->

You can indicate whether the results in a grouping should display collapsed or expanded in a list or report by using the standard report builder. The results in a grouping display expanded, by default. For information about creating a grouping, see [Create groupings in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/create-groupings.md).

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: the tips repeat in the Create groupings to organize results article, Understanding text mode, Edit groupings to organize reports, Create a Custom Report; create a snippet when convenient)</p>
-->

>[!TIP]
>
>* When you manually adjust groupings when viewing a list, Adobe Workfront remembers your manual preference until you log out. When you log back in, the list displays according to this setting.
>* The results of a grouping always display expanded after accessing them from a chart element.
>

You can also indicate whether a grouping should display expanded or collapsed using text mode.

## Access requirements

+++ Expand to view access requirements for the functionality in this article. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront package</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license</td> 
   <td> 
   <p>Contributor or Request to modify a filter </p>
   <p>Standard or Plan to modify a report</p>
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>Edit access to Reports, Dashboards, Calendars to modify a report</p> <p>Edit access to Filters, Views, Groupings to modify a filter</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to a report</p>  </td> 
  </tr> 
 </tbody> 
</table>

For more detail about the information in this table, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Indicate whether the results of a grouping should be collapsed or expanded using text mode

1. Go to a list of objects.
1. From the **Grouping**drop-down menu, select **New Grouping**.

1. Add a grouping, then click **Switch to Text Mode**.

   Or

   If the grouping is already in text mode, add the following code to the grouping level that you want to display collapsed:

   `group.0.iscollapsed=true`

1. (Optional) If you want the grouping to display expanded, add the following code to the appropriate grouping level:

   `group.0.iscollapsed=false`

1. Click **Done**, then **Save Grouping**. 
1. (optional) Update the name of the grouping, then click **Save Grouping**.
