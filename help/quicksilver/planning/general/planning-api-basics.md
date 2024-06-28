---
title: 'Adobe Workfront Planning API basics'
description: The goal for the Adobe Workfront Planning API is to simplify building integrations with Planning by introducing a REST-ful architecture that operates over HTTP. This document assumes you are familiar with REST and JSON responses and describes the approach taken by the Planning API.  
hidefromtoc: yes
hide: yes
recommendations: noDisplay, noCatalog
---

# Adobe Workfront Planning API basics

The goal for the Adobe Workfront Planning API is to simplify building integrations with Planning by introducing a REST-ful architecture that operates over HTTP. This document assumes you are familiar with REST and JSON responses and describes the approach taken by the Planning API.  

A familiarity with the Workfront Planning schema will assist you in understanding the database relationships that can be utilized to pull data out of Workfront Planning for integration purposes.  

## Workfront Planning API URL 

For information about the URL that you will use to call the Workfront Planning API, see <!--<Planning API page on developers site>. -->

### Operations 

Objects are manipulated by sending an HTTP request to their unique URI. The operation to be performed is specified by the HTTP method. 

The standard HTTP methods correspond to the following operations: 

* **GET** - Retrieves an object by ID, searches for all objects by a query, runs reports, or executes named queries 
* **POST** - Inserts a new object 
* **PUT** - Edits an existing object 
* **DELETE** - Deletes an object 

For more details and examples of each operation, <!--please reference the API Guide  -->

### Field types and search modifiers used with them 

You can use modifiers and filters with fields to control what data will be returned in results. Refer to the API Guide for examples.  

Using Search Modifiers 

Workfront Planning support the following search modifiers: 

Modifier 

Example 

Description 

Possible Values 

$contains 

"fieldId": { "$contains": "product" } 

Returns records whose field value contains the filter 

"New Product Launch" 

$doesNotContain 

"fieldId": { "$doesNotContain": "product" } 

Returns records whose field value does not contain the filter 

"New Launch" 

$is 

"fieldId" : { "$is": "new product launch" } 

"fieldId" : { "new product launch" } 

Returns records whose field value exactly match the filter 

"New Product Launch" 

$isNot 

"fieldId": { "$isNot": "product" } 

Returns records whose field value exactly is not match the filter 

"New Product Launch" 

$isEmpty 

"fieldId": "$isEmpty" 

"fieldId": { "$isEmpty": null } 

Returns records whose field value is empty 

"" 

null 

$isNotEmpty 

"fieldId": "$isNotEmpty" 

"fieldId": { "$isNotEmpty": null } 

Returns records whose field value is not empty 

"New Product Launch" 

$greaterThan 

"fieldId": { "$greaterThan": 10 } 

Returns records whose field value is greater than the filter 

20 

25 

$greaterThanOrEqual 

"fieldId": { "$greaterThanOrEqual": 10 } 

Returns records whose field value is greater than or equal the filter 

10 

20 

25 

$lessThan 

"fieldId": { "$lessThan": 10 } 

Returns records whose field value is less than the filter, ex: 5, 9 

5 

9 

$lessThanOrEqual 

"fieldId": { "$lessThanOrEqual": 10 } 

Returns records whose field value is less than or equal the filter, ex: 5, 9, 10 

5 

9 

10 

$isAfter 

"fieldId": { "$isAfter": "2024-05-14T20:00:00.000Z" } 

Returns records whose field value is after the filter 

"2024-05-15T20:00:00.000Z" 

$isBefore 

"fieldId": { "$isBefore": "2024-05-14T20:00:00.000Z" } 

Returns records whose field value is before the filter 

"2024-05-12T20:00:00.000Z" 

$isBetween 

"fieldId": { "$isBetween": ["2024-05-10T20:00:00.000Z", "2024-05-15T20:00:00.000Z"] } 

Returns records whose field value is between the filter 

"2024-05-12T20:00:00.000Z" 

"2024-05-14T20:00:00.000Z" 

$isNotBetween 

"fieldId": { "$isNotBetween": ["2024-05-10T20:00:00.000Z", "2024-05-15T20:00:00.000Z"] } 

Returns records whose field value is not between the filter 

"2024-05-09T20:00:00.000Z" 

"2024-05-17T20:00:00.000Z" 

$isAnyOf 

"fieldId": { "$isAnyOf": ["active", "completed"] } 

Returns records whose field value is any of the filter 

"active" 

"completed" 

$isNoneOf 

"fieldId": { "$isNoneOf": ["active", "completed"] } 

Returns records whose field value is non of the filter 

"finished" 

"fixed" 

$hasAnyOf 

