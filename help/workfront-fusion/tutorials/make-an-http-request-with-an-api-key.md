---
filename: make-an-http-request-with-an-api-key
product: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Make an HTTP request with an API Key
description: Use the JSON Generator in the Create JSON module to automatically add a data structure using a sample JSON. Learn how to modify it and make an HTTP request using an API key to connect to a third-party service.
---

# Make an HTTP request with an API Key

Use the JSON Generator in the Create JSON module to automatically add a data structure using a sample JSON. Learn how to modify it and make an HTTP request using an API key to connect to a third-party service.

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">In this tutorial, we have used SendGrid and have shown how to do the following:</p>
-->

In this tutorial, we have used SendGrid and have shown how to do the following:

<!--
<ol data-mc-conditions="QuicksilverOrClassic.Draft mode">
<li value="1">Connect to SendGrid over HTTP</li>
<li value="2">Send an email using SendGrid directly from the HTTP module on <em>Workfront Fusion</em></li>
<li value="3">Send an email using a template on SendGrid</li>
</ol>
-->

1. Connect to SendGrid over HTTP
1. Send an email using SendGrid directly from the HTTP module on *Workfront Fusion*
1. Send an email using a template on SendGrid

>[!NOTE]
>
>* >
>  <!-->
>  <p data-mc-conditions="QuicksilverOrClassic.Draft mode">SendGrid's authentication takes place using an API Key and hence why we use the 'Make a request' HTTP module on <em>Workfront Fusion</em>.</p>>
>  -->
>  SendGrid's authentication takes place using an API Key and hence why we use the 'Make a request' HTTP module on *Workfront Fusion*.
>
>  Screenshot
>
>* To send an email directly from the HTTP module, you need to add the 'content' Parameter to your JSON data structure. As you can see below, 'content' is an array of collections; 'type' and 'value' are where you need to define the content type and the actual content respectively. Also, it is a required parameter and will result in an error if left blank.
>
>  Screenshot
>
>* To send an email using a template, you need to add the 'template_id' parameter.>
>  <!-->
>  <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">>
>  As you can see in the image below,>
>  </MadCap:conditionalText>>
>  -->
>  `<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">  As you can see in the image below, </MadCap:conditionalText>` 'Template_id' is a simple string and is an optional parameter, so it can be left blank.
>
>  Screenshot
>

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">Video Tutorial:</p>
-->

Video Tutorial:

<!--
<p class="PinkDraftNote" data-mc-conditions="QuicksilverOrClassic.Draft mode">Video</p>
-->

Video

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">You can refer to the SendGrid API Docs <a href="https://sendgrid.com/docs/API_Reference/api_v3.html">here</a>.</p>
-->

You can refer to the SendGrid API Docs [here](https://sendgrid.com/docs/API_Reference/api_v3.html).

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">Please note that <em>Workfront Fusion</em> only supports V3 of the SendGrid API.</p>
-->

Please note that *Workfront Fusion* only supports V3 of the SendGrid API.
