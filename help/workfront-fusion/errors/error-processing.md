---
filename: error-processing
content-type: reference
product: workfront-fusion
product-area: workfront-integrations
navigation-topic: errors
---



# Error processing {#error-processing}

Sometimes an error can occur during the execution of a scenario. This usually happens if a service is unavailable due to a failure to connect to a service or if a validation fails. This article discusses the common errors that you may encounter. 


*`Adobe Workfront Fusion`* distinguishes between several basic error types. It will react differently depending upon on the type of error that occurred.


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
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray"> <p><span class="mc-variable WFVariables.WFFusionIntegration variable varname">Workfront Fusion for Work Automation and Integration</span> </p> <p data-mc-conditions="SnippetConditions.HIDE"><span class="mc-variable WFVariables.WFFusionAutomation variable varname">Workfront Fusion for Work Automation</span> </p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-LightGray" role="rowheader">Product</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-LightGray">Your organization must purchase <span class="mc-variable WFVariables.FullProdNameWFF variable varname">Adobe Workfront Fusion</span> as well as <span class="mc-variable WFVariables.FullProdNameWF variable varname">Adobe Workfront</span> to use functionality described in this article.</td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your *`Workfront administrator`*.


## Connection Error {#connection-error}

`<pre>ConnectionError</pre>` Connection error is one of the most common errors usually caused by unavailability of the third-party service for various reasons (overloading, maintenance, outage,and so on). The default handling of this error depends on which module it was encountered on:



* If the error occurs on the first module, the execution of the scenario is terminated with a warning message. *`Workfront Fusion`* then repeatedly attempts to rerun the scenario at increasing time intervals (these are explained below). If all attempts fail, *`Workfront Fusion`* deactivates the scenario.

* If the connection error occurs on another module than the first one, the subsequent steps depend on the [Allow storing incomplete executions](scenario-settings-panel.md#allow) option in the scenario advanced settings:
    
    
    * If this option is enabled, the execution of the scenario is moved to the Incomplete executions folder where *`Workfront Fusion`* repeatedly attempts to rerun the scenario at increasing time intervals. If all attempts fail, the execution will remain in the [View and resolve incomplete executions](view-and-resolve-incomplete-executions.md) folder awaiting manual resolution by the user.
    
    * If the option is disabled, the execution of the scenario ends with an error followed by a rollback phase. *`Workfront Fusion`* then repeatedly attempts to rerun the scenario at increasing time intervals. If all attempts fail, *`Workfront Fusion`* deactivates the scenario.
    
    
    





### Increasing time intervals {#increasing-time-intervals}

The algorithm of multiplicatively increasing time intervals between attempts when an error occurs is known as exponential backoff. The increasing time intervals are set as follows:



1. 10 minutes
1. 1 hour
1. 3 hours
1. 12 hours
1. 24 hours


The main reason for employing the increasing time intervals in *`Workfront Fusion`* is to prevent frequently executed scenarios from consuming operations on repeatedly failing attempts.


` `**Example: **``A scenario contains the Google Sheets trigger Watch Rows. Google Sheets is unavailable for 30 minutes due to maintenance when *`Workfront Fusion`* starts the scenario, so it is unable to retrieve new rows. The scenario stops and tries again in 10 minutes. As the service continues to be unavailable within this time frame, *`Workfront Fusion`* is still unable to get information about new rows. The next run of the scenario is scheduled in 1 hour. Google Sheets is available again within this time and the scenario runs successfully.


## Data error {#data-error}



```
DataError
```




A data error is generated when an item is incorrectly mapped and does not pass the validation performed on the *`Workfront Fusion`* side or on the side of the third-party service being used. For more information, see [Map information from one module to another](map-information-between-modules.md).


If this error occurs, the scenario, up to where the module failed, is moved to the [View and resolve incomplete executions](view-and-resolve-incomplete-executions.md) folder where you can troubleshoot the issue. However, the scenario does not stop and continues to run according to its schedule. To stop the execution of the scenario when Data error appears, enable the Sequential processing option in the [Scenario settings panel](scenario-settings-panel.md). For information about schedules, see [Schedule a scenario](schedule-a-scenario.md).


If you have not enabled the Allow storing incomplete executions option in the scenario settings, the execution of the scenario terminates with the error and a rollback is performed.


## Duplicate Data Error {#duplicate-data-error}

`<pre>DuplicateDataError</pre>` If *`Workfront Fusion`* tries to insert the same bundle twice into a service that does not allow duplicate data, a duplicate data error is generated. If this error occurs, *`Workfront Fusion`* proceeds in the same way as as it does for the data error.


## Invalid Access Token Error {#invalid-access-token-error}

`<pre>InvalidAccessTokenError</pre>` An invalid access token error occurs when *`Workfront Fusion`* cannot access your account registered with a third-party service. This mostly happens when you revoke access rights for *`Workfront Fusion`* in the administration of a given service but related scenarios keep running according to schedule.


If this error occurs, the execution of a scenario is stopped immediately. The rest of the scenario starting from the module where the error occurred is moved to the [View and resolve incomplete executions](view-and-resolve-incomplete-executions.md).


## Rate Limit Error {#rate-limit-error}



```
RateLimitError
```




If a limit set by a given service is exceeded, a rate limit error is generated. If this error happens, *`Workfront Fusion`* proceeds in the same way as it does for the Connection Error. For more information, see [Connection Error](#connecti) in the article [Error processing](#).


## Incomplete Data Error {#incomplete-data-error}



```
IncompleteDataError
```




An incomplete data error occurs only with triggers. This error is generated if a trigger fails to download required data from a given service.


If a scenario terminates with the IncompleteDataError, its further behavior will depend on its setting of Max number of consecutive errors. For more information, see [Number of consecutive errors](scenario-settings-panel.md#number) in the article [Scenario settings panel](scenario-settings-panel.md).


` `**Example: **``A scenario has the *`Workfront`* trigger Watch Record set to watch for documents. The scenario executes while you are uploading a large document, such as a long video. Because *`Workfront Fusion`* tries to download the video while it is still uploading to *`Workfront`*, the scenario terminates with the IncompleteDataError.


## Run time error {#run-time-error}

`<pre>RuntimeError</pre>` If any other error (not mentioned above) appears during scenario execution, it is reported as a RunTimeError.


If a scenario terminates with the RuntimeError, its further behavior will depend on its setting of Max number of consecutive errors. For more information, see [Number of consecutive errors](scenario-settings-panel.md#number) in the article [Scenario settings panel](scenario-settings-panel.md).


>[!NOTE]
>
>If a scenario starts with an instant trigger, the setting of Max number of consecutive errors is ignored and the scenario is deactivated immediately once the first error has occurred. For more information, see [Instant triggers](module-types.md#instant) in the article [Types of modules](module-types.md). 




## Inconsistency Error {#inconsistency-error}

`<pre>InconsistencyError</pre>` If any error described above occurs during the commit or rollback phase, a scenario will terminate with Inconsistency Error. For more information, see [Scenario execution, cycles, and phases](scenario-execution-cycles-phases.md).


If this error appears in a scenario, the execution of the scenario is immediately stopped.


## Warning {#warning}

While executing a scenario, you may receive a warning informing you about a problem. However, it does not prevent the scenario from being successfully completed.


For example, a warning can appear when the maximum allowed file size is exceeded and the Enable data loss option is disabled. For more information, see [Enable data loss](scenario-settings-panel.md#enable) in the article [Scenario settings panel](scenario-settings-panel.md).
