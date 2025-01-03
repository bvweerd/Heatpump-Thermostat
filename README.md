# LG Heatpump-Thermostat
These scripts are made to control a LG Heatpump via Modbus using Home Assistant.

The scripts are meant as inspiration only.

## Basic 
This folder contains the basic implementation of the modbus communication and the weather dependent control line

## Hotstart
This folder contains an overshoot control for the startup of the heatpump

## Thermostat and nightmode
This folder contains a simple room thermostat with hysteresis, and a nightmode (temperature reduction) with a schedule

## Silent mode
This folder contains 2 automations to control the silent mode of the heatpump, depending on the outdoor temperature, defrost status and compressor speed. 

Efficiency increases when silent mode is off in the defrosting region. The frequency limit will prevent the heatpump to rage to high frequencies if you prefer not to. Note that if the target temperature cannot be reached in silent mode in about 12 minutes, it would be more benificial to disable the silent mode.
