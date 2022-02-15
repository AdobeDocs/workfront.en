


# Configurable access to functionality for each object type {#configurable-access-to-functionality-for-each-object-type}

The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview Sandbox environment.


This article explains what a *`Adobe Workfront administrator`* can allow for each object type, in each access level. It also explains what the default configuration is for each type of access level.


For information about all functionality available for an object type in each access level, see [Functionality available for each object type](functionality-available-for-each-object-type.md).


## Projects {#projects}

In each access level, you can configure the following options for *`projects`*:

<table style="width: 100%;mc-table-style: url('../../../Resources/TableStyles/TableStyle-HeaderRow.css');margin-left: 0;margin-right: auto;" class="TableStyle-TableStyle-HeaderRow" cellspacing="15"> 
 <col class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <col class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <thead> 
  <tr class="TableStyle-TableStyle-HeaderRow-Head-Header1"> 
   <th class="TableStyle-TableStyle-HeaderRow-HeadE-Column1-Header1">Access level</th> 
   <th class="TableStyle-TableStyle-HeaderRow-HeadD-Column1-Header1">Options</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">Planner </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> 
    <ul> 
     <li> <p><b>No access</b>: Blocks all access to <span class="mc-variable Snippet_Variables.Object variable varname">projects</span>.</p> </li> 
     <li> <p><b>View</b>: Allows view-only access to <span class="mc-variable Snippet_Variables.Object variable varname">projects</span>.</p> <p>To fine-tune this, you can configure the ability to share <span class="mc-variable Snippet_Variables.Object variable varname">projects</span>. Click the gear icon <img src="assets/gear-icon-in-access-levels.png"> on the <span style="font-weight: bold;" class="mc-variable Snippet_Variables.AccessLevelsViewOrEdit variable varname">View</span> button, then disable or enable the <b>Share</b> option (enabled by default).</p> </li> 
     <li> <p><b>Edit</b> (selected by default): Allows full editing access to <span class="mc-variable Snippet_Variables.Object variable varname">projects</span>.</p> <p>To fine-tune this, click the gear icon <img src="assets/gear-icon-in-access-levels.png"> on the <b><span class="mc-variable Snippet_Variables.AccessLevelsViewOrEdit variable varname">Edit</span></b> button, then disable or enable any of the following options. All of them are enabled by default.</p> 
      <ul> 
       <li> <p>Create</p> </li> 
       <li> <p>Copy</p> </li> 
       <li> <p>Delete</p> </li> 
       <li> <p>View</p> </li> 
       <li> <p>Share</p> </li> 
       <li> <p>Share system-wide</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">Worker </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> 
    <ul> 
     <li> <p><b>No access</b>: Blocks all access to <span class="mc-variable Snippet_Variables.Object variable varname">projects</span>.</p> </li> 
     <li> <p><b>View</b>: Allows <MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE">
        limited 
       </MadCap:conditionalText>view-only access to <span class="mc-variable Snippet_Variables.Object variable varname">projects</span>.</p> <p>To fine-tune this, you can configure the ability to share <span class="mc-variable Snippet_Variables.Object variable varname">projects</span>. Click the gear icon <img src="assets/gear-icon-in-access-levels.png"> on the <span style="font-weight: bold;" class="mc-variable Snippet_Variables.AccessLevelsViewOrEdit variable varname">View</span> button, then disable or enable the <b>Share</b> option (enabled by default).</p> </li> 
     <li> <p><b>Edit</b> (selected by default): Allows limited editing access to projects. To see how Edit access is limited in a Worker access level as compared to a Planner access level (which allows full Edit access to projects), see the section <a href="functionality-available-for-each-object-type.md#projects" class="MCXref xref">Projects</a> in the article <a href="functionality-available-for-each-object-type.md" class="MCXref xref">Functionality available for each object type</a>.</p> <p>To fine-tune this, you can configure the ability to share <span class="mc-variable Snippet_Variables.Object variable varname">projects</span>. Click the gear icon <img src="assets/gear-icon-in-access-levels.png"> on the <span style="font-weight: bold;" class="mc-variable Snippet_Variables.AccessLevelsViewOrEdit variable varname">Edit</span> button, then disable or enable the <b>Share</b> option (enabled by default).</p> </li> 
    </ul> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">Reviewer</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> 
    <ul> 
     <li> <p><b>No access</b>: Blocks all access to <span class="mc-variable Snippet_Variables.Object variable varname">projects</span>.</p> </li> 
     <li> <p><b>View</b> (selected by default): Allows view-only access to <span class="mc-variable Snippet_Variables.Object variable varname">projects</span>.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">Requestor</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> 
    <ul> 
     <li> <p><b>No access</b>: Blocks all access to <span class="mc-variable Snippet_Variables.Object variable varname">projects</span>.</p> </li> 
     <li> <p><b>View</b> (selected by default): Allows <MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE">
        limited 
       </MadCap:conditionalText>view-only access to <span class="mc-variable Snippet_Variables.Object variable varname">projects</span>.</p> <p>View access is limited because you can't fine-tune it to enable or disable project sharing.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyB-Column1-LightGray">External User</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyA-Column1-LightGray"> <p>Access to <span class="mc-variable Snippet_Variables.Object variable varname">projects</span> is not available. External users can use <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span> only to review and download documents and to see calendars that are shared with them.</p> </td> 
  </tr> 
 </tbody> 
</table>



## Tasks {#tasks}

In each access level, you can configure the following options for *`tasks`*:

