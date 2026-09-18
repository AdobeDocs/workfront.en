---
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
title: Rich Text Field Storage in the API
description: If an object such as a project, issue, or task contains rich text, it is stored and accessible as a parameter value through the Workfront API.
author: Lisa
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: 2e4b18be-14bb-4d47-8e63-e2f4a5dc376f
TQID: https://experienceleague.adobe.com/lLZZugNI5odziqyz7uBMnkiVoOdGcT-jKb90j9TUG1Q
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
    internal-label: Administration
subfeature_v2:
  - id: d87de1f9-8e24-4c4d-aa4c-a403075091a1
    internal-label: Custom forms
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
    internal-label: Admin
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
---
# Rich text field storage in the API

If an object such as a project, issue, or task contains rich text, it is stored and accessible as a parameter value through the Workfront API.

Requesting text information from a project object that contains rich text can be done using the field **parameterValues**.

For example, a simple HTTP request could resemble the following:

`https://your-company.workfront.com/attask/api/v11.0/project?ID=your-project-ID&fields=parameterValues:*` 

If this example project contained a custom form with 3 custom fields: calc field, paragraph text, and rich 1. Then the above request would return a response that resembles the following, where the field "rich 1" is a rich text parameter field and the text value is "**Hello** *World!*":

```
{
    Data: {
        ID: "xxxxxxxxxxxxxxxxxxxxxxx",
        name: "new project with rich text",
        objCode: "PROJ",
        - parameterValues: {
            DE:rich 1: "{
                "blocks":[
                {
                    "key":"7eibh",
                    "text":"Hello Word!",
                    "type":"unstyled",
                    "depth":0,
                    "inlineStyleRanges":[
                    {
                        "offset":0,
                        "length":6,
                        "style":"BOLD"
                    },
                    {
                        "offset":6,
                        "length":5,
                        "style":"ITALIC"
                    }
                    ],
                    "entityRanges":[
                    ],
                "data":{
                }
                }
                ],
            "entityMap":{
            }
        }",
        DE: paragraph text: "here is some paragraph text",
        DE: calc field: "here is a calc field entry",
        }
    }
}
```

For a more in depth look at how rich text information is stored and can be retrieved through the Adobe Workfront API, see [Rich text fields in the Adobe Workfront API](../../../wf-api/general/rich-text-field-api.md).
