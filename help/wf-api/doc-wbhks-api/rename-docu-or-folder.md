---
filename: rename-docu-or-folder
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
---



# Rename a document or folder (not yet implemented) {#rename-a-document-or-folder-not-yet-implemented}

Renames a document or folder with the given ID in the external system.


## URL {#url}

PUT /rename


## Query Parameters {#query-parameters}


&nbsp;


## Response {#response}

A JSON string indicating success or failure, as specified in the Error Handling section below.


` `**Example: **``PUT&nbsp;https://www.acme.com/api/rename


-------------------------------


id=1234


name=Folder B ­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­


-------------------------------


returns
`<pre>{</pre>``<pre>status: “success”</pre>``<pre>}</pre>` returns
`<pre>{</pre>``<pre>status: “failure”, error: “Folder cannot be renamed because a folder with that name already exists.”</pre>``<pre>}</pre>`  