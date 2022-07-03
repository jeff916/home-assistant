# My Home Assistant Setup
These configuration files are my current effort in configuring HA for use in a van build.
I'm working on implimenting:
- [x] Modbus interface for Victron Energy components
- [ ] Lighting control
- [ ] Various automations for lighting, battery monitoring, water heater, etc.

Victron Energy Modbus 
------------------------------------------------------------
I'm using the Modbus interface avaiable via the CCGX to get infromatoin from the Victron Energy components; BMV-702, BlueSolar MPPT and a MultiPlus Inverter into Home Assistant.

![victron-sensors](./docs/assets/victron-sensors.jpg)

More Info: [Victron Modbus](docs/victron-modbus.md)

Zone based weather data
------------------------------------------------------------
A simple weather station that uses [OpenWeatherMap](https://openweathermap.org) as a source for current meteorological data for the location of a HA zone. Perfect for those that have a “home” that travels. Update the location of your home zone and the meteorological data is updated to the new location. 

![victron-sensors](./docs/assets/weather.jpg)

More Info: [My OWM weather station](docs/myowmstation.md)
