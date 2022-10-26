**Nesting** involves putting arrays and objects inside each other, creating multiple layers of collections.

You can put arrays inside objects, objects inside arrays, arrays inside arrays, etc.

Sometimes a JSON file is one big object with lots of objects and arrays inside of that one top-level object.

**An array of objects:**

```json
[
   "object",
   "object",
   "object"
]
```

**An array of objects with values:**

```json
[
   {
      "name":"Ike",
      "age":33
   },
   {
      "name":"Cheryl",
      "age":21
   },
   {
      "name":"Joey",
      "age":55
   }
]
```

**An object with an array in the value part of the key-value pair:**

```json
{
   "children":[
      "Mike",
      "Katie",
      "Tony",
      "Sally"
   ],
   "hobbies":[
      "running",
      "jumping",
      "hiking",
      "biking"
   ]
}
```

***

##### Sources
- [Documenting APIs: A guide for technical writers and engineers](https://idratherbewriting.com/learnapidoc/) by Tom Johnson
- [Learn API Technical Writing: JSON and XML for Writers](https://www.udemy.com/course/api-documentation-1-json-and-xml/) by Peter Gruenbaum

