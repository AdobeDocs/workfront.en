---
filename: get-list-folder-contents
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
---



# Get item list of folder contents {#get-item-list-of-folder-contents}

Returns metadata for the files and folders for a given folder.


## URL {#url}

GET /files


## Query Parameters {#query-parameters}




## Response {#response}

JSON containing a list of files and folders. The metadata for each item is the same that returned by the /metadata endpoint.


` `**Example: **``https://www.acme.com/api/files?parentId=123456
`<pre>[ {title:"Folder A",< br />kind:"folder"< br />id":"2lj23lkj",< br />viewLink:" https://www.acme.com/viewDocument?id=2lj23lkj ”,< br />downloadLink:"https://www.acme.com/downloadDocument?id=2lj23lkj",< br />mimeType:"",< br />dateModified:"2014­06­05T17:39:45.251Z"< br />size: ""< br />},< br />{< br />title:"My Document",< br />kind:"file"< br />id":"da8cj234",< br />viewLink:" https://www.acme.com/viewDocument?id=da8cj234 ”,< br />downloadLink:"https://www.acme.com/downloadDocument?id=da8cj234",< br />mimeType:"image/png",< br />dateModified:"2014­06­05T17:39:45.251Z"< br />size: "32554694"< br />}]</pre>` 