<table style="width: 100%;mc-table-style: url('../../../Resources/TableStyles/TableStyle-HeaderRow.css');margin-left: 0;margin-right: auto;" class="TableStyle-TableStyle-HeaderRow" cellspacing="15"> 
 <col class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <col class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <thead> 
  <tr class="TableStyle-TableStyle-HeaderRow-Head-Header1"> 
   <th class="TableStyle-TableStyle-HeaderRow-HeadE-Column1-Header1">Access level</th> 
   <th class="TableStyle-TableStyle-HeaderRow-HeadD-Column1-Header1">Options</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">Planner </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> 
    <ul> 
     <li> <p><b>No access</b>: Blocks all access to <span class="mc-variable Snippet_Variables.Object variable varname">tasks</span>.</p> </li> 
     <li> <p><b>View</b>: Allows view-only access to <span class="mc-variable Snippet_Variables.Object variable varname">tasks</span>.</p> <p>To fine-tune this, you can configure the ability to share <span class="mc-variable Snippet_Variables.Object variable varname">tasks</span>. Click the gear icon <img src="assets/gear-icon-in-access-levels.png"> on the <span style="font-weight: bold;" class="mc-variable Snippet_Variables.AccessLevelsViewOrEdit variable varname">View</span> button, then disable or enable the <b>Share</b> option (enabled by default).</p> </li> 
     <li> <p><b>Edit</b> (selected by default): Allows full editing access to <span class="mc-variable Snippet_Variables.Object variable varname">tasks</span>.</p> <p>To fine-tune this, click the gear icon <img src="assets/gear-icon-in-access-levels.png"> on the <b><span class="mc-variable Snippet_Variables.AccessLevelsViewOrEdit variable varname">Edit</span></b> button, then disable or enable any of the following options. All of them are enabled by default.</p> 
      <ul> 
       <li> <p>Create</p> </li> 
       <li> <p>Delete</p> </li> 
       <li> <p>Share</p> </li> 
       <li> <p>Share system-wide</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">Worker </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> 
    <ul> 
     <li> <p><b>No access</b>: Blocks all access to <span class="mc-variable Snippet_Variables.Object variable varname">tasks</span>.</p> </li> 
     <li> <p><b>View</b>: Allows view-only access to <span class="mc-variable Snippet_Variables.Object variable varname">tasks</span>.</p> <p>To fine-tune this, you can configure the ability to share <span class="mc-variable Snippet_Variables.Object variable varname">tasks</span>. Click the gear icon <img src="assets/gear-icon-in-access-levels.png"> on the <span style="font-weight: bold;" class="mc-variable Snippet_Variables.AccessLevelsViewOrEdit variable varname">View</span> button, then disable or enable the <b>Share</b> option (enabled by default).</p> </li> 
     <li> <p><b>Edit</b> (selected by default): Allows full editing access to <span class="mc-variable Snippet_Variables.Object variable varname">tasks</span>.</p> <p>To fine-tune this, click the gear icon <img src="assets/gear-icon-in-access-levels.png"> on the <b><span class="mc-variable Snippet_Variables.AccessLevelsViewOrEdit variable varname">Edit</span></b> button, then disable or enable any of the following options. All of them are enabled by default.</p> 
      <ul> 
       <li> <p>Create</p> </li> 
       <li> <p>Delete</p> </li> 
       <li> <p>Share</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">Reviewer</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> 
    <ul> 
     <li> <p><b>No access</b>: Blocks all access to <span class="mc-variable Snippet_Variables.Object variable varname">tasks</span>.</p> </li> 
     <li> <p><b>View</b> (selected by default): Allows view-only access to <span class="mc-variable Snippet_Variables.Object variable varname">tasks</span>.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">Requestor</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> 
    <ul> 
     <li> <p><b>No access</b>: Blocks all access to <span class="mc-variable Snippet_Variables.Object variable varname">tasks</span>.</p> </li> 
     <li> <p><b>View</b> (selected by default): Allows <MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE">
        limited 
       </MadCap:conditionalText>view-only access to <span class="mc-variable Snippet_Variables.Object variable varname">tasks</span>.</p> <p>View access is limited because you can't fine-tune it to enable or disable project sharing.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyB-Column1-LightGray">External User</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyA-Column1-LightGray"> <p>Access to <span class="mc-variable Snippet_Variables.Object variable varname">tasks</span> is not available. External users can use <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span> only to review and download documents and to see calendars that are shared with them.</p> </td> 
  </tr> 
 </tbody> 
</table>



## Issues {#issues}

In each access level, you can configure the following options for *`issues`*:

<table style="width: 100%;mc-table-style: url('../../../Resources/TableStyles/TableStyle-HeaderRow.css');margin-left: 0;margin-right: auto;" class="TableStyle-TableStyle-HeaderRow" cellspacing="15"> 
 <col class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <col class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <thead> 
  <tr class="TableStyle-TableStyle-HeaderRow-Head-Header1"> 
   <th class="TableStyle-TableStyle-HeaderRow-HeadE-Column1-Header1">Access level</th> 
   <th class="TableStyle-TableStyle-HeaderRow-HeadD-Column1-Header1">Options</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">Planner </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> 
    <ul> 
     <li> <p><b>No access</b>: Blocks all access to <span class="mc-variable Snippet_Variables.Object variable varname">issues</span>.</p> </li> 
     <li> <p><b>View</b>: Allows view-only access to <span class="mc-variable Snippet_Variables.Object variable varname">issues</span>.</p> <p>To fine-tune this, you can configure the ability to share <span class="mc-variable Snippet_Variables.Object variable varname">issues</span>. Click the gear icon <img src="assets/gear-icon-in-access-levels.png"> on the <span style="font-weight: bold;" class="mc-variable Snippet_Variables.AccessLevelsViewOrEdit variable varname">View</span> button, then disable or enable the <b>Share</b> option (enabled by default).</p> </li> 
     <li> <p><b>Edit</b> (selected by default): Allows full editing access to <span class="mc-variable Snippet_Variables.Object variable varname">issues</span>.</p> <p>To fine-tune this, click the gear icon <img src="assets/gear-icon-in-access-levels.png"> on the <b><span class="mc-variable Snippet_Variables.AccessLevelsViewOrEdit variable varname">Edit</span></b> button, then disable or enable any of the following options. All of them are enabled by default.</p> 
      <ul> 
       <li> <p>Create</p> </li> 
       <li> <p>Delete</p> </li> 
       <li> <p>Share</p> </li> 
       <li> <p>Share system-wide</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">Worker </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> 
    <ul> 
     <li> <p><b>No access</b>: Blocks all access to <span class="mc-variable Snippet_Variables.Object variable varname">issues</span>.</p> </li> 
     <li> <p><b>View</b>: Allows view-only access to <span class="mc-variable Snippet_Variables.Object variable varname">issues</span>.</p> <p>To fine-tune this, you can configure the ability to share <span class="mc-variable Snippet_Variables.Object variable varname">issues</span>. Click the gear icon <img src="assets/gear-icon-in-access-levels.png"> on the <span style="font-weight: bold;" class="mc-variable Snippet_Variables.AccessLevelsViewOrEdit variable varname">View</span> button, then disable or enable the <b>Share</b> option (enabled by default).</p> </li> 
     <li> <p><b>Edit</b> (selected by default): Allows full editing access to <span class="mc-variable Snippet_Variables.Object variable varname">issues</span>.</p> <p>To fine-tune this, click the gear icon <img src="assets/gear-icon-in-access-levels.png"> on the <b><span class="mc-variable Snippet_Variables.AccessLevelsViewOrEdit variable varname">Edit</span></b> button, then disable or enable any of the following options. All of them are enabled by default.</p> 
      <ul> 
       <li> <p>Create</p> </li> 
       <li> <p>Delete</p> </li> 
       <li> <p>Share</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">Reviewer</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> 
    <ul> 
     <li> <p><b>No access</b>: Blocks all access to <span class="mc-variable Snippet_Variables.Object variable varname">issues</span>.</p> </li> 
     <li> <p><b>View</b>: Allows view-only access to <span class="mc-variable Snippet_Variables.Object variable varname">issues</span>.</p> <p>To fine-tune this, you can configure the ability to share <span class="mc-variable Snippet_Variables.Object variable varname">issues</span>. Click the gear icon <img src="assets/gear-icon-in-access-levels.png"> on the <span style="font-weight: bold;" class="mc-variable Snippet_Variables.AccessLevelsViewOrEdit variable varname">View</span> button, then disable or enable the <b>Share</b> option (enabled by default).</p> </li> 
     <li> <p><b>Edit</b> (selected by default): Allows full editing access to <span class="mc-variable Snippet_Variables.Object variable varname">issues</span>.</p> <p>To fine-tune this, click the gear icon <img src="assets/gear-icon-in-access-levels.png"> on the <b><span class="mc-variable Snippet_Variables.AccessLevelsViewOrEdit variable varname">Edit</span></b> button, then disable or enable any of the following options. All of them are enabled by default.</p> 
      <ul> 
       <li> <p>Create</p> </li> 
       <li> <p>Delete</p> </li> 
       <li> <p>Share</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">Requestor</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> 
    <ul> 
     <li> <p><b>No access</b>: Blocks all access to <span class="mc-variable Snippet_Variables.Object variable varname">issues</span>.</p> </li> 
     <li> <p><b>View</b>: Allows view-only access to <span class="mc-variable Snippet_Variables.Object variable varname">issues</span>.</p> <p>To fine-tune this, you can configure the ability to share <span class="mc-variable Snippet_Variables.Object variable varname">issues</span>. Click the gear icon <img src="assets/gear-icon-in-access-levels.png"> on the <span style="font-weight: bold;" class="mc-variable Snippet_Variables.AccessLevelsViewOrEdit variable varname">View</span> button, then disable or enable the <b>Share</b> option (enabled by default).</p> </li> 
     <li> <p><b>Edit</b> (selected by default): Allows full editing access to <span class="mc-variable Snippet_Variables.Object variable varname">issues</span>.</p> <p>To fine-tune this, click the gear icon <img src="assets/gear-icon-in-access-levels.png"> on the <b><span class="mc-variable Snippet_Variables.AccessLevelsViewOrEdit variable varname">Edit</span></b> button, then disable or enable any of the following options. All of them are enabled by default.</p> 
      <ul> 
       <li> <p>Create</p> </li> 
       <li> <p>Delete</p> </li> 
       <li> <p>Share</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyB-Column1-LightGray">External User</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyA-Column1-LightGray"> <p>Access to <span class="mc-variable Snippet_Variables.Object variable varname">issues</span> is not available. External users can use <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span> only to review and download documents and to see calendars that are shared with them.</p> </td> 
  </tr> 
 </tbody> 
