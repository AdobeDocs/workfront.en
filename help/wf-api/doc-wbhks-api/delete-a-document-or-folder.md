---
filename: delete-a-document-or-folder
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
---



# Delete a document or folder (Not yet implemented) {#delete-a-document-or-folder-not-yet-implemented}



>[!NOTE]
>
>The release date for this feature is yet to be determined.


Deletes a document or folder with the given ID in the external system. Deleting a folder also deletes the folder contents.


## URL {#url}

PUT /delete


## Query Parameters {#query-parameters}


&nbsp;&nbsp;


Response A JSON string indicating success or failure, as specified in the Error Handling section below.


## Example {#example}

`<pre>PUT https://www.acme.com/api/delete ­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­ id=1234 ­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­</pre>` returns
`<pre>{</pre>``<pre>status: “success” </pre>``<pre>}</pre>` returns
`<pre>{</pre>``<pre>status: “failure”, error: “File not found”</pre>``<pre>}</pre>`  