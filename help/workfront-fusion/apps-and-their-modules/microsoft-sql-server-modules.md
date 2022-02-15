---
filename: microsoft-sql-server-modules
content-type: reference
product: workfront-fusion
product-area: workfront-integrations
keywords: connector
navigation-topic: apps-and-their-modules
---



# Microsoft SQL Server modules {#microsoft-sql-server-modules}



## Access requirements {#access-requirements}

You must have the following access to use the functionality in this article:

<table style="width: 100%;margin-left: 0;margin-right: auto;mc-table-style: url('../../Resources/TableStyles/TableStyle-List-options-in-steps.css');" class="TableStyle-TableStyle-List-options-in-steps" cellspacing="0"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2"> 
 <tbody> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader"><span class="mc-variable WFVariables.FullProdNameWF variable varname">Adobe Workfront</span> plan*</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p><span class="mc-variable WFVariables.WFPlan-Pro variable varname">Pro</span> or higher</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader"><span class="mc-variable WFVariables.FullProdNameWFF variable varname">Adobe Workfront Fusion</span> license**</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray"> <p><span class="mc-variable WFVariables.WFFusionIntegration variable varname">Workfront Fusion for Work Automation and Integration</span> </p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-LightGray" role="rowheader">Product</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-LightGray">Your organization must purchase <span class="mc-variable WFVariables.FullProdNameWFF variable varname">Adobe Workfront Fusion</span> as well as <span class="mc-variable WFVariables.FullProdNameWF variable varname">Adobe Workfront</span> to use functionality described in this article.</td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your *`Workfront administrator`*.


## Using Microsoft SQL Server modules {#using-microsoft-sql-server-modules}

You can execute your custom logic directly on your database server through stored procedures. *`Adobe Workfront Fusion`* loads interface of input/output parameters and recordset dynamically so each parameter or value can be mapped individually. Before you start configuring your scenario, make sure the account you're using to connect to your database has read access to 

```
INFORMATION_SCHEMA.ROUTINES
```

and 

```
INFORMATION_SCHEMA.PARAMETERS
```

views.


Network traffic from *`Workfront Fusion`* originates from one of these four IP addresses:
`<pre>35.160.0.242</pre>``<pre>34.213.36.118</pre>``<pre>3.209.27.146</pre>``<pre>18.205.251.4</pre>` When Fusion establishes the connection to the SQL server destination, the Fusion user identifies the Host (the domain name or IP address where the server is hosted) and the port. Fusion can connect to any available host and port.


To learn more about creating a stored procedure, see Microsoft SQL Server documentation.


>[!NOTE]
>
>*`Workfront Fusion`* doesn't support multiple recordsets. Only the first one is processed.




## Troubleshooting error ER_LOCK_WAIT_TIMEOUT: Lock wait timeout exceeded; try restarting transaction {#troubleshooting-error-er-lock-wait-timeout-lock-wait-timeout-exceeded-try-restarting-transaction}

This error occurs when you modify the same data using multiple modules. It is caused by SQL transactions.


When any SQL module is executed, it starts a transaction. The transaction is finished after the scenario is fully executed.


If another module tries to access the same data, it has to wait until the previous transaction is finished. Since the first transaction will be finished after the scenario is finished, the second transaction can never begin.


### Solution: {#solution}

Turn on Auto-commit. Auto-commit finishes (commits) every transaction immediately after the module execution is done.



1. Click the Scenario settings icon ![](assets/scenario-settings-icon.png)at the bottom of the screen.
1. Click the `Auto commit` checkbox.
1. Click `OK` to save the scenario settings.


