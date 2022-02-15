---
filename: create-folder-docu-webhook
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
---



# Create a Folder with Document Webhooks {#create-a-folder-with-document-webhooks}

Creates a folder in a given directory.


## URL {#url}

POST /createFolder


## Query Parameters {#query-parameters}


&nbsp;


`Response` 


The metadata for the newly created folder, as defined by the /metadata endpoint.


## Example {#example}

`<pre>POST https://www.acme.com/api/createFolder ­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­<br>-------------------------------<br>parentId=1234<br>name=New Folder ­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­<br>-------------------------------</pre>` returns
`<pre>{title:"New Folder",br /> kind:"folder"<br> id":"5678",<br> viewLink:"”,<br> downloadLink:"",<br> mimeType:"",<br> dateModified:"2014­06­05T17:39:45.251Z"<br> size: ""<br> }</pre>`  