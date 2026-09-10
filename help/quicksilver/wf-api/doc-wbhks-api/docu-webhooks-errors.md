---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: Document Webhooks Error Handling
description: Document Webhooks Error Handling
author: Becky
feature: Workfront API
role: Developer
exl-id: 6e0f3be7-5321-44bd-a404-d5bef1462d82
TQID: https://experienceleague.adobe.com/KoMJXXZbDdywLGIwYTu7o8GigPxQ5RG6sNQpOTMHWY0
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
role_v2:
  - id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
    internal-label: Developer
---
# Document Webhooks Error Handling

Problems can arise when processing API requests. This should be handled in a consistent way across all API endpoints. When an error occurs, the webhook provider should innclude an error code in the response header. Error codes include:

* 403 - Forbidden. Indicates that either the request tokens are missing or invalid, or that credentials associated with the tokens don't have access to the specified resource. For OAuth-based webhook providers, Adobe Workfront will attempt to retrieve new access tokens.

* 404 - Not found. Indicates that the specified file or folder doesn't exist.

* 500 - Internal Server Error. Any other type of error.

* Description of the error in the response body using the following format:  
  
  ```
  {status: "error"
   error: "Sample error message"}
  ```