"fieldId": { "$hasAnyOf": ["active", "completed"] } 

Returns records whose field value has any of the filter 

["active", "fixed"] 

["fixed", "completed", "finished"] 

$hasAllOf 

"fieldId": { "$hasAllOf": ["active", "completed"] } 

Returns records whose field value has all of the filter 

["active", "completed"] 

["active", "completed", "finished"] 

$hasNoneOf 

"fieldId": { "$hasNoneOf": ["active", "completed"] } 

Returns records whose field value has none of the filter 

["fixed", "finished"] 

$isExactly 

"fieldId": { "$isExactly": ["active", "completed"] } 

Returns records whose field value is exactly the filter 

["active", "completed"] 

 

 

Field Types 

Below is the list of supported field types and what search modifiers can be used with each of those field types  

Field Type 

Supported search modifiers 

text 

$contains, $doesNotContain, $is, $isNot, $isEmpty, $isNotEmpty 

long-text 

$contains, $doesNotContain, $is, $isNot, $isEmpty, $isNotEmpty 

number 

$is, $isNot, $greaterThan, $greaterThanOrEqual, $lessThan, $lessThanOrEqual, $isEmpty, $isNotEmpty 

percentage 

$is, $isNot, $greaterThan, $greaterThanOrEqual, $lessThan, $lessThanOrEqual, $isEmpty, $isNotEmpty 

currency 

$is, $isNot, $greaterThan, $greaterThanOrEqual, $lessThan, $lessThanOrEqual, $isEmpty, $isNotEmpty 

date 

$is, $isNot, $isAfter, $isBefore, $isBetween, $isNotBetween, $isEmpty, $isNotEmpty 

single-select 

$is, $isNot, $isAnyOf, $isNoneOf, $isEmpty, $isNotEmpty 

multi-select 

$hasAnyOf, $hasAllOf, $isExactly, $hasNoneOf, $isEmpty, $isNotEmpty 

boolean 

$is 

user 

$hasAnyOf, $hasAllOf, $isExactly, $hasNoneOf, $isEmpty, $isNotEmpty 

formula 

$contains, $doesNotContain, $is, $isNot, $isEmpty, $isNotEmpty 

url 

$contains, $doesNotContain, $is, $isNot, $isEmpty, $isNotEmpty 

created-by 

$is, $isNot, $isAnyOf, $isNoneOf 

created-at 

$is, $isNot, $isAfter, $isBefore, $isBetween, $isNotBetween 

updated-by 

$is, $isNot, $isAnyOf, $isNoneOf, $isEmpty, $isNotEmpty 

updated-at 

$is, $isNot, $isAfter, $isBefore, $isBetween, $isNotBetween, $isEmpty, $isNotEmpty 

reference 

$hasAnyOf, $hasAllOf, $isExactly, $hasNoneOf, $isEmpty, $isNotEmpty 

lookup 

Depends on the linked field 

 

 

Using "And" and "Or" Statements 

In the API call you can have filters that based on several criteria combined by $and" and "$or" statements  

Example 

 

Using the Fields Request Parameter 

  

You can use the fields request parameter to specify a comma-separated list of specific fields that should be returned. These field names are case-sensitive.  

For example, the request 

  

/attask/api/v15.0/task/search?fields=plannedStartDate,priority 

returns a response similar to the following: 

  

{ 

    "priority": 2, 

    "name": "first task", 

    "ID": "4c7c08fa0000002ff924e298ee148df4", 

    "plannedStartDate": "2010-08-30T09:00:00:000-0600" } 

 

Sorting Query Results in the API 

You can sort your results by any field if you append the following to your API call: 

 Example  

 

Query limits and paginated responses 

When working with Planning API, please consider that by default, the API requests return 500 results, starting from the beginning of the list. To override the default limitation for number of results, you can use "limit" parameter in your requests and set it to a different number, up to 2000 results.  

We recommend that you consider using paginated responses for large datasets by adding "offset" parameter to your requests. Paginated responses allow you to specify the location of the first result that should be returned. For example, if you want to return the results 2001-4000, you can use the following request:  

  

For example, the below query is for returning 2000 records that are in active status, starting from the 2001st result: 

POST /v1/records/search 

  

Request body: 

{ 

    "recordTypeId": "recordTypeId", 

    "offset": "2001", 

    "limit": "2000", 

    "filters": [ 

        { "status": "active" } 

    ] 

} 

To make sure your results are properly paginated, use a sorting parameter. This allows the results to be returned in the same order, so that the pagination does not repeat or skip results. For example, to sort using the object ID, use ID_Sort=asc.  

 

Using Count   

You can use count to return the number of results that match your query.  

Example  

 