</table>



## Portfolios {#portfolios}

In each access level, you can configure the following options for *`portfolios`*:

<table style="width: 100%;mc-table-style: url('../../../Resources/TableStyles/TableStyle-HeaderRow.css');margin-left: 0;margin-right: auto;" class="TableStyle-TableStyle-HeaderRow" cellspacing="15"> 
 <col class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <col class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <thead> 
  <tr class="TableStyle-TableStyle-HeaderRow-Head-Header1"> 
   <th class="TableStyle-TableStyle-HeaderRow-HeadE-Column1-Header1">Access level</th> 
   <th class="TableStyle-TableStyle-HeaderRow-HeadD-Column1-Header1">Options</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">Planner </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> 
    <ul> 
     <li> <p><b>No access</b>: Blocks all access to <span class="mc-variable Snippet_Variables.Object variable varname">portfolios</span>.</p> </li> 
     <li> <p><b>View</b>: Allows view-only access to <span class="mc-variable Snippet_Variables.Object variable varname">portfolios</span>.</p> <p>To fine-tune this, you can configure the ability to share <span class="mc-variable Snippet_Variables.Object variable varname">portfolios</span>. Click the gear icon <img src="assets/gear-icon-in-access-levels.png"> on the <span style="font-weight: bold;" class="mc-variable Snippet_Variables.AccessLevelsViewOrEdit variable varname">View</span> button, then disable or enable the <b>Share</b> option (enabled by default).</p> </li> 
     <li> <p><b>Edit</b> (selected by default): Allows full editing access to <span class="mc-variable Snippet_Variables.Object variable varname">portfolios</span>.</p> <p>To fine-tune this, click the gear icon <img src="assets/gear-icon-in-access-levels.png"> on the <b><span class="mc-variable Snippet_Variables.AccessLevelsViewOrEdit variable varname">Edit</span></b> button, then disable or enable any of the following options. All of them are enabled by default.</p> 
      <ul> 
       <li> <p>Create</p> </li> 
       <li> <p>Delete</p> </li> 
       <li> <p>Share</p> </li> 
       <li> <p>Share system-wide</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">Worker </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> 
    <ul> 
     <li> <p><b>No access</b>: Blocks all access to <span class="mc-variable Snippet_Variables.Object variable varname">portfolios</span>.</p> </li> 
     <li> <p><b>View</b> (selected by default): Allows view-only access to <span class="mc-variable Snippet_Variables.Object variable varname">portfolios</span>.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">Reviewer</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> 
    <ul> 
     <li> <p><b>No access</b>: Blocks all access to <span class="mc-variable Snippet_Variables.Object variable varname">portfolios</span>.</p> </li> 
     <li> <p><b>View</b> (selected by default): Allows view-only access to <span class="mc-variable Snippet_Variables.Object variable varname">portfolios</span>.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">Requestor</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> <p>Access to <span class="mc-variable Snippet_Variables.Object variable varname">portfolios</span> is not available.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyB-Column1-LightGray">External User</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyA-Column1-LightGray"> <p>Access to <span class="mc-variable Snippet_Variables.Object variable varname">portfolios</span> is not available. External users can use <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span> only to review and download documents and to see calendars that are shared with them.</p> </td> 
  </tr> 
 </tbody> 
</table>



## Programs {#programs}

In each access level, you can configure the following options for *`programs`*:

<table style="width: 100%;mc-table-style: url('../../../Resources/TableStyles/TableStyle-HeaderRow.css');margin-left: 0;margin-right: auto;" class="TableStyle-TableStyle-HeaderRow" cellspacing="15"> 
 <col class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <col class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <thead> 
  <tr class="TableStyle-TableStyle-HeaderRow-Head-Header1"> 
   <th class="TableStyle-TableStyle-HeaderRow-HeadE-Column1-Header1">Access level</th> 
   <th class="TableStyle-TableStyle-HeaderRow-HeadD-Column1-Header1">Options</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">Planner </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> 
    <ul> 
     <li> <p><b>No access</b>: Blocks all access to <span class="mc-variable Snippet_Variables.Object variable varname">programs</span>.</p> </li> 
     <li> <p><b>View</b>: Allows view-only access to <span class="mc-variable Snippet_Variables.Object variable varname">programs</span>.</p> <p>To fine-tune this, you can configure the ability to share <span class="mc-variable Snippet_Variables.Object variable varname">programs</span>. Click the gear icon <img src="assets/gear-icon-in-access-levels.png"> on the <span style="font-weight: bold;" class="mc-variable Snippet_Variables.AccessLevelsViewOrEdit variable varname">View</span> button, then disable or enable the <b>Share</b> option (enabled by default).</p> </li> 
     <li> <p><b>Edit</b> (selected by default): Allows full editing access to <span class="mc-variable Snippet_Variables.Object variable varname">programs</span>.</p> <p>To fine-tune this, click the gear icon <img src="assets/gear-icon-in-access-levels.png"> on the <b><span class="mc-variable Snippet_Variables.AccessLevelsViewOrEdit variable varname">Edit</span></b> button, then disable or enable any of the following options. All of them are enabled by default.</p> 
      <ul> 
       <li> <p>Create</p> </li> 
       <li> <p>Delete</p> </li> 
       <li> <p>Share</p> </li> 
       <li> <p>Share system-wide</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">Worker </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> 
    <ul> 
     <li> <p><b>No access</b>: Blocks all access to <span class="mc-variable Snippet_Variables.Object variable varname">programs</span>.</p> </li> 
     <li> <p><b>View</b> (selected by default): Allows view-only access to <span class="mc-variable Snippet_Variables.Object variable varname">programs</span>.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">Reviewer</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> 
    <ul> 
     <li> <p><b>No access</b>: Blocks all access to <span class="mc-variable Snippet_Variables.Object variable varname">programs</span>.</p> </li> 
     <li> <p><b>View</b> (selected by default): Allows view-only access to <span class="mc-variable Snippet_Variables.Object variable varname">programs</span>.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">Requestor</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> <p>Access to <span class="mc-variable Snippet_Variables.Object variable varname">programs</span> is not available.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyB-Column1-LightGray">External User</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyA-Column1-LightGray"> <p>Access to <span class="mc-variable Snippet_Variables.Object variable varname">programs</span> is not available. External users can use <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span> only to review and download documents and to see calendars that are shared with them.</p> </td> 
  </tr> 
 </tbody> 
