Previously, in Documenting a single-level response in JSON, we used a table to document a single-level JSON response.

To document nesting, you can either **indent** or **create a table for each object type**:

### Indent
- Each indent indicates a level of nesting.
    - Use the tag `&nbsp` to create an indent/space in tables.
- Best for cases where objects are not reused.
- Takes up less space.

The following JSON data is nested and represents song information:

```json
{
   "song":{
      "title":"JSON Lullaby",
      "artist":"The Instructors",
      "musicians":[
         "Jen Trainer",
         "John Teacher"
      ]
   }
}
```

We can document this data in a table:

| Element | Description | Type |
| ---- | ---- | ---- |
| song | Top level | song data object |
| &nbsp; &nbsp; title | Song title | string |
| &nbsp; &nbsp; artist | Song artist | string |
| &nbsp; &nbsp; musicians | A list of musicians that play on the song | array of string |


### Create a table for each object type
- Best for cases where objects are reused.
- Takes up more space.

See: Activity: Using JSON to Describe a Menu Structure for an example.

***

The above method is from the course [Learn API Technical Writing: JSON and XML for Writers](https://www.udemy.com/course/api-documentation-1-json-and-xml/) by Peter Gruenbaum.