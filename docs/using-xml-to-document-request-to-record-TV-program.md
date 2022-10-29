# Using XML to document a request to record a TV program (part 1)

Let's say we have an API that sends requests to record a TV program with XML:

```xml
<recordTV>
	<date>2015-06-01</date>
	<time format="24">18:00</time>
	<duration>1.5</duration>
	<channel>54</channel>
</recordTV>
```

We can document this data in a table:

Represents a request to record a television program.
 
| Element | Description | Type | Required | Notes |
| --- | --- | --- | --- | --- |
| recordTV | Top level | TV program data | Required | |
| &nbsp; &nbsp; date | Date of the program | string | Optional | Format is YYYY-MM-DD HH:MM:SS. Default value is today's date. |
| &nbsp; &nbsp; time | Time the program begins | number | Required | Attributes: **format** has values `24` or `12` for 24 or 12 hour formats. Format is HH:MM, with am or pm afterwards for 12 hour format |

# Using XML to document a request to record a TV program (part 2)

Let's say we have a different request to record a TV program. This time the XML has attributes:

```xml
<recordTV>
	<when date="2015-06-01" time="18:00" format="24"/>
	<duration hours="1.5"/>
	<station channel="54"/>
</recordTV>
```

We can also document this data in a table:

Represents a request to record a television program.
 
| Element | Attribute | Description | Type | Required | Notes |
| --- | --- | --- | --- | --- | --- |
| recordTV | | Top level | TV program data | Required | |
| &nbsp; &nbsp; when | | Date and time when the program starts | | Required |  |
|  | date | Date | string | Optional | Format is YYYY-MM-DD. Default value is today's date. |
|  | time | Time the program begins | string | Required | Format is HH:MM, with am or pm afterwards for 12 hour format |
|  | format | Format for the time: either 12 hour or 24 hour | string | Required| Valid values: `24` or `12`  |
| &nbsp; &nbsp; duration | hours | Length of the program | number | Required | In hours |
| &nbsp; &nbsp; station | channel | Channel to record | number | Required | |

*[XML]: Extensible Markup Language
*[HTML]: HyperText Markup Language
*[JSON]: JavaScript Object Notation
*[HTTP]: Hypertext Markup Language

***

##### Sources
- [Learn API Technical Writing: JSON and XML for Writers](https://www.udemy.com/course/api-documentation-1-json-and-xml/) by Peter Gruenbaum