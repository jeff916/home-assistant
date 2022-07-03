# **My Weather Station**

The weather service integrations that I tried in HA all seem to use the location that is defined during installation for weather data. This doesn't really work on a "home" that moves. This weather station is built using the Rest sensor platform in HA to get the weather data from Open Weather Map. Using the Rest platform enables the weather data to accessed using a zones location. All that ones needs to do us update the zone to your current location.

I’ve split up my configuration into multiple files to help keep it a bit more manageable. My Sensor configuration is stored in a sensors folder with multiple files for different sensor definitions. If you use this approach then you can use the files for the weather stations by including the following in your configuration.yaml file.
```

sensor: !include_dir_merge_list sensors
weather: !include my-weather-station.yaml

```
