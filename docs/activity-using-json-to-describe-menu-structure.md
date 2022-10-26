Let's say we have the following menu design:

| File | View |
| -- | -- |
| Open | Zoom In |
| New | Zoom Out |
| Close | Original View |

We have two menu columns (**File** and **View**) that we can represent in JSON:

```json
[
   {
      "header":"File",
      "items":[
         {
            "id":"Open",
            "label":"Open"
         },
         {
            "id":"New",
            "label":"New"
         },
         {
            "id":"Close",
            "label":"Close"
         }
      ]
   },
   {
      "header":"View",
      "items":[
         {
            "id":"ZoomIn",
            "label":"Zoom In"
         },
         {
            "id":"ZoomOut",
            "label":"Zoom Out"
         },
         {
            "id":"OriginalView",
            "label":"Original View"
         }
      ]
   }
]
```


We can also represent the data in the following table:
- indentation indicates level of nesting
- `&nbsp;` is used for spaces.


| Element | Description | Type |
| -- | -- | -- |
| Top level | Menu columns | Array of menu column objects |
| &nbsp; &nbsp; header | Name of the column | String |
| &nbsp; &nbsp; items | List of menu items under the column | Array of menu items |
| &nbsp; &nbsp; &nbsp; id | ID of the menu item | String |
| &nbsp; &nbsp; &nbsp; label | Label that is displayed in the user interface | String |

We can also create separate tables for each object type:

**Menu array: Represents a menu**

| Element | Description | Type |
| -- | -- | -- |
| top level | Menu columns | Array of menu columns |

**Menu column object: Represents a column in a menu**

| Element | Description | Type |
| -- | -- | -- |
| header | The name of the column. | String |
| items | A list of menu items under the column. | Array of menu items |

**Menu item object: Represents something you can see in the menu**

| Element | Description | Type |
| -- | -- | -- |
| id | The ID of the menu item | String |
| label | The label that is displayed in the user interface | String

***

The above activity is from the course [Learn API Technical Writing: JSON and XML for Writers](https://www.udemy.com/course/api-documentation-1-json-and-xml/) by Peter Gruenbaum.