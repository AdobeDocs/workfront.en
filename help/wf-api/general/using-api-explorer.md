---
filename: using-api-explorer
content-type: api
navigation-topic: general-api
title: Using the API Explorer
description: When using the Adobe Workfront Core API, the API Explorer is a legacy reference tool that catalogs the relationships between supported resources, parameters, and variables.
---

# Using the API Explorer

When using the Adobe Workfront Core API, the API Explorer is a legacy reference tool that catalogs the relationships between supported resources, parameters, and variables.

## Access the API Explorer:

<ol> 
 <li value="1">Use a web browser to navigate to the <a href="https://one.workfront.com/s/api-explorer" target="_blank">API Explorer</a> <br><img src="assets/mceclip1-350x149.png" style="width: 350;height: 149;"></li> 
 <li value="2">In the upper right of the API Explorer, select the desiredWorkfront <span class="bold">API Version</span>, by default the most current version is automatically selected</li> 
 <li value="3"> The <span class="bold">Filter</span> field, can be used to filter the objects listed by name and will truncate the list of objects displayed accordingly:<p><br><img src="assets/mceclip2-350x147.png" style="width: 350;height: 147;"></p>
  <ul>
   <li><span class="bold">Fields</span>: Available fields within the specified object.</li>
   <li><span class="bold">References</span>: Available reference variables for the specified object. A reference is an alias for a variable. Once initialized, a reference can be used interchangeably with the variable name. A reference uses initialized memory.</li>
   <li><span class="bold">Collections</span>: Available collections for the object. Collections are variables that represent a one-to-many relationship between the object and the resource.</li>
   <li><span class="bold">Search</span>: Available search resources for the object. The results of a search are based on the query parameters specified by the search resource in the API request.</li>
   <li><span class="bold">Actions</span>: Supported actions for the object. Actions can be simple or complex procedures that execute against a resource or set of resources. A given action may also affect related resources.</li>
  </ul></li> 
 <li value="4">Open a tab, then click the Object ID to view applicable variables.<br><img src="assets/approval-350x89.png" style="width: 350;height: 89;"><br>Depending on the object selected, the following variables may apply:<br>
  <table cellspacing="15">
   <col>
   <col>
   <thead>
    <tr>
     <th>Variable</th>
     <th>Definition</th>
    </tr>
   </thead>
   <tbody>
    <tr>
     <td>Field Name</td>
     <td>The name of a field used in an operation within the Workfront API.</td>
    </tr>
    <tr>
     <td>Field Type</td>
     <td>The kind of values that can be entered into a specific field in a data table. Possible field type values include string, double, int, dateTime.</td>
    </tr>
    <tr>
     <td>Enumerated Type</td>
     <td>The kind of values that can be used to identify a data type.</td>
    </tr>
    <tr>
     <td>Possible Values</td>
     <td>Acceptable values for the object.</td>
    </tr>
    <tr>
     <td>Attribute Type ObjCode</td>
     <td>Attributes that can be used to modify the object class.</td>
    </tr>
    <tr>
     <td>URL</td>
     <td>The entry path that allows your app to communicate with the Workfront API.</td>
    </tr>
    <tr>
     <td>Arguments</td>
     <td>The object's variables that can be passed between your application and Workfront.</td>
    </tr>
    <tr>
     <td>Result Type</td>
     <td>Allowable data types that can be returned from a method.</td>
    </tr>
   </tbody>
  </table></li> 
</ol>