</table>



## Reports, dashboards, and calendars {#reports-dashboards-and-calendars}

In each access level, you can configure the following options for *`reports, dashboards, and calendars`*:

<table style="width: 100%;mc-table-style: url('../../../Resources/TableStyles/TableStyle-HeaderRow.css');margin-left: 0;margin-right: auto;" class="TableStyle-TableStyle-HeaderRow" cellspacing="15"> 
 <col class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <col class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <thead> 
  <tr class="TableStyle-TableStyle-HeaderRow-Head-Header1"> 
   <th class="TableStyle-TableStyle-HeaderRow-HeadE-Column1-Header1">Access level</th> 
   <th class="TableStyle-TableStyle-HeaderRow-HeadD-Column1-Header1">Options</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">Planner </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> 
    <ul> 
     <li> <p><b>No access</b>: Blocks all access to <span class="mc-variable Snippet_Variables.Object variable varname">reports, dashboards, and calendars</span>.</p> </li> 
     <li> <p><b>View</b>: Allows view-only access to <span class="mc-variable Snippet_Variables.Object variable varname">reports, dashboards, and calendars</span>.</p> <p>To fine-tune this, click the gear icon <img src="assets/gear-icon-in-access-levels.png"> on the <b>Edit</b> button), then disable or enable any of the following actions. Both of them are enabled by default:</p> 
      <ul> 
       <li> <p>View Built-In Reports</p> </li> 
       <li> <p>Share</p> </li> 
      </ul> </li> 
     <li> <p><b>Edit</b> (selected by default): Allows full editing access to <span class="mc-variable Snippet_Variables.Object variable varname">reports, dashboards, and calendars</span>.</p> <p>To fine-tune this, click the gear icon <img src="assets/gear-icon-in-access-levels.png"> on the <b><span class="mc-variable Snippet_Variables.AccessLevelsViewOrEdit variable varname">Edit</span></b> button, then disable or enable any of the following options. All of them are enabled by default.</p> 
      <ul> 
       <li> <p>Create</p> </li> 
       <li> <p>Delete</p> </li> 
       <li> <p>View Built-In Reports</p> </li> 
       <li> <p>Share</p> </li> 
       <li> <p>Share Reports Publicly (externally)</p> </li> 
       <li> <p>Share system-wide</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">Worker </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> 
    <ul> 
     <li> <p><b>No access</b>: Blocks all access to <span class="mc-variable Snippet_Variables.Object variable varname">programs</span>.</p> </li> 
     <li> <p><b>View</b> (selected by default): Allows view-only access to <span class="mc-variable Snippet_Variables.Object variable varname">reports, dashboards, and calendars</span>.</p> <p>To fine-tune this, click the gear icon <img src="assets/gear-icon-in-access-levels.png"> on the <b>Edit</b> button, then disable or enable any of the following actions. Both of them are enabled by default:</p> 
      <ul> 
       <li> <p>View Built-In Reports</p> </li> 
       <li> <p>Share</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">Reviewer</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> 
    <ul> 
     <li> <p><b>No access</b>: Blocks all access to <span class="mc-variable Snippet_Variables.Object variable varname">reports, dashboards, and calendars</span>.</p> </li> 
     <li> <p><b>View</b> (selected by default): Allows view-only access to <span class="mc-variable Snippet_Variables.Object variable varname">reports, dashboards, and calendars</span>.</p> <p>To fine-tune this, click the gear icon <img src="assets/gear-icon-in-access-levels.png"> on the <b>Edit</b> button, then disable or enable any of the following actions. Only the Share option is enabled by default.</p> 
      <ul> 
       <li> <p>View Built-In Reports</p> </li> 
       <li> <p>Share</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">Requestor</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> 
    <ul> 
     <li> <p><b>No access</b>: Blocks all access to <span class="mc-variable Snippet_Variables.Object variable varname">reports, dashboards, and calendars</span>.</p> </li> 
     <li> <p><b>View</b> (selected by default): Allows view-only access to reports, dashboards, and calendars that have been shared with them.</p> <p>To fine-tune this, you can configure the ability to view built-in reports. Click the gear icon <img src="assets/gear-icon-in-access-levels.png"> on the <b>View</b> button, then disable or enable <b>View Built-in Reports </b>(disabled by default).</p> </li> 
    </ul> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyB-Column1-LightGray">External User</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyA-Column1-LightGray"> <p>Access to <span class="mc-variable Snippet_Variables.Object variable varname">reports, dashboards, and calendars</span> is not available. External users can use <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span> only to review and download documents and to see calendars that are shared with them.</p> </td> 
  </tr> 
 </tbody> 
</table>



## Filters, views, and groupings {#filters-views-and-groupings}

In each access level, you can configure the following options for *`filters, views, and groupings`*:

