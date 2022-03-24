---
filename: docu-webhooks-errors
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: Document Webhooks Error Handling
description: Problems can arise when processing API requests. This should be handled in a consistent way across all API endpoints. When an error occurs, the webhook provider should do the following:
---

# Document Webhooks Error Handling

Problems can arise when processing API requests. This should be handled in a consistent way across all API endpoints. When an error occurs, the webhook provider should do the following:

* Include an error code in the response header. Error codes include:

   * 403 - Forbidden. Indicates that either the request tokens are missing or invalid, or that credentials associated with the tokens don’t have access to the specified resource. For OAuth-based webhook providers, Adobe Workfront will attempt to retrieve new access tokens.
   * 404 - Not found. Indicates that the specified file or folder doesn’t exist.
   * 500 - Internal Server Error. Any other type of error.

* Describe the error in the response body using the following format:  
  <pre>{</pre><pre>status: “error”</pre><pre>error: “Sample error message”</pre><pre>}</pre>

