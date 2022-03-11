---
filename: embed-external-web-page-dashboard
product-area: dashboards
navigation-topic: create-and-manage-dashboards
title: Embed an external web page in a dashboard
description: You can embed an external web page in a dashboard to provide access to related information from other systems within Adobe Workfront or to other Workfront pages.
---

# Embed an external web page in a dashboard

You can embed an external web page in a dashboard to provide access to related information from other systems within `Adobe Workfront` or to other `Workfront` pages.

For example, if your organization has a web-based document repository, wiki, or other content management system that contains project information that is regularly accessed through a URL, you can display that information into `Workfront` by creating an external page on a dashboard.

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
   <td role="rowheader"><span>Adobe Workfront</span> plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><span>Adobe Workfront</span> license*</td> 
   <td> <p><span>Plan</span> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Reports, Dashboards, and Calendars</p> <p>Note: If you still don't have access, ask your <span>Workfront administrator</span> if they set additional restrictions in your access level. For information on how a <span>Workfront administrator</span> can change your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to the dashboard</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects in Adobe Workfront</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your `Workfront administrator`.

## Prerequisites

You must create a dashboard before you can embed an external page in it.

For information on creating dashboards, see [Create a dashboard](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/create-dashboard.md).

## Embed an external page in a dashboard

>[!IMPORTANT]
>
>You can remove an External Page from a dashboard if it's no longer needed. However, you cannot delete an external page after it is created in `Workfront`. You can delete an external page only using the API. For more information, see [Remove an External Page from a dashboard in Adobe Workfront](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/remove-external-page-from-dashboard.md).

<ol> 
 <li value="1">Locate the URL of the page to display in <span>Workfront</span> and copy the URL located in the address bar.<br><note type="note">
    If you are sharing URLs to 
   <span>Workfront</span> objects, remember that some URLs expire over time. For example, document URLs expire after they have been opened. This is configured as a security measure, and by design they are considered as non-static URLs and should not be shared.
  </note></li> 
 <li value="2"> Click the Main Menu icon, then click Dashboards. </li> 
 <li value="3">To edit an existing dashboard, select the dashboard you want to embed the website page in, then click <span class="bold">Dashboard Actions</span>, and select <span class="bold">Edit</span> from the menu.<br>Or<br>To create a new dashboard, click <span class="bold">New Dashboard</span>.<br>For more information about creating a dashboard, see <a href="../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/create-dashboard.md" class="MCXref xref">Create a dashboard</a>.</li> 
 <li value="4">Click <span class="bold">Add External Page</span>.<p></p></li> 
 <li value="5">Specify a <span class="bold">Name</span> for the external page.</li> 
 <li value="6">Specify a <span class="bold">Description</span>.</li> 
 <li value="7">Paste the URL you copied earlier into the <span class="bold">URL</span> field.<br>You can specify the following types of URLs:
  <ul>
   <li>An https (encrypted) URL to a web page.<br>Only https (encrypted) pages load with the URL.<br></li>
   <li>A template URL that contains session information for a specific website.<br>For example: <i>https://localhost/?session={!$$SESSION}</i><br>You must be logged into the specified website to display the External Page.<br>For information about how to obtain a SessionID from <span>Workfront</span>, see <a href="../../../wf-api/general/api-basics.md" class="MCXref xref">API basics</a>.<br>Your <span>Workfront administrator</span> may configure your system preferences in a way that does not allow the use of session information in your external pages, for security reasons. In this case, the external page does not load on the dashboard.<br>For more information about system security preferences, see <a href="../../../administration-and-setup/manage-workfront/security/configure-security-preferences.md" class="MCXref xref">Configure system security preferences</a>.<br><img src="assets/external-page-with-session-id-example-350x134.png" alt="external_page_with_session_id_example.png" style="width: 350;height: 134;"></li>
  </ul></li> 
 <li value="8">Click <span class="bold">Save</span>.<br>The page is automatically added to the dashboard. If future dashboards are created, the external page can be added. The external page will be found among the Available Reports.</li> 
</ol>

## Update an external page in a dashboard

To update the information for an external page used in a dashboard:

<ol> 
 <li value="1"> <p> Click the Main Menu icon, then click Dashboards. </p> </li> 
 <li value="2"> <p>Select the dashboard that you want to update, then click <span class="bold">Edit</span> .</p> <p>  </p> </li> 
 <li value="3"> <p>On the right side of the screen, locate the external page you want to update and click the <span class="bold">Edit</span> icon.<br></p> </li> 
 <li value="4"> <p>In the <span class="bold">Edit External Page</span> dialog, update the fields you want to change, then click <span class="bold">Save</span>.</p> </li> 
 <li value="5"> <p>(Optional)&nbsp;Click the <span class="bold">Delete</span> icon <img src="assets/delete.png"> to remove the external page from the dashboard. For more information, see <a href="../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/remove-external-page-from-dashboard.md" class="MCXref xref">Remove an External Page from a dashboard in&nbsp;Adobe Workfront</a>. </p> </li> 
 <li value="6"> <p>In the bottom-left corner, click <span class="bold">Save +&nbsp;Close</span>.</p> </li> 
</ol>

## View external pages in a report

You can view all external pages in `Workfront` in an External Page report.

<ol> 
 <li value="1"> Go to the Main Menu icon > Reports. </li> 
 <li value="2"> <p>Click <span class="bold">New Report</span> > select <span class="bold">External Page</span>.</p> <p>  </p> </li> 
 <li value="3"> <p>(Optional) Update the View, Filters, or Groupings tabs of the report. </p> <p>For more information, see <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md" class="MCXref xref">Create a custom report</a>. </p> </li> 
 <li value="4"> <p>Click <span class="bold">Save+Close</span>. </p> <p>You can view the name and the URL associated with the external pages in your system in the new report. </p> <p> <img src="assets/external-page-report-name-url-columns-nwe-350x213.png" style="width: 350;height: 213;"> </p> </li> 
</ol>

