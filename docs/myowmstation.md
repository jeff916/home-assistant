# **My Weather Station**

The weather service integrations that I tried in HA all seem to use the location that is defined during installation for weather data. This doesn't really work on a "home" that moves. This weather station is built using the Rest sensor platform in HA to get the weather data from Open Weather Map. Using the Rest platform enables the weather data to accessed using a zones location. All that ones needs to do us update the zone to your current location.

To include these files you need to add the following to your configuration.yaml
```

weather: !include my-weather-station.yaml

```
