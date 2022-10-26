Previously, we documented JSON responses using a table.

To document JSON requests, we can use the same table but with an extra column called **Required**.

- When you send a request, not all elements are required.

- If an element is optional, the developer needs to know.

- Indicates if the element is necessary for the request.

The columns of the table will include:

- **Element**: the *key* in the key-value pair.

- **Description**: a sentence fragment, usually a descriptive noun.

- **Type**: number, string, Boolean, array (specify what it's an array of), or object (what kind of object)

- **Required**: choose either **required** or **optional** to make it easier for developers to read the table.

- **Notes** (optional): additional information (omit if not necessary).

### Request Example: Adding a Comment

```json
{
   "comment":{
      "userID":"mpatel",
      "discID":3989384939,
      "time":"2015-02-28 10:04:32",
      "text":"Well said, Barbara!"
   }
}
```
Note that `time` is GMT and also optional. If not included, then it uses the current time when the request is received by the server.

| Element | Description | Type | Required | Notes |
| -- | -- | -- | -- | -- |
| comment | Top level | comment data object | Required | |
| &nbsp; &nbsp; userID | ID of the user making the comment | string | Required | |
| &nbsp; &nbsp; discID | ID of the discussion that is being commented on | string | Required | |
| &nbsp; &nbsp; time | Time that the comment was posted | string | Optional | YYYY-MM-DD HH:MM:SS Greenwich Mean Time. Default is the time the comment is received by the server. |
| &nbsp; &nbsp; text | Text of the comment | string | Required | |

***

The above method is from the course [Learn API Technical Writing: JSON and XML for Writers](https://www.udemy.com/course/api-documentation-1-json-and-xml/) by Peter Gruenbaum.