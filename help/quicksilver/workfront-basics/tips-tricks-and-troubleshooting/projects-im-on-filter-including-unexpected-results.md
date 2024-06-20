---
content-type: tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-basics
title: Projects I'm On filter including unexpected results
description: Read this article to troubleshoot the Projects I'm On filter including unexpected results.
feature: Get Started with Workfront
author: Nolan
exl-id: 4701464a-4cf5-4be1-bcc0-0892019986ec
---
# Projects I'm On filter includes unexpected results 

## Access requirements

You must have the following access to perform the steps in this article:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] plan</strong></td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe [!DNL Workfront] license</strong></td> 
   <td> <p>[!UICONTROL Plan] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Access level configurations</strong></td> 
   <td> <p>[!UICONTROL System administrator]</p> </td> 
  </tr> 
 </tbody> 
</table>

## Problem

The [!UICONTROL **Projects I'm On**] filter includes results that I would not expect, as I am not assigned or asssociated with those projects.

## Solution

The [!UICONTROL **Projects I'm On**] filter includes projects that contain the user in any of its [!UICONTROL **Project Details**] fields, including easily missed or automatically filled fields such as [!UICONTROL **Entered By**] or [!UICONTROL **Sponsor ID**]. To remove unwanted results, there are two possible solutions:

1. Check the [!UICONTROL **Project Details**] for each unexpected project included by the filter, and remove your name from all fields.

   OR

1. Try using a similar filter, such as [!UICONTROL **Projects I Own**], which only includes projects that are specifically assigned to you.

 For more information on using filters in [!DNL Workfront], see [Filters Overview](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/filters-overview.md).
