The new endpoint is `/surfreport/{beachId}`. This endpoint is for surfers who want to check things like tide and wave conditions to determine whether they should head out to the beach to surf. `{beachId}` is retrieved from a list of beaches on our site.

Optional parameters:

- Number of days: Max is 7. Default is 3. Optional.
- Units: imperial or metric. With imperial, you get feet and knots. With metric, you get centimeters and kilometers per hour. Optional.
- Time: time of the day corresponding to time zone of the beach you're inquiring about. Format is unix time, aka epoch. Unix time is the milliseconds since 1970. Time zone is GMT or UTC. Optional.

If you include the hour, then you only get back the surf condition for the hour you specified. Otherwise, you get back 3 days, with conditions listed out by hour for each day.

The response will include the surf height, the wind, temp, the tide, and overall recommendation.

Sample endpoint with parameters:

`https://api.openweathermap.org/com/surfreport/123?&days=2&units=metrics&hour=1400`

The response contains these elements:

surfreport:

- surfheight (units: feet)
- wind (units: kts)
- tide (units: feet)
- water temperature (units: F degrees)
- recommendation - string ("Go surfing!", "Surfing conditions okay, not great", "Not today -- try some other activity.")

The recommendation is based on an algorithm that takes optimal surfing conditions, scores them in a rubric, and includes one of three responses.

Sample format:

```json
{
    "surfreport": [
        {
            "beach": "Santa Cruz",
            "monday": {
                "1pm": {
                    "tide": 5,
                    "wind": 15,
                    "watertemp": 60,
                    "surfheight": 5,
                    "recommendation": "Go surfing!"
                },
                "2pm": {
                    "tide": -1,
                    "wind": 1,
                    "watertemp": 50,
                    "surfheight": 3,
                    "recommendation": "Surfing conditions are okay, not great"
                }
                ...

            }
        }
    ]
}
```

Negative numbers in the tide represent incoming tide.

The report won't include any details about riptide conditions.

Although users can enter beach names, there are only certain beaches included in the report. Users can look to see which beaches are available from our website at `https://example.com/surfreport/beaches_available` (not a real URL). The beach names must be url encoded when passed in the endpoint as query strings.

To switch from feet to metrics, users can add a query string of `&units=metrics`. Default is `&units=imperial`.

Here's an [example](https://www.surfline.com/) of how developers might integrate this information. This site shows the height of the surf coupled with a cam.

If the query is malformed, you get error code 400 and an indication of the error.

***

##### References
- [Documenting APIs: A guide for technical writers and engineers](https://idratherbewriting.com/learnapidoc/) by Tom Johnson
