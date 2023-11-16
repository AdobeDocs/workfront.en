---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: Authentication for Document Webhooks
description: Authentication for Document Webhooks
author: Becky
feature: Workfront API
role: Developer
exl-id: 2303c202-27c7-4922-a613-e9824910504c
---
# Authentication for Document Webhooks

## Authentication

Adobe Workfront document webhooks supports two different forms of authentication: OAuth2 and ApiKey. In both cases, Workfront passes authentication tokens in the header when making an API call.

### OAuth2

OAuth2 allows Workfront to make authorized API calls to a webhook provider on behalf of a user. Before doing so, the user must connect their external document provider account to Workfront and grant Workfront

access to act on their behalf. This handshaking process only happens once for each user. Here's how it works:

1. The user begins connecting the webhook integration to their account. Currently, this is done by&nbsp;clicking the "Add Document" dropdown > "Add Service" > Custom integration name.
1. Workfront navigates the user the Authentication URL, which may prompt the user to login to the&nbsp;external document provider. This page is hosted by the webhook provider or the external document management system. When doing so Workfront adds a "state" parameter to the Authentication URL. This value must be passed back to Workfront by appending the same value to the Workfront Return URI in the step below.
1. After logging to the external system (or if the user is already logged in), the user is taken to an&nbsp;"Authentication" page, which explains that Workfront is requesting access to perform a set of actions on the user's behalf.
1. If the user clicks the "Allow" button, the browser will redirect to the Workfront Redirect URI , adding "code=`<code>`" to the querystring. Per the OAuth2 spec, this token is short lived. The querystring must also have the following, "state=`<sent_by_workfront>`".
1. Workfront processes this request and makes an API call to the Token Endpoint URL with the&nbsp;authorization code.
1. The Token Endpoint URL returns a refresh token and access token.
1. Workfront stores a these tokens and fully provisions the webhook integration for this user.
1. From this point forward, Workfront will be able to make authorized API calls to the webhook provider.&nbsp;When making these calls, Workfront will send the the access token in the HTTP request header as shown below:  

   ```
   -------------------------------  
   Authorization: Bearer [access_token] ­­­­­­­­­­­­­­­­­­­­­­­­­­  
   -------------------------------
   ```

1. If the access token has expired, Workfront will make a call to the Token Endpoint URL to retrieve a&nbsp;new access token then attempt the authorized API call again with the new access token.

### ApiKey

Making authorized API calls to a webhook provider using an ApiKey is much simpler than OAuth2. When making an API call, Workfront will simply pass the ApiKey and Workfront username in the HTTP request header:&nbsp;

```
-------------------------------

apiKey: 12345

username: johndoe@foo.com

-------------------------------
```

The Webhook provider can use the username to apply user-specific permissions. This works best when both systems connect to LDAP using Single Sign On (SSO).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h3>Adding Request Headers (optional)</h3>
<p>In addition to using either OAuth2 tokens or an ApiKey for authentication, Workfront can send a predefined set of headers to the webhook provider for every API call. A Workfront admin can setup set this up when&nbsp;registering or editing a Webook Integration, as described in the section above. See Registering a Webhook Integration.</p>
<p>For example, this can be used for Basic Authentication. To do this, the Workfront administrator would add the following Request Header information in the Custom Integration dialog:</p>
<p>&nbsp; &nbsp; &nbsp;Authorization Basic QWxhZGRpbjpvcGVuIHNlc2FtZQ==</p>
<p>where QWxhZGRpbjpvcGVuIHNlc2FtZQ== is a base-64 encoded string of "username:password". See Basic Authentication . Provided that this added, Workfront will pass this in the HTTP request header, in addition to other request headers:&nbsp;</p>
<p>-------------------------------</p>
<p>apiKey: 12345</p>
<p>username: johndoe@foo.com</p>
<p>Authorization: Basic QWxhZGRpbjpvcGVuIHNlc2FtZQ== ­­­­­­­­­­­­­­­­­­­­­­­­­­</p>
<p>-------------------------------</p>
</div>
-->
