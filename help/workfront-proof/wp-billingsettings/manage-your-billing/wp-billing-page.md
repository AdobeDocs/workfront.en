---
filename: wp-billing-page
content-type: overview
product: workfront-proof
product-area: documents;system-administration
navigation-topic: manage-your-billing-workfront-proof
---



# The *`Workfront Proof`* Billing Page {#the-workfront-proof-billing-page}



>[!IMPORTANT] {type="important"}
>
>This article refers to functionality in the standalone product *`Workfront Proof`*. For information on proofing inside *`Adobe Workfront`*, see [Proofing](_proofing.md).




## The Billing Page {#the-billing-page}

To access the Billing page, open the `Settings` menu it the top right of the screen and choose `Billing` in the drop-down menu.


The Billing page contains the following:



* Account name (1)
* Accounts list (e.g. if you have Satellite accounts)(2)
* Change plan (3)
* Change payment details (4)
* New satellite account (5)
* Close account (6)
* Current plan information (7)
* Billing contact and address (8)
* Usage statistics (9)
* Billing history (10)
*  Billing activity (11)


  ![Billing_page.jpg](assets/billing-page-350x315.jpg)







## Current Plan {#current-plan}

This section (7) shows the details of your current plan, including the following:



* The name of the plan
* Current payment method
* Current plan start and finish dates
* Next plan type
*  Next plan payment method


  For more information, see [Choosing Your Payment Method in Workfront Proof](choose-payment-method-in-wp.md).





## Billing Contact and Address {#billing-contact-and-address}

This section (8) shows the main billing contact and address details for your account.


The Billing contact can be selected only from the users set up as the Billing Administrators on your account. On the Satellite accounts, only the Billing Administrators from the main account can be set in this field.


![Billing_Contact.png](assets/billing-contact-350x137.png)




>[!NOTE]
>
>&nbsp;You can have multiple Billing Administrators on your account, but only one of them, selected in the Billing contact field, will be receiving all the billing notifications and account usage alerts. For more information, see [The Workfront Proof Billing Page](#).


This includes the following notification emails:



* Proof usage
* Invoices
* Downgrade
* Late payment/Account suspension alert
*  Credit card failure


  ![Billin_CC.png](assets/billin-cc-350x103.png)





The Billing CC field also allows you to add an email address to be copied on all billing-related emails. Click on the filed to activate incline editing and enter an email address of your choice (this can be an existing user's email address too).


## Billing Address {#billing-address}

This section&nbsp;uses inline editing so simply click on the fields to enter/edit&nbsp;the text.


>[!NOTE]
>
>&nbsp;We include this address on&nbsp;your subscription invoices so make sure this data is always&nbsp;up-to-date.



![Billing_Address.png](assets/billing-address-350x199.png) 

## Usage Statistics {#usage-statistics}

This section shows the usage statistics for your account within the current billing period, including the following:



* Storage used
* Proofs used
* Users limit used


![Usage_Statistics.png](assets/usage-statistics-350x51.png) 

### Usage Warnings {#usage-warnings}

The [Proof Permissions Profiles in Workfront Proof](proof-perm-profiles-in-wp.md) set as the Billing Contact (1) on your account will be notified via email when your account reaches:



* 75% and then 98% of your storage capacity
* 75% and then 100% of your *`proof`* limit


![Billing_Contact__1_.png](assets/billing-contact--1--350x74.png)

Once the *`proofs`* or storage limits are reached you will also see the alerts at the top of the Billing page:



* For the *`proofs`* limit reached


&nbsp; ![Proofs_limit_reached.png](assets/proofs-limit-reached-350x65.png)





* For the storage limit reached


![Storage_limit_reached.png](assets/storage-limit-reached-350x65.png)



>[!NOTE]
>
>Your *`proof`* count is used up when *`proofs`* are created in your account and cannot be restored by removing the *`proofs`*.


Storage space can be freed by deleting the *`proofs`* and files and emptying the Trash afterwards.


Please remember that if you need more *`proofs`*, storage, or users you can upgrade your account&nbsp;at any time; and it takes immediate effect.


## Billing History {#billing-history}

This section shows the activity for any recent billing periods. You can also download your invoices from this section.


For more information, see " [Downloading Your Workfront Proof Invoice](download-wp-invoice.md)."


## Billing Activity {#billing-activity}

This section shows recent changes to your billing set up, e.g., subscriptions, upgrades, downgrades, and renewals of your *`Workfront Proof`* Plan.


If you change your plan to one with a lower user limit (1), users exceeding the new limit will automatically be deactivated when the new plan starts. This activity will also be captured in your Account logs (2).


![Billing_Downgrade_log.png](assets/billing-downgrade-log-350x45.png)




&nbsp; ![Account_Activity_-_Deleted_users.png](assets/account-activity---deleted-users-350x94.png)


