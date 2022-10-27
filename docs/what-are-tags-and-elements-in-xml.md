# What are tags and elements in XML?
XML holds structured data. That data is enclosed in **tags**. A tag starts with `<` and ends with `/>`.

XML has three types of tags:

- **Start tags**, such as `<start>`
- **End tags**, such as `</start>`
- **Empty-element tags**, such as `<line-break />`

Start tags and end tags must match. For every starting tag, there must be an end tag for it. Empty-element tags are an exception.

Tag names must start with letters, and can only contain letters, numbers, and underscores.

!!! example

    ```xml
    <city>New York</city>
    <age>23</age>
    <enabled>false</enabled>
    ```

**Content** is what's stored in between tags. Content can be *nested*, with tags inside of tags.

!!! example
    ```xml
    <color>
        <red>205</red>
        <green>123</green>
        <blue>52</blue>
    </color>
    ```

## What is an element?
Elements refer to tags and the content within tags. An empty-element tag is also considered an element.

!!! note

    This is different from JSON, where an element is an object.

*[XML]: Extensible Markup Language
*[HTML]: HyperText Markup Language
*[JSON]: JavaScript Object Notation
*[HTTP]: Hypertext Markup Language    

***

##### Sources
- [MDN Web Docs](https://developer.mozilla.org/en-US/)
- [Learn API Technical Writing: JSON and XML for Writers](https://www.udemy.com/course/api-documentation-1-json-and-xml/) by Peter Gruenbaum
- [W3 Schools](https://www.w3schools.com/xml/default.asp)
