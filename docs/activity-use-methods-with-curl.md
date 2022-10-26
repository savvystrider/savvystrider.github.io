This is an activity from the Documenting APIs online course. For this activity, we will be using curl and the [Swagger Petstore](https://petstore.swagger.io/#/).

## Create a new pet

We will create a new pet by passing a JSON file with a curl command.

1. Insert the following JSON code into a text file:

```json
{
   "id":555,
   "category":{
      "id":0,
      "name":"string"
   },
   "name":"doctordog",
   "photoUrls":[
      "string"
   ],
   "tags":[
      {
         "id":0,
         "name":"string"
      }
   ],
   "status":"available"
}
```
**Note**: This information comes from the Swagger Petstore and will be passed in the `-d` (send data) parameter of the curl request.

2. Change the first `id` value to another integer and change the `name` value to another name.
3. Save the the file as `mypet.json` in a local directory.
4. Open a command prompt from the directory.
5. After your terminal or command prompt is in the same directory as your JSON file, create the new pet with the following curl request:

```html
curl -X POST --header "Content-Type: application/json" --header "Accept: application/json" -d @mypet.json "https://petstore.swagger.io/v2/pet"
```

- `X POST`: create (`POST`) a new resource.
- `--header`: include extra or custom headers.
- `Content-Type`: the type of content to submit with the *request*.
- `Accept`: the type of content we will accept in the *response*.
- `-d @mypet.json`: send data/file.

The response should look like this and contain the name of the newly created pet:

```json
{"id":555,"category":{"id":0,"name":"string"},"name":"doctordog","photoUrls":["string"],"tags":[{"id":0,"name":"string"}],"status":"available"}
```

***

## Update the name of your pet

We will change our pet's name with the update pet method.

1. Open the `mypet.json` file and change the `name` value.
2. Use the `PUT` (update) method instead of the `POST` (create) method.
3. Update the name of the pet with the following curl request:

```html
curl -X PUT --header "Content-Type: application/json" --header "Accept: application/json" -d @mypet.json "https://petstore.swagger.io/v2/pet"
``` 

The response should look like this and contain the updated pet name:

```json
{"id":555,"category":{"id":0,"name":"string"},"name":"misterdog","photoUrls":["string"],"tags":[{"id":0,"name":"string"}],"status":"available"}
```

***

## Get your pet's name by ID

We will search for our pet by passing the `id` into the `/pet/{petID}` endpoint:

1. Copy the first `id` value from the `mypet.json` file.
2. Use this curl command to get information about the pet:

```html
curl -X GET --header "Accept: application/json" "https://petstore.swagger.io/v2/pet/555"
```

The response should look like this and contain the name of the pet:

```json
{"id":555,"category":{"id":0,"name":"string"},"name":"misterdog","photoUrls":["string"],"tags":[{"id":0,"name":"string"}],"status":"available"}
```

***

## Delete your pet

We will delete our pet from the registry.

1. Delete the pet from the registry with following curl request:

```html
curl -X DELETE --header "Accept: application/json" "https://petstore.swagger.io/v2/pet/555"
```

2. The response should look like this:

```json
{"code":200,"type":"unknown","message":"555"}
```

3. Confirm the pet has been deleted from the registry with this curl command:

```html
curl -X GET --header "Accept: application/json" "https://petstore.swagger.io/v2/pet/555"
```

The response should look like this:

```json
{"code":1,"type":"error","message":"Pet not found"}
```

This activity demonstrates how to perform **CRUD** (create, read, update, delete) operations with curl requests.


***

## How import a curl request into Postman

We will confirm our pet has been deleted from the petstore registry by importing our previous curl request into Postman.

1. Open Postman.
2. Click **Import**.
3. Click **Raw text**.
4. Copy and paste the following curl request from the previous activity (**Delete your pet**).

    ```html
    curl -X GET --header "Accept: application/json" "https://petstore.swagger.io/v2/pet/555"
    ```

5. Click **Continue**.
6. The **Import Entities** tab will open.
7. Click **Import**.
8. The curl request has been converted to the following `GET` request in Postman:

    ```html
    https://petstore.swagger.io/v2/pet/555
    ```

9. Click **Send** to complete the process.

    You should see the same message from Step 4 of the previous activity (**Delete your pet**).


***

##### Sources
- [Documenting APIs: A guide for technical writers and engineers](https://idratherbewriting.com/learnapidoc/) by Tom Johnson
- [Swagger Petstore API](https://petstore.swagger.io/#/)