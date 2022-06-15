# **Victron Modbus Configuration**

Configuration for the Victron Energy components, MultiPlus, BMV-702, BlueSolar MPPT in Home Assistant.
Below are the Victron sensors implemented by the configuration files.

![victron-sensors](./assets/victron-sensors.jpg)

The configuration is defined my 2 files:
- The victron-modbus.yaml file contains the configuration for the modbus regesters
- The VictronValueMapping.yaml files (located in the templates folder) maps numeric values to user friendly textual values. Like solar charger on/off value 1 or 4 to On or Off

Together these files implement the Victron Energy I’m currently using in my HA setup.

To include these files you need to add the following to your configuration.yaml
```
# Modbus
modbus: !include victron-modbus.yaml
        
template: !include_dir_merge_list templates
```
