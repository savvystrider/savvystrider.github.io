# What are arrays and objects in JSON?

JSON has two types of basic structures: **arrays** and **objects**.

## What is an array?

An **array** is an *ordered* sequence of zero or more values enclosed in brackets `[]` and separated by commas.

**An array of numbers:**

```json
[4, 6, 23.1, -4, 0, 56]
```

**An array of strings:**

```json
["red", "green", "blue"]
```

**Mixed array with a Boolean value and a null value:**

```json
[65, "toast", true, 21, null, 100]
```

## What is an object?

An **object** is an *unordered* collection of zero or more name/value pairs enclosed in curly braces `{}` and separated by commas.

### About objects
- Objects are JSON's *dictionaries*, meaning they consist of **keys** and **values**, where you can look up a value with a given key.
- Keys and values are separated from each other with a colon.
- Key-value pairs are separated with commas.
- Keys and values can be any data type, although strings are the most common.

**An object in curly brackets that holds values for “red”, “green”, and “blue”.**

```json
{"red":205, "green":123, "blue":53}
```

- The first key is the string `"red"`, which has a value of `205`.
- Keys and values are separated by a colon.
- Key-value pairs are separated with commas.

**Data about a person:**

```json
{
   "firstName":"Manish",
   "lastName":"Patel",
   "employed":false
}
```

- `"firstName"` = key; `"Manish"` = value (string)
- `"lastName"` = key; `"Patel"` = value (string)
- `"employed"` = key; `false` = value (Boolean)

***

##### Sources
- [Documenting APIs: A guide for technical writers and engineers](https://idratherbewriting.com/learnapidoc/) by Tom Johnson
- [Learn API Technical Writing: JSON and XML for Writers](https://www.udemy.com/course/api-documentation-1-json-and-xml/) by Peter Gruenbaum
- [JSON.org](https://www.json.org/json-en.html)
- [Data Base Camp](https://databasecamp.de/en/data/json-en)