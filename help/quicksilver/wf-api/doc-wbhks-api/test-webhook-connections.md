---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: Test Webhook connections
description: Test Webhook connections
author: Becky
feature: Workfront API
role: Developer
exl-id: 7452ebfc-7c72-4fea-99ac-7f76b12404b8
---

# Test Webhook connections

To verify that your document webhook implementation works correctly, run the manual tests in this section. These steps go through the Adobe Workfront web interface and indirectly hit the endpoints for your webhook implementation.

## Prerequisites

The following prerequisites are required to run the tests:

* A Workfront account with Advanced Document Management (ADM) enabled

* A Workfront user for this account with System Admin rights

* A Document Webhook instance with HTTP endpoints that are accessible to Workfront

These tests also assume that your Document Webhook instance is registered. (You can register your instance in Workfront under Setup > Documents > Custom Integrations.)

**Test 1: Provision the Document Webhook service for a user**

Tests the Authentication URL and Token Endpoint URL for OAuth-based Webhook providers.

1. In Workfront, Go to the main Documents page by clicking on the Documents link in the top&nbsp;navigation bar.
1. Click on the Add Documents drop-down and select your Document Webhook service under Add&nbsp;Service.
1. (OAuth services only) After completing the previous step, you will see your service's OAuth2&nbsp;authentication page load in a popup window. (Note: you may be prompted to log in to your service first.) From the authentication page, grant Workfront access to the user's account by clicking the Trust or Allow button.
1. Verify your service has been added to the Add Documents drop-down. If you don't see it initially, try&nbsp;refreshing your browser.

**Test 2: Link a document into Workfront Tests the following endpoints: /files, /metadata**

1. In Workfront, Go to the main Documents page by clicking on the Documents link in the top&nbsp;navigation bar.
1. Select your Document Webhook service under Add Documents.
1. From the modal, navigate through the folder structure.
1. Verify that you are able to navigate the folder structure.
1. Select and link a document into Workfront

**Test 3: Navigate to a document in the content management system**

Tests the following endpoints: /metadata (specifically the viewLink)

1. Link a document into Workfront
1. Select the document and click the Open link.
1. Verify that the document opens in a new tab.

**Test 4: Navigate to a document in the content management system (with login)**

Tests the following endpoints: /metadata (specifically the viewLink)

1. Ensure that you are logged out of the content management system.
1. Link a document into Workfront.
1. Select the document and click the Open link.
1. Verify that content management system's login screen loads in a new tab.
1. Login and verify that you're taken to the document

**Test 5: Download the document from the content management system**

Tests the following endpoints (specifically the download link): /metadata&nbsp;

1. Link a document into Workfront.
1. Select the document and click the Download link.
1. Verify that the download begins.

**Test 6: Search for content**

Tests the following endpoints: /search

1. In Workfront, Go to the main Documents page by clicking on the Documents link in the top&nbsp;navigation bar.
1. Select your Document Webhook service under Add Documents.
1. From the modal, perform a search.
1. Verify that the search results are correct.

**Test 7: Send document from Workfront to content management system**

Tests the following endpoints: /files, /uploadInit, /upload

1. In Workfront, Go to the main Documents page by clicking on the Documents link in the top navigation bar.
1. Upload a document to Workfront from your computer
1. Go to the document details page
1. From the Document Actions dropdown, select your Document Webhook service under Send To...
1. Go to the desired destination folder and click the Save button.
1. Verify that the document is uploaded to the correct location in the content management system.

**Test 8: View Thumbnails in Workfront**

Tests the following endpoints: /thumbnail

1. Link a document into Workfront.
1. Select the document in the list.
1. Verify that the thumbnail appears in the right panel.

**Test 9: Get the content bytes**

Tests the following endpoints: /download

1. Link a document into Workfront.
1. Go to the document details page.
1. Send the document to Workfront by selecting Document Actions > Send To... > Workfront. This will&nbsp;create a new document version in Workfront.
1. Download the document from Workfront by clicking on the Download link.

**Test 10: Refresh access token (OAuth2 Webhook providers only)**

Tests the following endpoints: Token Endpoint URL

1. Provision a the Document Webhook service for a user
1. Invalidate the user's access token by either 1 )waiting for it to timeout, or 2) invalidating it manually in&nbsp;the external system.
1. Refresh the access token in Workfront. You can do this, for example, by linking a document into Workfront. You will know that the access token refreshed successfully if you were able to navigate to and link a document.

>[!NOTE]
>
>Currently, the Send To... is not available for linked documents. This will be added by Workfront. You can test the /download endpoint by hitting the endpoint manually using a REST client, such as Postman. Alternatively, the /download endpoint can be tested by generating a digital proof. To enable, digital proofing please contact Workfront.
