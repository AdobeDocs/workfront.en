---
filename: embed-external-web-page-dashboard
product-area: dashboards
navigation-topic: create-and-manage-dashboards
title: Embed an external web page in a dashboard
description: You can embed an external web page in a dashboard to provide access to related information from other systems within Adobe Workfront or to other Workfront pages.
---

# Embed an external web page in a dashboard

You can embed an external web page in a dashboard to provide access to related information from other systems within Adobe Workfront or to other Workfront pages.

For example, if your organization has a web-based document repository, wiki, or other content management system that contains project information that is regularly accessed through a URL, you can display that information into Workfront by creating an external page on a dashboard.

>[!IMPORTANT]
>
>For security reasons, some websites do not allow you to embed web pages as an iframe. If the web page you want to embed in a dashboard does not allow this, the page does not display in the dashboard. However, you can still access the external page by clicking the name of the dashboard.  
  
>To allow embedding for a website you own, work with your web administrator to adjust the `X-Frame-Options` setting. For more information, see [X-Frame-Options](https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers/X-Frame-Options).

## Access requirements

You must have the following:

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
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Reports, Dashboards, and Calendars</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to the dashboard</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects in Adobe Workfront</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your Workfront administrator.

## Prerequisites

You must create a dashboard before you can embed an external page in it.

For information on creating dashboards, see [Create a dashboard](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/create-dashboard.md).

## Embed an external page in a dashboard

>[!IMPORTANT]
>
>You can remove an External Page from a dashboard if it's no longer needed. However, you cannot delete an external page after it is created in Workfront. You can delete an external page only using the API. For more information, see [Remove an External Page from a dashboard in Adobe Workfront](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/remove-external-page-from-dashboard.md).

1. Locate the URL of the page to display in Workfront and copy the URL located in the address bar.

   >[!NOTE]
   >
   >If you are sharing URLs to Workfront objects, remember that some URLs expire over time. For example, document URLs expire after they have been opened. This is configured as a security measure, and by design they are considered as non-static URLs and should not be shared.

1. Click the Main Menu icon, then click Dashboards. 
1. To edit an existing dashboard, select the dashboard you want to embed the website page in, then click `Dashboard Actions`, and select `Edit` from the menu.  
   Or  
   To create a new dashboard, click `New Dashboard`.  
   For more information about creating a dashboard, see [Create a dashboard](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/create-dashboard.md).

1. Click `Add External Page`.

1. Specify a `Name` for the external page.
1. Specify a `Description`.
1. Paste the URL you copied earlier into the `URL` field.  
   You can specify the following types of URLs:

  * An https (encrypted) URL to a web page.  
    Only https (encrypted) pages load with the URL.  
  
  * A template URL that contains session information for a specific website.  
    For example: *https://localhost/?session={!$$SESSION}* 
    You must be logged into the specified website to display the External Page.  
    For information about how to obtain a SessionID from Workfront, see [API basics](../../../wf-api/general/api-basics.md).  
    Your Workfront administrator may configure your system preferences in a way that does not allow the use of session information in your external pages, for security reasons. In this case, the external page does not load on the dashboard.  
    For more information about system security preferences, see [Configure system security preferences](../../../administration-and-setup/manage-workfront/security/configure-security-preferences.md).  
    ![external_page_with_session_id_example.png](assets/external-page-with-session-id-example-350x134.png)

1. Click `Save`.  
   The page is automatically added to the dashboard. If future dashboards are created, the external page can be added. The external page will be found among the Available Reports.

## Update an external page in a dashboard

To update the information for an external page used in a dashboard:

1. Click the Main Menu icon, then click Dashboards. 
1. Select the dashboard that you want to update, then click `Edit` .

1. On the right side of the screen, locate the external page you want to update and click the `Edit` icon.  

1. In the `Edit External Page` dialog, update the fields you want to change, then click `Save`.
1. (Optional) Click the `Delete` icon ![](assets/delete.png) to remove the external page from the dashboard. For more information, see [Remove an External Page from a dashboard in Adobe Workfront](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/remove-external-page-from-dashboard.md). 
1. In the bottom-left corner, click `Save + Close`.

## View external pages in a report

You can view all external pages in Workfront in an External Page report.

1. Go to the Main Menu icon > Reports. 
1. Click `New Report` > select `External Page`.

1. (Optional) Update the View, Filters, or Groupings tabs of the report.

   For more information, see [Create a custom report](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md). 

1. Click `Save+Close`.

   You can view the name and the URL associated with the external pages in your system in the new report.

   ![](assets/external-page-report-name-url-columns-nwe-350x213.png)

