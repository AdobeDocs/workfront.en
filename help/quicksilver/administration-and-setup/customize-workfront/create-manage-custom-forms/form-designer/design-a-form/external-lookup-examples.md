---
title: Examples of the External Lookup Field in a Custom Form
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: An External lookup field in a custom form calls an external API and returns values as options in a dropdown field. This article provides examples of using the External lookup field to call the same instance of Workfront or a public API.
author: Lisa
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: 13880fcb-8523-45d2-9ac6-38453e8e2391
---
# Examples of the External lookup field in a custom form

An External lookup field in a custom form calls an external API and returns values as options in a dropdown field. Users who work with the object the custom form is attached to can select one or more of these options from the dropdown.

This article provides examples of using the External lookup field to call the same instance of Workfront or a public API. You can also use the External lookup to communicate with an external system such as Jira, Salesforce, or ServiceNow.

For more information about adding an External lookup field to a custom form and additional definitions of the external lookup components, see [Create a custom form](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

## Access requirements

+++ Expand to view access requirements for the functionality in this article.

You must have the following access to perform the steps in this article:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Adobe Workfront plan </td> 
   <td>Any</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license</td> 
   <td>
   <p>New: Standard</p>
   <p>or</p>
   <p>Current: Plan</p></td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Access level configurations</td> 
   <td>Administrative access to custom forms </td> 
  </tr>  
 </tbody> 
</table>

For more detail about the information in this table, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Set up an External lookup field for the same instance of Workfront

You can use the External lookup to bring data from your Workfront instance into the custom form.

### Use native Workfront field values in the External lookup

This example demonstrates how to call the Workfront API and populate a list of projects in an External Lookup field, filtered by status using the value of the "Status Query" custom field and a search term via $$QUERY.

1. Open the custom form.
1. On the left side of the screen, find **External lookup** and drag it to a section on the canvas.
1. Enter the **Label** and **Name** for the field.
1. Select the **Format** for the field.
1. Enter the API call in the **Base API URL** field.

   * Use $$HOST to reference the same instance of Workfront where the custom form is.
   * Use $$QUERY to dynamically filter the results based on user input.

   **Example API call**
   `$$HOST/attask/api/v15.0/project/search?status={DE:Status Query}&description=$$QUERY`

1. Review the **Dependencies** for the fields referenced in the API call.

   A dependency field can be any custom or native field available on the object. For example, when you're creating a custom form for groups that includes an external lookup field, dependency fields can include any fields available on a group.

   In this example, `{DE:Status Query}` will be dynamically replaced with the value of the "Status Query" custom field for the current group. So, when the form is attached to Group A, `{DE:Status Query}` is replaced with the value set in the "Status Query" field for that group.

1. Select the **HTTP Method**.

   This will mostly likely be **Get**.

1. Enter the **JSON Path** to get the results from your API call.
   
   **Example**
   `$.data[*].name`

   >[!NOTE]
   >
   >**Header** information is not required for a call to the same Workfront instance.

1. Click **Apply**.

   ![Setup of API call to Workfront in custom form](assets/external-lookup-to-workfront.png)

   When the custom form is added to a Workfront object (in this example, a project), it looks similar to this.

   ![Custom form with external lookup field](assets/external-lookup-project-status-example1.png)

   ![External lookup options based on status](assets/external-lookup-project-status-example2.png)

### Use custom field values in the External lookup

This example shows you to call the Workfront API and bring data from a custom field into your External lookup field. The example custom field is called "Custom Colors."

1. Open the custom form.
1. On the left side of the screen, find **External lookup** and drag it to a section on the canvas.
1. Enter the **Label** and **Name** for the field.
1. Select the **Format** for the field.
1. Enter the API URL call in the **Base API URL** field.

   **Example**
   `$$HOST/attask/api/v18.0/PORT/search?ID={portfolioID}&fields=parameterValues`

1. Review the **Dependencies** for the fields that this lookup field is referencing in the API.

   A dependency field can be any custom or native field existing in the object's details page.

1. Select the **HTTP Method**.

   This will mostly likely be **Get**.

1. Enter the **JSON Path** to get the results from your API call.
   
   **Example**
   `$.data[*].parameterValues.["DE:Combo Colors"]`

   * "parameterValues" refers to any custom field in Workfront for the object you're on.
   * For this example, "DE:Combo Colors" is the specific custom field containing the values you want to retrieve.

   >[!NOTE]
   >
   >**Header** information is not required for a call to the same Workfront instance.

1. Click **Apply**.

   When the custom form is added to a Workfront object, all of the values in the "Combo Colors" field appear in the External lookup field dropdown.

## Set up an External lookup field for the Workfront Planning API

An endpoint is available in the Workfront Planning API to search records by record type ID through the Get method. You can use this endpoint to reference Planning records in External lookup fields.

* **Base API URL:** `$$HOST/maestro/api/v1/records/search?recordTypeId={recordTypeID}`
* **HTTP Method:** Get
* **JSON Path:** `$.records[*].data.{fieldID}`
  
  **{fieldID}** is the field to display in the External lookup search results on the custom form for end users.

For more information, see [Workfront Planning API](/help/quicksilver/planning/general/planning-api-basics.md). 

## Set up an External lookup field for a public API

You can use the External lookup to call an external, public API and retrieve data.

This example shows how to call an API of countries (such as <https://api.first.org/data/v1/countries>) so that you don't have to hard code all of the country names in the dropdown options.

1. Open the custom form.
1. On the left side of the screen, find **External lookup** and drag it to a section on the canvas.
1. Enter the **Label** and **Name** for the field.
1. Select the **Format** for the field.
1. Enter the API URL call in the **Base API URL** field.

   * You can add $$QUERY to implement query filtering for your end users.

   **Examples**
   Lists all countries: <https://api.first.org/data/v1/countries>

   Allows the user to search for any country in the dropdown field: <https://api.first.org/data/v1/countries?q=$$QUERY>

   Allows the user to search for a country in a region: <https://api.first.org/data/v1/countries?region={DE:Region}&q=$$QUERY>

     * The available regions are defined in a separate custom field in Workfront.
     * When the user selects a region on the form, then the External lookup field shows only the countries in that region (which country is in which region is defined in the API). The user can also search for a country in the selected region.

1. Review the **Dependencies** for the fields that this lookup field is referencing in the API.   

   A dependency field can be any custom or native field existing in the object's details page.

   In this example, the `{DE:Region}` will be replaced with the value of the Region custom field.

1. Select the **HTTP Method**.

   This will mostly likely be **Get**.

1. Enter the **JSON Path** to get the results from your API call.

   This option allows extracting data from the JSON returned by the API URL. It serves as a way to select which values from inside the JSON will appear in the dropdown options.
   
   **Example**
   `$.data[*].country`

1. (Optional) Click **Add Header**, and type or paste the key-value pair required for authentication with the API.

   >[!NOTE]
   >
   >The Header fields are not a secure place to store credentials, and you should be careful of what you enter and save.

1. (Optional) Select **Multi-Select Dropdown** to allow the user to select more than one value in the dropdown.

1. Click **Apply**.

   ![Setup of API call to public API in custom form](assets/external-lookup-to-api-for-countries.png)

   When the custom form is added to a Workfront object (in this example, a project), it looks similar to this.

   ![Custom form with external lookup field](assets/external-lookup-countries-example1.png)

   ![External lookup options for a country based on region](assets/external-lookup-countries-example2.png)

## Additional use cases for External lookup fields

There are many other use cases for creating an External lookup.

**Use case:** Replace typeahead fields, because they can cause problems with reporting.
**Solution:** Use an API call to existing objects in the system.

   Example Base API URL for templates, to replace a typeahead field:
   `$$HOST/attask/api/v17.0/tmpl/search?isActive=true&name_Sort=asc`

**Use case:** Create dropdown fields with more features (for example, there is line wrap in the External eookup field).
**Solution:** Use an API call to existing objects in the system, or create a new object and use an API call to this object.

**Use case:** Define a way for users to maintain their own fields outside of the custom forms area. Set up the External lookup field and you can give users to the objects that comprise the field. This option is good for high maintenance fields and teams.
**Solution:** Create a new object and use an API call to this object.

**Use case:** Integration with objects outside of Workfront. For example, accessing another system to get the name of every user, rather than being restricted in a typeahead field.
**Solution:** Webhook/Fusion automation to connect to other systems.