<table style="width: 100%;mc-table-style: url('../../../Resources/TableStyles/TableStyle-HeaderRow.css');margin-left: 0;margin-right: auto;" class="TableStyle-TableStyle-HeaderRow" cellspacing="15"> 
 <col class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <col class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <thead> 
  <tr class="TableStyle-TableStyle-HeaderRow-Head-Header1"> 
   <th class="TableStyle-TableStyle-HeaderRow-HeadE-Column1-Header1">Access level</th> 
   <th class="TableStyle-TableStyle-HeaderRow-HeadD-Column1-Header1">Options</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">Planner </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> 
    <ul> 
     <li> <p><b>View</b>: Allows view-only access to <span class="mc-variable Snippet_Variables.Object variable varname">filters, views, and groupings</span>.</p> <p>To fine-tune this, you can configure the ability to share <span class="mc-variable Snippet_Variables.Object variable varname">filters, views, and groupings</span>. Click the gear icon <img src="assets/gear-icon-in-access-levels.png"> on the <span style="font-weight: bold;" class="mc-variable Snippet_Variables.AccessLevelsViewOrEdit variable varname">View</span> button, then disable or enable the <b>Share</b> option (enabled by default).</p> </li> 
     <li> <p><b>Edit</b> (selected by default): Allows full editing access to <span class="mc-variable Snippet_Variables.Object variable varname">filters, views, and groupings</span>.</p> <p>To fine-tune this, click the gear icon <img src="assets/gear-icon-in-access-levels.png"> on the <b><span class="mc-variable Snippet_Variables.AccessLevelsViewOrEdit variable varname">Edit</span></b> button, then disable or enable any of the following options. All of them are enabled by default.</p> 
      <ul> 
       <li> <p>Create</p> </li> 
       <li> <p>Delete</p> </li> 
       <li> <p>Share</p> </li> 
       <li> <p>Share system-wide</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">Worker </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> 
    <ul> 
     <li> <p><b>View</b>: Allows view-only access to <span class="mc-variable Snippet_Variables.Object variable varname">filters, views, and groupings</span>.</p> <p>To fine-tune this, you can configure the ability to share <span class="mc-variable Snippet_Variables.Object variable varname">filters, views, and groupings</span>. Click the gear icon <img src="assets/gear-icon-in-access-levels.png"> on the <span style="font-weight: bold;" class="mc-variable Snippet_Variables.AccessLevelsViewOrEdit variable varname">View</span> button, then disable or enable the <b>Share</b> option (enabled by default).</p> </li> 
     <li> <p><b>Edit</b> (selected by default): Allows full editing access to <span class="mc-variable Snippet_Variables.Object variable varname">filters, views, and groupings</span>.</p> <p>To fine-tune this, click the gear icon <img src="assets/gear-icon-in-access-levels.png"> on the <b><span class="mc-variable Snippet_Variables.AccessLevelsViewOrEdit variable varname">Edit</span></b> button, then disable or enable any of the following options. All of them are enabled by default.</p> 
      <ul> 
       <li> <p>Create</p> </li> 
       <li> <p>Delete</p> </li> 
       <li> <p>Share</p> </li> 
       <li> <p>Share system-wide</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">Reviewer</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> 
    <ul> 
     <li> <p><b>View</b>: Allows view-only access to <span class="mc-variable Snippet_Variables.Object variable varname">filters, views, and groupings</span>.</p> <p>To fine-tune this, you can configure the ability to share <span class="mc-variable Snippet_Variables.Object variable varname">filters, views, and groupings</span>. Click the gear icon <img src="assets/gear-icon-in-access-levels.png"> on the <span style="font-weight: bold;" class="mc-variable Snippet_Variables.AccessLevelsViewOrEdit variable varname">View</span> button, then disable or enable the <b>Share</b> option (enabled by default).</p> </li> 
     <li> <p><b>Edit</b> (selected by default): Allows full editing access to <span class="mc-variable Snippet_Variables.Object variable varname">filters, views, and groupings</span>.</p> <p>To fine-tune this, click the gear icon <img src="assets/gear-icon-in-access-levels.png"> on the <b><span class="mc-variable Snippet_Variables.AccessLevelsViewOrEdit variable varname">Edit</span></b> button, then disable or enable any of the following options. All of them are enabled by default.</p> 
      <ul> 
       <li> <p>Create</p> </li> 
       <li> <p>Delete</p> </li> 
       <li> <p>Share</p> </li> 
       <li> <p>Share system-wide</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">Requestor</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> 
    <ul> 
     <li> <p><b>View</b>: Allows view-only access to <span class="mc-variable Snippet_Variables.Object variable varname">filters, views, and groupings</span>.</p> <p>To fine-tune this, you can configure the ability to share <span class="mc-variable Snippet_Variables.Object variable varname">filters, views, and groupings</span>. Click the gear icon <img src="assets/gear-icon-in-access-levels.png"> on the <span style="font-weight: bold;" class="mc-variable Snippet_Variables.AccessLevelsViewOrEdit variable varname">View</span> button, then disable or enable the <b>Share</b> option (enabled by default).</p> </li> 
     <li> <p><b>Edit</b> (selected by default): Allows full editing access to <span class="mc-variable Snippet_Variables.Object variable varname">filters, views, and groupings</span>.</p> <p>To fine-tune this, click the gear icon <img src="assets/gear-icon-in-access-levels.png"> on the <b>Edit</b> button, then disable or enable any of the following actions .All of the options are selected by default except for the <b>Share</b> option.</p> 
      <ul> 
       <li> <p>Create</p> </li> 
       <li> <p>Delete</p> </li> 
       <li> <p>Share</p> </li> 
       <li> <p>Share system-wide</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyB-Column1-LightGray">External User</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyA-Column1-LightGray"> <p>Access to <span class="mc-variable Snippet_Variables.Object variable varname">filters, views, and groupings</span> is not available. External users can use <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span> only to review and download documents and to see calendars that are shared with them.</p> </td> 
  </tr> 
 </tbody> 
</table>



## Documents {#documents}

In each access level, you can configure the following options for *`documents`*:

