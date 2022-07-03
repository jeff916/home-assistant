# **My Weather Station**

The weather service integrations that I tried in HA all seem to use the location that is defined during installation for weather data. This doesn't really work on a "home" that moves. This weather station is built using the Rest sensor platform in HA to get the weather data from Open Weather Map. Using the Rest platform enables youe change your location for the weather. All that ones needs to do is update the zone to your current location.

My Weather Station configuration is defined with 2 files:
- The sensors/weather.yaml file contains the configuration for the rest Open Weather Map sensor.
- The my-weather-station.yaml file maps the data from the Open Weahter Map service to the HA Weather object

I’ve split up my configuration into multiple files to help keep it a bit more manageable. My Sensor configuration is stored in a sensors folder with multiple files for different sensor definitions. If you use this approach then you can include the files for the weather station by including the following in your configuration.yaml file.
```

sensor: !include_dir_merge_list sensors
weather: !include my-weather-station.yaml

```
