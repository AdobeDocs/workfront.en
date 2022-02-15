---
filename: preview-sandbox
content-type: overview;how-to-procedural
product: workfront-proof
product-area: documents;system-administration
navigation-topic: system-information
---



# Preview Sandbox Testing Environment- *`Workfront Proof`*  {#preview-sandbox-testing-environment-workfront-proof}



>[!IMPORTANT] {type="important"}
>
>This article refers to functionality in the standalone product *`Workfront Proof`*. For information on proofing inside *`Adobe Workfront`*, see [Proofing](_proofing.md).


The Preview Sandbox is a testing environment that serves as a replica of your live environment and is refreshed each weekend by *`Workfront Proof`*.&nbsp;


## Understanding&nbsp;the Preview Sandbox {#understanding-the-preview-sandbox}

The Preview Sandbox serves as an environment where users in your organization&nbsp;can safely test and work with&nbsp;data from the Production&nbsp;environment without affecting the Production environment. It&nbsp;is ideal for running training sessions, testing out new features, and determining setup functionality.&nbsp;


Also, new product features are uploaded to the Preview Sandbox environment before they are&nbsp;delivered to the Production environment. Your users can try out new functionality there without affecting their usual workflow in the Production environment.


The Preview Sandbox contains your actual production&nbsp;data. Data flows from Production to Preview, and not in reverse. It refreshes every weekend, so the data can be up to one week behind the Production environment. Items created since the last refresh time are in the Preview Sandbox environment until the following refresh.


## Accessing the Preview Sandbox {#accessing-the-preview-sandbox}

By default, as a system administrator, you have access to the Preview Sandbox environment. If you cannot access the Preview Sandbox environment as described in this section, contact your *`Workfront administrator`* or our Support&nbsp;team.



* [Accessing the Preview Sandbox as a Stand-Alone Workfront Proof Customer](#accessing-the-preview-sandbox-as-a-stand-alone-proofhq-customer) 
* [Accessing the Preview Sandbox as a Workfront+Workfront Proof Customer](#accessing-the-preview-sandbox-as-a-workfront-proofhq-customer) 




### Accessing the Preview Sandbox as a Stand-Alone *`Workfront Proof`*&nbsp;Customer {#accessing-the-preview-sandbox-as-a-stand-alone-workfront-proof-customer}




1. Navigate to this URL:  `https://preview.proofhq.com`.
1. Log in using your Preview credentials.  
   Your Preview credentials should be the same as your Production credentials unless you changed them in Production after the Preview refresh happened. The logins are synchronized only when a refresh occurs, which takes place every weekend. They do not synchronize automatically.




### Accessing the Preview Sandbox as a Workfront+ *`Workfront Proof`* Customer {#accessing-the-preview-sandbox-as-a-workfront-workfront-proof-customer}

As a system administrator, you can access the *`Workfront Proof`* Preview Sandbox via the *`Workfront`* interface.&nbsp;


To access the *`Workfront Proof`*&nbsp;Preview Sandbox:



1.  Log in to your *`Workfront`* environment. 
1.  Click `Setup` in the Global Navigation bar. 
1. Click `System`> `Preferences`.  

1.  In the `Test Environments` section, click `Sandbox Preview`.  

1.  Log in with your Preview credentials.  
   Your Preview credentials should be the same as your Production credential unless you changed them in Production after the Preview refresh happened.&nbsp;The logins are synchronized only when a refresh occurs. They do not synchronize automatically. 
1.  Click the *`Workfront Proof`*&nbsp;icon in the Global Navigation Bar.  
   ![proof_access_proofhq.png](assets/proof-access-proofhq-350x39.png)  
   The *`Workfront Proof`*&nbsp;Preview environment displays. 





## Receiving Emails from the Preview Sandbox {#receiving-emails-from-the-preview-sandbox}

Email notifications are never triggered from the *`Workfront Proof`*&nbsp;Preview environment.&nbsp;