<table style="width: 100%;mc-table-style: url('../../../Resources/TableStyles/TableStyle-HeaderRow.css');margin-left: 0;margin-right: auto;" class="TableStyle-TableStyle-HeaderRow" cellspacing="15"> 
 <col class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <col class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <thead> 
  <tr class="TableStyle-TableStyle-HeaderRow-Head-Header1"> 
   <th class="TableStyle-TableStyle-HeaderRow-HeadE-Column1-Header1">Access level</th> 
   <th class="TableStyle-TableStyle-HeaderRow-HeadD-Column1-Header1">Options</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">Planner </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> 
    <ul> 
     <li> <p><b>No access</b>: Blocks all access to <span class="mc-variable Snippet_Variables.Object variable varname">documents</span>.</p> </li> 
     <li> <p><b>View</b>: Allows view-only access to <span class="mc-variable Snippet_Variables.Object variable varname">documents</span>.</p> <p>To fine-tune this, you can configure the ability to share <span class="mc-variable Snippet_Variables.Object variable varname">documents</span>. Click the gear icon <img src="assets/gear-icon-in-access-levels.png"> on the <span style="font-weight: bold;" class="mc-variable Snippet_Variables.AccessLevelsViewOrEdit variable varname">View</span> button, then disable or enable the <b>Share</b> option (enabled by default).</p> </li> 
     <li> <p><b>Edit</b> (selected by default): Allows full editing access to <span class="mc-variable Snippet_Variables.Object variable varname">documents</span>.</p> <p>To fine-tune this, click the gear icon <img src="assets/gear-icon-in-access-levels.png"> on the <b><span class="mc-variable Snippet_Variables.AccessLevelsViewOrEdit variable varname">Edit</span></b> button, then disable or enable any of the following options. All of them are enabled by default.</p> 
      <ul> 
       <li> <p>Create</p> </li> 
       <li> <p>Delete</p> </li> 
       <li> <p>Share</p> </li> 
       <li> <p>Share Documents Publicly (externally)</p> </li> 
       <li> <p>Share system-wide</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">Worker </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> 
    <ul> 
     <li> <p><b>No access</b>: Blocks all access to <span class="mc-variable Snippet_Variables.Object variable varname">documents</span>.</p> </li> 
     <li> <p><b>View</b>: Allows view-only access to <span class="mc-variable Snippet_Variables.Object variable varname">documents</span>.</p> <p>To fine-tune this, you can configure the ability to share <span class="mc-variable Snippet_Variables.Object variable varname">documents</span>. Click the gear icon <img src="assets/gear-icon-in-access-levels.png"> on the <span style="font-weight: bold;" class="mc-variable Snippet_Variables.AccessLevelsViewOrEdit variable varname">View</span> button, then disable or enable the <b>Share</b> option (enabled by default).</p> </li> 
     <li> <p><b>Edit</b> (selected by default): Allows full editing access to <span class="mc-variable Snippet_Variables.Object variable varname">documents</span>.</p> <p>To fine-tune this, click the gear icon <img src="assets/gear-icon-in-access-levels.png"> on the <b><span class="mc-variable Snippet_Variables.AccessLevelsViewOrEdit variable varname">Edit</span></b> button, then disable or enable any of the following options. All of them are enabled by default.</p> 
      <ul> 
       <li> <p>Create</p> </li> 
       <li> <p>Delete</p> </li> 
       <li> <p>Share</p> </li> 
       <li> <p>Share Documents Publicly (externally)</p> </li> 
       <li> <p>Share system-wide</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">Reviewer</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> 
    <ul> 
     <li> <p><b>No access</b>: Blocks all access to <span class="mc-variable Snippet_Variables.Object variable varname">documents</span>.</p> </li> 
     <li> <p><b>View</b>: Allows view-only access to <span class="mc-variable Snippet_Variables.Object variable varname">documents</span>.</p> <p>To fine-tune this, you can configure the ability to share <span class="mc-variable Snippet_Variables.Object variable varname">documents</span>. Click the gear icon <img src="assets/gear-icon-in-access-levels.png"> on the <span style="font-weight: bold;" class="mc-variable Snippet_Variables.AccessLevelsViewOrEdit variable varname">View</span> button, then disable or enable the <b>Share</b> option (enabled by default).</p> </li> 
     <li> <p><b>Edit</b> (selected by default): Allows full editing access to <span class="mc-variable Snippet_Variables.Object variable varname">documents</span>.</p> <p>To fine-tune this, click the gear icon <img src="assets/gear-icon-in-access-levels.png"> on the <b>Edit</b> button, then disable or enable any of the following actions. All of them are enabled by default except for the last two, <b>Share Documents Publicly</b> and <b>Share system-wide</b>.</p> 
      <ul> 
       <li> <p>Create</p> </li> 
       <li> <p>Delete</p> </li> 
       <li> <p>Share</p> </li> 
       <li> <p>Share Documents Publicly (externally)</p> </li> 
       <li> <p>Share system-wide</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">Requestor</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> 
    <ul> 
     <li> <p><b>No access</b>: Blocks all access to <span class="mc-variable Snippet_Variables.Object variable varname">documents</span>.</p> </li> 
     <li> <p><b>View</b>: Allows view-only access to <span class="mc-variable Snippet_Variables.Object variable varname">documents</span>.</p> <p>To fine-tune this, you can configure the ability to share <span class="mc-variable Snippet_Variables.Object variable varname">documents</span>. Click the gear icon <img src="assets/gear-icon-in-access-levels.png"> on the <span style="font-weight: bold;" class="mc-variable Snippet_Variables.AccessLevelsViewOrEdit variable varname">View</span> button, then disable or enable the <b>Share</b> option (enabled by default).</p> </li> 
     <li> <p><b>Edit</b> (selected by default): Allows full editing access to <span class="mc-variable Snippet_Variables.Object variable varname">documents</span>.</p> <p>To fine-tune this, click the gear icon <img src="assets/gear-icon-in-access-levels.png"> on the <b><span class="mc-variable Snippet_Variables.AccessLevelsViewOrEdit variable varname">Edit</span></b> button, then disable or enable any of the following options. All of them are enabled by default.</p> 
      <ul> 
       <li> <p>Create</p> </li> 
       <li> <p>Delete</p> </li> 
       <li> <p>Share</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyB-Column1-LightGray">External User</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyA-Column1-LightGray"> <p>Access to documents is not configurable in this access level. But external users can use <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span> to view, review, and download documents.</p> </td> 
  </tr> 
 </tbody> 
</table>



## Users {#users}

In each access level, you can configure the following options for *`users`*:

<table style="width: 100%;mc-table-style: url('../../../Resources/TableStyles/TableStyle-HeaderRow.css');margin-left: 0;margin-right: auto;" class="TableStyle-TableStyle-HeaderRow" cellspacing="15"> 
 <col class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <col class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <thead> 
  <tr class="TableStyle-TableStyle-HeaderRow-Head-Header1"> 
   <th class="TableStyle-TableStyle-HeaderRow-HeadE-Column1-Header1">Access level</th> 
   <th class="TableStyle-TableStyle-HeaderRow-HeadD-Column1-Header1">Options</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">Planner </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> 
    <ul> 
     <li> <p><b>View</b>: Allows view-only access to <span class="mc-variable Snippet_Variables.Object variable varname">users</span>.</p> <p>To fine-tune this, you can configure the ability to view users' contact information. Click the gear icon <img src="assets/gear-icon-in-access-levels.png"> on the <b>View</b> button, then disable or enable the <b>View Contact Info</b> option (enabled by default).</p> </li> 
     <li> <p><b>Edit</b> (selected by default): Allows full editing access to <span class="mc-variable Snippet_Variables.Object variable varname">users</span>.</p> <p>To fine-tune this, click the gear icon <img src="assets/gear-icon-in-access-levels.png"> on the <b>Edit</b> button, then disable or enable any of the following actions. Only the first two options, <b>Create</b> and <b>Delete</b>, are enabled by default.</p> 
      <ul> 
       <li> <p>Create</p> </li> 
       <li> <p>Delete</p> </li> 
       <li>User Admin (All Users)</li> 
       <li> <p>User Admin (Group Users)</p> </li> 
      </ul> <p>For information about the two User Admin options, see the section <a href="grant-access-other-users.md#access-to-edit" class="MCXref xref">Configure users’ access to edit users using a custom access level</a>in the article <a href="grant-access-other-users.md" class="MCXref xref">Grant access to users</a>.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">Worker </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> 
    <ul> 
     <li> <p><b>View</b> (only option available): Allows view-only access to <span class="mc-variable Snippet_Variables.Object variable varname">users</span>.</p> <p>To fine-tune this, you can configure the ability to view users' contact information. Click the gear icon <img src="assets/gear-icon-in-access-levels.png"> on the <b>View</b> button, then disable or enable the <b>View Contact Info</b> option (enabled by default).</p> </li> 
    </ul> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">Reviewer</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> 
    <ul> 
     <li> <p><b>View</b> (only option available): Allows view-only access to <span class="mc-variable Snippet_Variables.Object variable varname">users</span>.</p> <p>To fine-tune this, you can configure the ability to view users' contact information. Click the gear icon <img src="assets/gear-icon-in-access-levels.png"> on the <b>View</b> button, then enable or disable the <b>View Contact Info</b> option (disabled by default).</p> </li> 
    </ul> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">Requestor</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> 
    <ul> 
     <li> <p><b>View</b> (only option available): Allows view-only access to <span class="mc-variable Snippet_Variables.Object variable varname">users</span>.</p> <p>To fine-tune this, you can configure the ability to view users' contact information. Click the gear icon <img src="assets/gear-icon-in-access-levels.png"> on the <b>View</b> button, then enable or disable the <b>View Contact Info</b> option (disabled by default).</p> </li> 
    </ul> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyB-Column1-LightGray">External User</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyA-Column1-LightGray"> <p>Access to <span class="mc-variable Snippet_Variables.Object variable varname">users</span> is not available. External users can use <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span> only to review and download documents and to see calendars that are shared with them.</p> </td> 
  </tr> 
 </tbody> 
</table>




## Teams {#teams}

In each access level, you can configure the following options for *`teams`*:

