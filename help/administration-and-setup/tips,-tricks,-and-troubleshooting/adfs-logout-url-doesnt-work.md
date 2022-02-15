---
filename: adfs-logout-url-doesnt-work
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration
navigation-topic: tips-tricks-troubleshooting-setup-admin
---




# ADFS logout URL doesn't work {#adfs-logout-url-doesnt-work}



## Overview {#overview}

When using the ADFS logout URL (https://myadfsserver.domain.net/adfs/ls/?wa=wsignout1.0), you receive a message page with the error: "There was a problem accessing the site. Try to browse to the site again."


If the problem persists, contact the administrator of this site and provide the following reference number to identify the problem: **57092dfc-751a-4915-8e6a-b4c5d413f8c6**


## Details {#details}




1. In your ADFS manager server, go to **Trust Relationships** > **Relying Party Trusts** > <your party trust> properties.

1. Under the **Endpoints** tab, click **Add**.

1.  **Endpoint Type** = SAML Logout, Binding = POST, URL = https://myadfsserver.domain.net/adfs/ls/?wa=wsignout1.0


   You can set a response URL if you want it to redirect to another page. But we recommend the ADFS site because it warns that you are logged off, but you should still close your browser.



