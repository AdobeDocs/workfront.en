---
content-type: api;tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-api
title: Retrieve currency information for a project when currency is null
description: Retrieve currency information for a project when currency is null
author: Becky
feature: Workfront API
role: Developer
exl-id: 31ed533b-be19-4ccb-aad4-7c78e008b3e9
---
# Retrieve currency information for a project when currency is null (not assigned)

The project object with the currency field can be retrieved using the following request: 

```
GET /attask/api-internal/project/{{projectID}}?fields=currency
```

This would return the following response body:

```
{
{
"data": {
"ID": "some_project_id",
"name": "some_project_name",
"objCode": "PROJ",
"currency": "EUR"
}
}
}
```

If the currency is not set for the project, this response would include a currency with the value `null`:

```
{
{
"data": {
"ID": "some_project_id",
"name": "some_project_name",
"objCode": "PROJ",
"currency": null
}
}
}
```

If you require the currency for the project (such as for calculations), you can retrieve the default currency for the customer:

`GET /attask/api-internal/CUST/currentCustomer?fields=currency`

The response includes the currency that the user has set as default, which would be used by any projects for that customer that do not have the currency set:

```
{
"data": [
{
"ID": "some_customer_id,
"name": "some_customer_name",
"objCode": "CUST",
"currency": "USD"
}
]
}
```
