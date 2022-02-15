---
filename: wp-spf-records
product: workfront-proof
product-area: documents;system-administration
navigation-topic: avoiding-spam-filters
---



# *`Workfront Proof`* SPF records {#workfront-proof-spf-records}



>[!IMPORTANT] {type="important"}
>
>This article refers to functionality in the standalone product *`Workfront Proof`*. For information on proofing inside *`Adobe Workfront`*, see [Proofing](_proofing.md).


*`Workfront Proof`* sends email notifications to your reviewers from a *`Workfront Proof`* email address such as notification@ *`proofing`*.yourdomain.com. In order to ensure that your recipients' mail servers trust all *`Workfront Proof`* email notifications, you need to set up a Sender Policy Framework (SPF) record for your customized domain connected to the *`Workfront Proof`* account (for example, ` *`proofing`*.yourdomain.com`).


To set up an SPF record, you will need to include the SPF record used for our primary domain.



1.  Add a  `DNS TXT` entry for your domain with the following value:


   v=spf1 a:mx.proofhq.com -all


   Your email administrator or IT personnel can help you set this up.  



   >[!TIP] {type="tip"}
   >
   >You can use the free tool at [https://mxtoolbox.com/spf.aspx](https://mxtoolbox.com/spf.aspx) to review *`Workfront`* SPF records.  






