# What are namespaces in XML?

Each tag in an XML file should have a unique name. However, you might have a tag name that means one thing in one context, but a different thing in a different context. For this, you have **namespaces** to uniquely identify the tags. 

!!! example

    ```xml
    <education:onlineCourse>
    ```
In the above example:

- `education` is the namespace.
- `onlineCourse` is the tag.
- The namespace acts as a "prefix" to the tag. They are separated by a colon.

*[XML]: Extensible Markup Language
*[HTML]: HyperText Markup Language
*[JSON]: JavaScript Object Notation
*[HTTP]: Hypertext Markup Language

***

##### Sources
- [MDN Web Docs](https://developer.mozilla.org/en-US/)
- [Learn API Technical Writing: JSON and XML for Writers](https://www.udemy.com/course/api-documentation-1-json-and-xml/) by Peter Gruenbaum
- [W3 Schools](https://www.w3schools.com/xml/default.asp)