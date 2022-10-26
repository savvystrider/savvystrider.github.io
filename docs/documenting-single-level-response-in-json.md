JSON with no nesting is the easiest to document because all data is one level.

For this example, we have one object in curly braces `{}` with four **key-value pairs**.

```json
{
   "firstName":"Manish",
   "lastName":"Patel",
   "age":16,
   "fullTime":true
}
```

We can document this data using a table. The columns will include:

- **Element**: the *key* in the key-value pair.

- **Description**: a sentence fragment, usually a descriptive noun.

- **Type**: number, string, Boolean, array (specify what it's an array of), or object (what kind of object)

- **Notes** (optional): additional information (omit if not necessary).

| Element | Description | Type | Notes |
| -- | -- | -- | -- |
| firstName | First name | String | |
| lastName | Last name | String | |
| age | Age, in years | Number | |
| fullTime | True, if working full-time; otherwise, false. | Boolean | Full-time is defined as 40 hours per week. |

***

The above method is from the course [Learn API Technical Writing: JSON and XML for Writers](https://www.udemy.com/course/api-documentation-1-json-and-xml/) by Peter Gruenbaum.