

# Intacct modules

>[!IMPORTANT]
>
>You're currently viewing the Adobe Workfront Classic version of this document. Adobe Workfront Classic is no longer supported. All Adobe Workfront Classic functionality, along with this documentation, will be removed in July 2022. Please transition to the the new Adobe Workfront experienceas soon as possible, and switch to the new Adobe Workfront experience version of this document.

In an Adobe Workfront Fusion scenario, you can automate workflows that use Intacct, as well as connect it to to multiple third-party applications and services.

If you need instructions on creating a scenario, see [Create a scenario in Adobe Workfront Fusion](../../workfront-fusion/scenarios/create-a-scenario.md).

For information about modules, see [Modules in Adobe Workfront Fusion](../../workfront-fusion/modules/modules.md).

## Access requirements

You must have the following access to use the functionality in this article:

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Pro or higher</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Plan, Work</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront Fusion license**</td> 
   <td> <p>Workfront Fusion for Work Automation and Integration </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>Your organization must purchase Adobe Workfront Fusion as well as Adobe Workfront to use functionality described in this article.</td> 
  </tr> <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td role="rowheader">Access level configurations*</td> 
    <td> <!--
      <p data-mc-conditions="QuicksilverOrClassic.Draft mode">You must be a Workfront Fusion administrator for your organization.</p>
     --> <!--
      <p data-mc-conditions="QuicksilverOrClassic.Draft mode">You must be a Workfront Fusion administrator for your team.</p>
     --> </td> 
   </tr>
  --> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your Workfront administrator.

&#42;&#42;For information on Adobe Workfront Fusion licenses, see [Adobe Workfront Fusion licenses](../../workfront-fusion/get-started/license-automation-vs-integration.md)

## Prerequisites

To use Intacct modules, you must have an Intacct account.

## Connect Intacct to Workfront Fusion

### Authorizing Workfront Fusion to make changes in Intacct

Before Workfront Fusion can connect to Intacct, you must authorize it.

In your Intacct account, navigate to the **Company** tab.

1. Click **Company Info**.
1. Navigate to the **Security** tab.
1. Click Edit in the upper-right corner
1. Select Web Services Authorizations.
1. Click the plus icon
1. Enter AzuquaMPP as the sender_id.
1. (Optional) Enter a description for the connection

### Set up a connection in Workfront Fusion {#set-up-a-connection-in-workfront-fusion}

You can create a connection to your Intacct account directly from inside a Intacct module.

1. In any Intacct module, click **Add** next to the Connection field.
1. Enter your Intacct credentials

   * Company ID
   * User ID
   * Password

1. Click **Continue** to create the connection and go back to the module.

## Intacct modules and their fields

When you configure Intacct modules, Workfront Fusion displays the fields listed below. Along with these, additional Intacct fields might display, depending on factors such as your access level in the app or service. A bolded title in a module indicates a required field.

If you see the map button above a field or function, you can use it to set variables and functions for that field. For more information, see [Map information from one module to another in Adobe Workfront Fusion](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

### Make a custom API call

This action module lets you make a custom authenticated call to the Intacct API. This way, you can create a data flow automation that can't be accomplished by the other Intacct modules. 

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>Connection</p> </td> 
   <td> <p>For instructions about connecting your Intacct account to Workfront Fusion 2.0, see <a href="#set-up-a-connection-in-workfront-fusion" class="MCXref xref">Set up a connection in Workfront Fusion</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Body XML</td> 
   <td> <p>Include only the XML inside the body. The request will automatically include authentication headers.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Search records

This search module retrieves a list of records that match specific search criteria.

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>Connection</p> </td> 
   <td> <p>For instructions about connecting your Intacct account to Workfront Fusion 2.0, see <a href="#set-up-a-connection-in-workfront-fusion" class="MCXref xref">Set up a connection in Workfront Fusion</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Record type</td> 
   <td> <p>Select the type of record you want to search.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Search criteria</p> </td> 
   <td> 
    <ul> 
     <li> <p>Select the field by which you want to search</p> </li> 
     <li> <p>Select the operator that you want to use for the search</p> </li> 
     <li> <p>Enter the value that you want to search for</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Result set</td> 
   <td>Select whether you want to return all matching records, or only the first matching record.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Limit</td> 
   <td> <p>Enter or map the maximum number of records you want the module to return during each scenario execution cycle.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Sort by</td> 
   <td>Select the field you want to sort the results by. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Order</td> 
   <td>Select whether you want to sort ascending or descending.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Outputs</td> 
   <td> <p>Select the information you want included in the output bundle for this module.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Case sensitivity</td> 
   <td>Enable this option to make your query case-sensitive.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Query into private entities</td> 
   <td>Enable this option to allow the module to search private entities.</td> 
  </tr> 
 </tbody> 
</table>