<table style="width: 100%;mc-table-style: url('../../../Resources/TableStyles/TableStyle-HeaderRow.css');margin-left: 0;margin-right: auto;" class="TableStyle-TableStyle-HeaderRow" cellspacing="15"> 
 <col class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <col class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <thead> 
  <tr class="TableStyle-TableStyle-HeaderRow-Head-Header1"> 
   <th class="TableStyle-TableStyle-HeaderRow-HeadE-Column1-Header1">Access level</th> 
   <th class="TableStyle-TableStyle-HeaderRow-HeadD-Column1-Header1">Options</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">Planner </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> 
    <ul> 
     <li> <p><b>View</b>: Allows view-only access to <span class="mc-variable Snippet_Variables.Object variable varname">teams</span>.</p> <p>To fine-tune this, click the gear icon <img src="assets/gear-icon-in-access-levels.png"> on the <b>View</b> button, then disable or enable any of the following options*. Both are disabled by default.</p> 
      <ul> 
       <li>View all teams</li> 
       <li> <p>View teams associated with my groups</p> </li> 
      </ul> </li> 
     <li> <p><b>Edit</b> (selected by default): Allows full editing access to <span class="mc-variable Snippet_Variables.Object variable varname">teams</span>.</p> <p>To fine-tune this, click the gear icon <img src="assets/gear-icon-in-access-levels.png"> on the <b>View</b> button, then disable or enable any of the following options*. All of them are enabled by default, except for the last two, <b>View all teams</b> and <b>View teams associated with my groups</b>.</p> 
      <ul> 
       <li>Create</li> 
       <li>Delete</li> 
       <li> <p>Edit teams I am on</p> </li> 
       <li> <p>Edit teams in groups I manage (Group Admins only)</p> </li> 
       <li> <p>View all teams</p> </li> 
       <li> <p>View teams associated with my groups</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">Worker </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> 
    <ul> 
     <li> <p><b>View</b>: Allows view-only access to <span class="mc-variable Snippet_Variables.Object variable varname">teams</span>.</p> <p>To fine-tune this, click the gear icon <img src="assets/gear-icon-in-access-levels.png"> on the <b>View</b> button, then disable or enable any of the following options*. Both are disabled by default.</p> 
      <ul> 
       <li>View all teams</li> 
       <li> <p>View teams associated with my groups</p> </li> 
      </ul> </li> 
     <li> <p><b>Edit</b> (selected by default): Allows full editing access to <span class="mc-variable Snippet_Variables.Object variable varname">teams</span>.</p> <p>To fine-tune this, click the gear icon <img src="assets/gear-icon-in-access-levels.png"> on the <b>View</b> button, then disable or enable any of the following options*. Only the first option, <b>Edit teams I am on</b>, is enabled by default.</p> 
      <ul> 
       <li> <p>Edit teams I am on</p> </li> 
       <li> <p>View all teams</p> </li> 
       <li> <p>View teams associated with my groups</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">Reviewer</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> 
    <ul> 
     <li> <p><b>View</b> (only option available): Allows view-only access to <span class="mc-variable Snippet_Variables.Object variable varname">teams</span>.</p> <p>To fine-tune this, click the gear icon <img src="assets/gear-icon-in-access-levels.png"> on the <b>View</b> button, then disable or enable any of the following options*. Both are disabled by default.</p> 
      <ul> 
       <li> <p>View all teams</p> </li> 
       <li>View teams associated with my groups</li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">Requestor</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> 
    <ul> 
     <li> <p><b>View</b> (only option available): Allows view-only access to <span class="mc-variable Snippet_Variables.Object variable varname">teams</span>.</p> <p>To fine-tune this, click the gear icon <img src="assets/gear-icon-in-access-levels.png"> on the <b>View</b> button, then disable or enable any of the following options*. Both are disabled by default.</p> 
      <ul> 
       <li> <p>View all teams</p> </li> 
       <li>View teams associated with my groups</li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyB-Column1-LightGray">External User</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyA-Column1-LightGray"> <p>Access to <span class="mc-variable Snippet_Variables.Object variable varname">teams</span> is not available. External users can use <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span> only to review and download documents and to see calendars that are shared with them.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42; For information about these options, see [Grant access to teams](grant-access-teams.md).


## Templates {#templates}

In each access level, you can configure the following options for *`templates`*:

<table style="width: 100%;mc-table-style: url('../../../Resources/TableStyles/TableStyle-HeaderRow.css');margin-left: 0;margin-right: auto;" class="TableStyle-TableStyle-HeaderRow" cellspacing="15"> 
 <col class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <col class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <thead> 
  <tr class="TableStyle-TableStyle-HeaderRow-Head-Header1"> 
   <th class="TableStyle-TableStyle-HeaderRow-HeadE-Column1-Header1">Access level</th> 
   <th class="TableStyle-TableStyle-HeaderRow-HeadD-Column1-Header1">Options</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">Planner </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> 
    <ul> 
     <li> <p><b>No access</b>: Blocks all access to <span class="mc-variable Snippet_Variables.Object variable varname">templates</span>.</p> </li> 
     <li> <p><b>View</b>: Allows view-only access to <span class="mc-variable Snippet_Variables.Object variable varname">templates</span>.</p> <p>To fine-tune this, you can configure the ability to share <span class="mc-variable Snippet_Variables.Object variable varname">templates</span>. Click the gear icon <img src="assets/gear-icon-in-access-levels.png"> on the <span style="font-weight: bold;" class="mc-variable Snippet_Variables.AccessLevelsViewOrEdit variable varname">View</span> button, then disable or enable the <b>Share</b> option (enabled by default).</p> </li> 
     <li> <p><b>Edit</b> (selected by default): Allows full editing access to <span class="mc-variable Snippet_Variables.Object variable varname">templates</span>.</p> <p>To fine-tune this, click the gear icon <img src="assets/gear-icon-in-access-levels.png"> on the <b><span class="mc-variable Snippet_Variables.AccessLevelsViewOrEdit variable varname">Edit</span></b> button, then disable or enable any of the following options. All of them are enabled by default.</p> 
      <ul> 
       <li> <p>Create</p> </li> 
       <li> <p>Delete</p> </li> 
       <li> <p>Share</p> </li> 
       <li> <p>Share Documents Publicly (externally)</p> </li> 
       <li> <p>Share system-wide</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">Worker </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> 
    <ul> 
     <li> <p><b>No access</b> (only option available): Blocks all access to <span class="mc-variable Snippet_Variables.Object variable varname">templates</span>.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">Reviewer</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> 
    <ul> 
     <li> <p><b>No access</b> (only option available): Blocks all access to <span class="mc-variable Snippet_Variables.Object variable varname">templates</span>.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">Requestor</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> 
    <ul> 
     <li> <p><b>No access</b> (only option available): Blocks all access to <span class="mc-variable Snippet_Variables.Object variable varname">templates</span>.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyB-Column1-LightGray">External User</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyA-Column1-LightGray"> <p>Access to <span class="mc-variable Snippet_Variables.Object variable varname">templates</span> is not available. External users can use <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span> only to review and download documents and to see calendars that are shared with them.</p> </td> 
  </tr> 
 </tbody> 
</table>



## Financial data {#financial-data}

In each access level, you can configure the following options for *`financial data`*:

