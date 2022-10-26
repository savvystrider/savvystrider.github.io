# Mock surf report API documentation

## Surfreport

Provides data about surfing conditions, including surf height, wind, tide, and water temperature, as well as an overall recommendation for going surfing.

## Endpoints

**GET** surfreport/`{beachId}`

Gets the surf conditions for a specific beach ID.

## Parameters

### Path parameters

| Path parameter | Description |
| -- | -- |
| `{beachId}` | The value for a specific beach. Valid `beachId` values can be found at: https://example.com/surfreport/beaches_available. |

### Query string parameters

| Query string parameter | Required / Optional | Description | Type |
| -- | -- | -- | -- |
| `days` | Optional | The number of days to include in the response. The default is 3. The maximum is 7. | Integer |
| `units` | Optional | Valid values are imperial or metric. The default is imperial. | Integer |
| `time` | Optional | If you include the time, then only conditions for the specified hour will be included in the response. | Integer. Unix format (ms since 1970) in GMT or UTC. |

## Sample request

```html
curl -I -X GET "https://api.openweathermap.org/data/2.5/surfreport?&appid=APIKEY&zip=95050&units=metric&days=2"
```

(In the above curl request, replace `APIKEY` with your unique API key.)

## Sample response

The following is a sample response from the `surfreport/{beachId}` endpoint:

```json
{
    "surfreport": [
        {
            "beach": "Santa Cruz",
            "monday": {
                "1pm": {
                    "tide": 5,
                    "wind": 15,
                    "watertemp": 80,
                    "surfheight": 5,
                    "recommendation": "Go surfing!"
                },
                "2pm": {
                    "tide": -1,
                    "wind": 1,
                    "watertemp": 50,
                    "surfheight": 3,
                    "recommendation": "Surfing conditions are okay, not great."
                },
                "3pm": {
                    "tide": -1,
                    "wind": 10,
                    "watertemp": 65,
                    "surfheight": 1,
                    "recommendation": "Not a good day for surfing."
                }
                ...
            }
        }
    ]
}
```

### Response definitions

The following table describes each item in the response.

| Response item | Description | Data type |
| -- | -- | -- |
| `beach` | The selected beach based on the beach ID provided in the request. | String |
| `{day}` | The selected day of the week. A minimum of 3 days gets returned in the response. A maximum of 7 days can be returned in the response. | Object |
| `{time}` | The time of the day for surf conditions. Only included if specified as a parameter in the request. | String |
| {day}/{time}/`tide` | The level of tide at the beach for a specific day and time. Can be a positive or negative number, or 0. | Integer |
| {day}/{time}/`wind` | The wind speed at the beach, measured in knots (nautical miles per hour). High wind speeds result in undesireable surf conditions. | Integer |
| {day}/{time}/`watertemp` | The temperature of the water, returned in either degrees Fahrenheit or Celsius, depending on specified units. | Integer |
| {day}/{time}/`surfheight` | The height of the waves, returned in either feet or centimeters, depending on specified units. High surf height results in undesireable surf conditions. | Integer |
| {day}/{time}/`recommendation` | An overall recommendation for surfing. The recommendation is based on an algorithm for optimal surf conditions and includes one of three responses: (1) "Go surfing!, (2) "Surfing conditions are okay, not great", and (3) "Not a good day for surfing." | String |


***

##### Source
- [Documenting APIs: A guide for technical writers and engineers](https://idratherbewriting.com/learnapidoc/) by Tom Johnson