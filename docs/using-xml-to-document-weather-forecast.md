# Using XML to document a weather forecast

We can use XML to hold structured data about a weather forecast:

```xml
<?xml version="1.0" encoding="UTF-8"?>
<forecast>
    <dailyForecast>
        <date>2015-06-01</date>
        <description>sunny</description>
        <maxTemp unit="C">22</maxTemp>
        <minTemp unit="C">20</minTemp>
        <windSpeed unit="kph">12</windSpeed>
        <danger>false</danger>
    </dailyForecast>
    <dailyForecast>
        <date>2014-06-02</date>
        <description>windy</description>
        <maxTemp unit="C">22</maxTemp>
        <minTemp unit="C">20</minTemp>
        <windSpeed unit="kph">40</windSpeed>
        <danger>true</danger>
    </dailyForecast>
    <dailyForecast />
</forecast>
```

In the above example, we have a three-day forecast.

- Each day is represented by the `<dailyForecast>` tag.
- The third day is represented by an empty element: `<dailyForecast />`
- The XML here is nested, with `<forecast>` as the top-level and the `<dailyForecast>` tags as the second-level.
- The content of each tag captures weather forecast data, including the date (`<date>`), description (`<description>`), temperature (`<maxTemp>` and `<minTemp>`), wind speed (`<windSpeed>`), and alerts (`<danger>`).

***

##### Source
- [Learn API Technical Writing: JSON and XML for Writers](https://www.udemy.com/course/api-documentation-1-json-and-xml/) by Peter Gruenbaum.