<table style="width: 100%;mc-table-style: url('../../../Resources/TableStyles/TableStyle-HeaderRow.css');margin-left: 0;margin-right: auto;" class="TableStyle-TableStyle-HeaderRow" cellspacing="15"> 
 <col class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <col class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <thead> 
  <tr class="TableStyle-TableStyle-HeaderRow-Head-Header1"> 
   <th class="TableStyle-TableStyle-HeaderRow-HeadE-Column1-Header1">Access level</th> 
   <th class="TableStyle-TableStyle-HeaderRow-HeadD-Column1-Header1">Options</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">Planner </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> 
    <ul> 
     <li> <p><b>No access</b>: Blocks all access to <span class="mc-variable Snippet_Variables.Object variable varname">financial data</span>.</p> </li> 
     <li> <p><b>View</b>: Allows view-only access to <span class="mc-variable Snippet_Variables.Object variable varname">financial data</span>.</p> <p>To fine-tune this, click the gear icon <img src="assets/gear-icon-in-access-levels.png"> on the <b>View</b> button, then disable or enable any of the following options*. Both are enabled by default.</p> 
      <ul> 
       <li>View Role Billing &amp; Cost Rates</li> 
       <li> <p>View User Billing &amp; Cost Rates</p> </li> 
      </ul> </li> 
     <li> <p><b>Edit</b> (selected by default): Allows full editing access to <span class="mc-variable Snippet_Variables.Object variable varname">financial data</span>.</p> <p>To fine-tune this, click the gear icon <img src="assets/gear-icon-in-access-levels.png"> on the <b>View</b> button, then disable or enable any of the following options*. Only the last two options, <b>View Role Billing &amp; Cost Rates</b> and <b>View User Billing &amp; Cost Rates</b>, are enabled by default.</p> 
      <ul> 
       <li>Edit Role Billing &amp; Cost Rates</li> 
       <li> <p>Edit User Billing &amp; Cost Rates</p> </li> 
       <li>View Role Billing &amp; Cost Rates</li> 
       <li> <p>View User Billing &amp; Cost Rates</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">Worker </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> 
    <ul> 
     <li> <p><b>No access</b> (selected by default): Blocks all access to <span class="mc-variable Snippet_Variables.Object variable varname">financial data</span>.</p> </li> 
     <li> <p><b>View</b>: Allows view-only access to <span class="mc-variable Snippet_Variables.Object variable varname">financial data</span>.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">Reviewer</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> 
    <ul> 
     <li> <p><b>No access</b> (selected by default): Blocks all access to <span class="mc-variable Snippet_Variables.Object variable varname">financial data</span>.</p> </li> 
     <li> <p><b>View</b>: Allows view-only access to <span class="mc-variable Snippet_Variables.Object variable varname">financial data</span>.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">Requestor</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> 
    <ul> 
     <li> <p><b>No access</b> (only option available): Blocks all access to <span class="mc-variable Snippet_Variables.Object variable varname">financial data</span>.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyB-Column1-LightGray">External User</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyA-Column1-LightGray"> <p>Access to <span class="mc-variable Snippet_Variables.Object variable varname">financial data</span> is not available. External users can use <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span> only to review and download documents and to see calendars that are shared with them.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42; For information about these options, see [Overview of Billing and Revenue](billing-and-revenue-overview.md).


## Resource Management {#resource-management}

In each access level, you can configure the following options for *`Resource Management`*:

<table style="width: 100%;mc-table-style: url('../../../Resources/TableStyles/TableStyle-HeaderRow.css');margin-left: 0;margin-right: auto;" class="TableStyle-TableStyle-HeaderRow" cellspacing="15"> 
 <col class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <col class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <thead> 
  <tr class="TableStyle-TableStyle-HeaderRow-Head-Header1"> 
   <th class="TableStyle-TableStyle-HeaderRow-HeadE-Column1-Header1">Access level</th> 
   <th class="TableStyle-TableStyle-HeaderRow-HeadD-Column1-Header1">Options</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">Planner </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> 
    <ul> 
     <li> <p><b>No access</b>: Blocks all access to <span class="mc-variable Snippet_Variables.Object variable varname">Resource Management</span>.</p> </li> 
     <li> <p><b>View</b>: Allows view-only access to <span class="mc-variable Snippet_Variables.Object variable varname">Resource Management</span>.</p> </li> 
     <li> <p><b>Edit</b> (selected by default): Allows full editing access to <span class="mc-variable Snippet_Variables.Object variable varname">Resource Management</span>.</p> <p>To fine-tune this, click the gear icon <img src="assets/gear-icon-in-access-levels.png"> on the <b>Edit</b> button, then disable or enable any of the following options. Only the first option, <b>Edit priorities and budget hours in the Planner</b>, is enabled by default.</p> 
      <ul> 
       <li> <p> Edit priorities and budget hours in the Planner</p> </li> 
       <li> <p>Manage Resource Pools</p> <p>Note: In order to manage resource pools, a user needs additional access to financial data and permissions to project finances. If you grant Resource Management access to a Planner user who doesn't have access to financial data, the user can still see the hourly allocations in the Resource Planner, but can't switch to Cost view or view the Business Case. For more information, see <a href="grant-access-financial.md" class="MCXref xref">Grant access to financial data</a> and <a href="share-financial-permissions-object.md" class="MCXref xref">Share financial permissions on an object in Adobe Workfront</a>.</p> </li> 
       <li> <p>Update Planned Hours in the Workload Balancer</p> <p>Note: In order to update planned hours in the Workload Balancer, a user needs permission to contribute to the object, with Make Assignments enabled under Advanced Settings. For information, see <a href="sharing-permissions-on-objects-overview.md" class="MCXref xref">Overview of sharing permissions on objects in Adobe Workfront</a>.</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">Worker </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> 
    <ul> 
     <li> <p><b>No access</b>: Blocks all access to <span class="mc-variable Snippet_Variables.Object variable varname">Resource Management</span>.</p> </li> 
     <li> <p><b>View</b> (selected by default): Allows view-only access to <span class="mc-variable Snippet_Variables.Object variable varname">Resource Management</span>.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">Reviewer</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray"> 
    <ul> 
     <li> <p><b>No access</b>: Blocks all access to <span class="mc-variable Snippet_Variables.Object variable varname">Resource Management</span>.</p> </li> 
     <li> <p><b>View</b> (selected by default): Allows view-only access to <span class="mc-variable Snippet_Variables.Object variable varname">Resource Management</span>.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">Requestor</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray"> 
    <ul> 
     <li> <p><b>No access</b> (only option available): Blocks all access to <span class="mc-variable Snippet_Variables.Object variable varname">Resource Management</span>.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyB-Column1-LightGray">External User</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyA-Column1-LightGray"> <p>Access to <span class="mc-variable Snippet_Variables.Object variable varname">Resource Management</span> is not available. External users can use <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span> only to review and download documents and to see calendars that are shared with them.</p> </td> 
  </tr> 
 </tbody> 
</table>



## Scenario Planner area {#scenario-planner-area}

The default setting for all access levels is No Access. A *`Workfront administrator`* can change this to View or Edit access for any Planner, Worker, and Reviewer access level.


>[!NOTE]
>
>Users can view a plan that another user created only if a link to the plan is shared with them. 




## *`Workfront Goals`* area {#workfront-goals-area}

All six of the default access levels (and all 4 of the license types) can edit and view *`Workfront Goals`*.


Edit is the default option.
