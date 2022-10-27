# What are attributes in XML?

Tags in XML hold content. The tags can also have attributes as a way of holding simple data. **Attributes** contain data related to specific elements in key-value pairs.

Attributes appear in the start tag:

!!! example

    ```xml
    <tag key="value">content</tag>
    ```

In the above example:

- `<tag` is the start tag.
- `key` is the attribute.
- `value` is the value of the attribute.
- `content` is the content between the start and end tags.
- `/tag>` is the end tag.

!!! example

    ```xml
    <fileSize unit="kB">34.6</fileSize>
    ```

In the above example, the attribute is named `unit` and its value is `kB`.

*[XML]: Extensible Markup Language
*[HTML]: HyperText Markup Language
*[JSON]: JavaScript Object Notation
*[HTTP]: Hypertext Markup Language

***

##### Sources
- [MDN Web Docs](https://developer.mozilla.org/en-US/)
- [Learn API Technical Writing: JSON and XML for Writers](https://www.udemy.com/course/api-documentation-1-json-and-xml/) by Peter Gruenbaum
- [W3 Schools](https://www.w3schools.com/xml/default.asp)