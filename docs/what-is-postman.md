# What is Postman?

**Postman** is an API platform for building and using APIs, and generating API documentation.

Postman is known as a **GUI REST client**, meaning it has a graphical user interface and can invoke REST services.

For this exercise, we will use Postman to make a `GET` request for the weather using the [OpenWeatherMap API](https://openweathermap.org/api).

To use this API, you must create an account and create an `API key`.

## How to make a request with Postman

1. Download and install Postman.
2. Open Postman.
3. Click **New**.
4. Click **HTTP Request**.
5. Insert the following endpoint into the empty box ("Enter request URL") next to **GET**:

    `https://api.openweathermap.org/data/2.5/weather`

6. Click on the tab labelled **Params** (parameters). It should be displayed by default.
7. Add the following parameters in the respective **key** and **value** rows:

    - **key**: `zip` / **value**: `28215`
    - **key**: `units` / **value**: `imperial`
    - **key**: `appid` / **value**: / `e326886bb536c5eac65ccc70df1067bb`

    **Note**: When you add these parameters, they appear as a query string to the endpoint URL in the **GET** box. The endpoint now looks like this:
    
    `https://api.openweathermap.org/data/2.5/weather?zip=28215&units=imperial&appid=e326886bb536c5eac65ccc70df1067bb`

8. Click **Send**.

    The response (in JSON) appears in the lower pane:

```json
{
   "coord":{
      "lon":-80.7387,
      "lat":35.244
   },
   "weather":[
      {
         "id":803,
         "main":"Clouds",
         "description":"broken clouds",
         "icon":"04d"
      }
   ],
   "base":"stations",
   "main":{
      "temp":56.53,
      "feels_like":55.74,
      "temp_min":54.23,
      "temp_max":59.4,
      "pressure":1026,
      "humidity":82
   },
   "visibility":10000,
   "wind":{
      "speed":8.05,
      "deg":10
   },
   "clouds":{
      "all":75
   },
   "dt":1665408709,
   "sys":{
      "type":2,
      "id":2011045,
      "country":"US",
      "sunrise":1665401084,
      "sunset":1665442490
   },
   "timezone":-14400,
   "id":0,
   "name":"Charlotte",
   "cod":200
}
```

## How to make the same request with curl

1. In Postman, click on the code (**< / >**) button.
2. Below **Code Snippet**, select **cURL** from the dropdown.
3. Copy the code using the **Copy snippet** button.
4. Paste the code into the command line.
5. Replace the single-quotes around the hyperlink with double-quotes to avoid an error message:

   `curl --location --request GET "https://api.openweathermap.org/data/2.5/weather?zip=28215&units=imperial&appid=e326886bb536c5eac65ccc70df1067bb"`

!!! success   
   
   The unminified (unformatted) response should look like this:
   
   ```json
   {"coord":{"lon":-80.7387,"lat":35.244},"weather":[{"id":802,"main":"Clouds","description":"scattered clouds","icon":"03d"}],"base":"stations","main":{"temp":64.02,"feels_like":63.32,"temp_min":60.94,"temp_max":66.99,"pressure":1027,"humidity":68},"visibility":10000,"wind":{"speed":10.36,"deg":70},"clouds":{"all":40},"dt":1665416552,"sys":{"type":2,"id":2011045,"country":"US","sunrise":1665401084,"sunset":1665442490},"timezone":-14400,"id":0,"name":"Charlotte","cod":200}
   ```

## How to save a request with Postman
1. In Postman, click the **Save** button. It is above the **Send** button.
2. In the **Request name** box, replace the endpoint with: `OpenWeatherMap Current API`.
3. Click the **Add Description** box.
4. Type a description: “gets the current weather for 28215 in imperial units.”
5. Scroll down and click **New Collection** to create a new folder to save the request in.
6. Type the name of your new collection (“OpenWeatherMap”) in the **Name your collection** box.
7. Click **Create**.
8. Click the orange **Save** button.

!!! success

   The request has been saved and will now appear in the left-side pane in the **Collections** tab.

## How to create a Run in Postman button
1. Click on the **Collections** tab in the left-side pane.
2. Next to the collection name, select the *more actions* icon (three dots) and then click **Share**.
3. Click on the **Via Run in Postman** tab.
4. Click **Embed a static version**.
5. Click on the **Markdown friendly** option.
6. Click **Copy code** and embed the code below:

   [![Run in Postman](https://run.pstmn.io/button.svg)](https://app.getpostman.com/run-collection/d95c183e4c7fce5c07fb?action=collection%2Fimport)

***

##### Sources
- [Documenting APIs: A guide for technical writers and engineers](https://idratherbewriting.com/learnapidoc/) by Tom Johnson
- [Postman Learning Center](https://learning.postman.com/)