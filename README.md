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

Zone based weather 
------------------------------------------------------------
The weather services that I tried in HA all seemed to use a location that is defined during their installation for accessing weather data.  This doesn't really work on a "home" that moves around. This weather station is built using the Rest sensor platform in HA to get the weather data from Open Weather Map. Using the Rest platform enables the weather data to accessed using a zones location.

![victron-sensors](./docs/assets/weather.jpg)
