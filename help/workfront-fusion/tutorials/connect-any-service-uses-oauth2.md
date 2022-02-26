---
filename: connect-any service-uses-oauth2
product: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Connect to any web service that uses OAuth2
description: Example used throughout - unsupported app DeviantArt. Recreate this with an app we support??
---

# Connect to any web service that uses OAuth2

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">Example used throughout - unsupported app DeviantArt. Recreate this with an app we support??</p>
-->

Example used throughout - unsupported app DeviantArt. Recreate this with an app we support??

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">Should the title not specify just the OAuth2 authorization type, since there are also 2 others--Basic Authorization and API key?</p>
-->

Should the title not specify just the OAuth2 authorization type, since there are also 2 others--Basic Authorization and API key?

One of the many great features of *Workfront Fusion* is the ability to connect almost any web service to a scenario. In the following guide, we will show you with the help of a real example, that you can manage communication with an API without writing a single line of code.

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">This article users the DeviantArt service to show how <em>Workfront Fusion</em> can integrate with any web service. Our goal is to get a list of the latest deviations. Before we can configure this scenario though, we first have to find out some basic information about the service. Our first step will be to go through the Development section and find out what method DeviantArt uses for user authentication, and which API is appropriate to perform the desired function.</p>
-->

This article users the DeviantArt service to show how *Workfront Fusion* can integrate with any web service. Our goal is to get a list of the latest deviations. Before we can configure this scenario though, we first have to find out some basic information about the service. Our first step will be to go through the Development section and find out what method DeviantArt uses for user authentication, and which API is appropriate to perform the desired function.

*Workfront Fusion* supports the following authorization types:

* OAuth2
* Basic Authorization
* API key

Screenshot

## Getting ready

In the Authentication section you will learn that DeviantArt uses a standardized OAuth2 protocol for authorization. At the same time, you will find out that you must first create a so-called client to be able to communicate with the API. To do that, click the register your application link. This will open up a form that allows to create a new application. Fill in the name and description of the application and upload the icon.

Screenshot

Next follows the Application settings section in which you need to fill out the OAuth2 Redirect URI Whitelist field. All services that use standard OAuth2 protocol for authorization require this parameter. The value of this parameter is always the same - 

```
https://www.workfront.com/oauth/cb/oauth2
```

. This is the URL, that a user is redirected to after they authorize *Workfront Fusion* to access the given service. This way, *Workfront Fusion* learns that the authorization has been successful, and creates a new connection with the service.

Screenshot

Once you have completed the registration, you will be taken to a screen where you can view two important values - 

```
client_id
```

and 

```
client_secret
```

. Write down these two values, you will need them later on.

Screenshot

Now go back to the Authentication section and get two important pieces of information - authorization URL and access token URL. All services that use standard authorization OAuth2 protocol always include both URL addresses in their documentation.

Screenshot

Now we have all important information about authorization so we can go on to the section APIs which describes in detail all API calls. The API that suits our purpose is located at 

```
GET /browse/newest
```

. Expand the 

```
Authentication
```

and 

```
Parameters
```

sections, from which you can then learn what 

```
scope
```

is required to call this API and what parameters you can send along with the request.

Screenshot

## Creating a scenario

Now, go to *Workfront Fusion* and create a new scenario.

>[!NOTE]
>
>Before you start setting up your scenario in *Workfront Fusion*, we recommend that you go through all APIs that you plan to call and get a list of all scopes that are needed. This way you can aquire all the necessary scopes at once and avoid the hassle of expanding the scopes in the future.

Choose the OAuth 2.0 HTTP(S) request and response processing module from the HTTP app and add it to your scenario. In the open configuration window, click the `Add` button. This will bring up a window that allows you to add a new OAuth2 connection. In this step, enter the information that you have found in the documentation:

| &nbsp; |&nbsp; |
|---|---|
| Connection name |Enter any name you would like to identify as the connection. |
| Authorize URI |the Authorize URL specified in the Authentication section of the DeviantArt documentation. |
| Token URI |the Access Token URL indicated in the Authentication section of the DeviantArt documentation. |
| Scope  |Specify the list of access scope that you want to grant to *Workfront Fusion* and associate with this connection. In our case, it is enough to select the browse value. |
| Client ID |the client ID you were given once you had created the application. |
| Client Secret |the secret key you were given once you had created the application. |

Screenshot

After you click the Create a connection button, *Workfront Fusion* will try to establish the connection. If you have filled in the correct information, a window will pop up after a few seconds, in which you can authorize *Workfront Fusion* to access the given service via the application you have created.

Screenshot

After you grant consent, the access tokens will be exchanged in the background automatically. If everything is okay, the configuration window will be automatically populated with the newly created connection. Set up the URL address of the API endpoint according to the specifications given in the API documentation and specify optional parameters (in our case, we will enter 

```
https://www.deviantart.com/api/v1/oauth2/browse/newest
```

). When creating a scenario, it is always better to work with a smaller number of bundles. We will, therefore, add the limit=5 parameter to the end of the URL.

## Testing

The integration is now ready and you can run the scenario. The execution results show that the call has ended with a 200 status, which means that the run completed successfully. The response details contain complete JSON data that is available for further use. In order to use this data in your scenario, you first need to parse it. That’s what the Parse JSON module from the JSON app is for. Before you add this module to your scenario, copy the whole JSON response to the system clipboard - you’ll need it in order to generate a data structure. Thanks to the data structures, *Workfront Fusion* knows exactly what structure the received data has.

Screenshot

To add the Parse JSON module to your scenario, in the settings of the module, map the Data variable from the HTTP app to the JSON string field. Next to the Data structure field, click the Add button and in the panel that opens, choose Generator. In the data structure generator, choose the 

```
JSON
```

value as Content type and in the Sample data field paste the JSON response from the server that you have copied to the system clipboard. Once you confirm your entries, the data structure will be generated automatically. Give a name to the Data structure and click the Save button. The configuration of the Parse JSON module is now complete. Click the Save button to confirm the settings.

Now you can run the scenario. Once the scenario run is complete, view details of the JSON module run. If everything has been processed without errors, you will see a list of 5 new DeviantArt deviations. You can then easily browse through the data structure and map obtained values to other modules.

Screenshot
