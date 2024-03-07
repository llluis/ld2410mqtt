# ld2410mqtt
Daemon for ld2410 sensor reporting through MQTT on the Raspberry Pi under python3

* This code uses the [vjsyong's LD2410 Interface for Python](https://github.com/vjsyong/LD2410) code to communicate with the ld2410 sensor attached to a raspberry pi serial and report the results over MQTT.
* MQTT daemon is a modified version of [mqtt-hass-base](https://gitlab.com/ttblt-oss/hass/mqtt-hass-base).
* The daemon uses pyyaml to read an .yaml file to get information on the MQTT server to contact.

I am currently running this code on a raspberry pi zero 2 W.

## Requirements
* Python 3.7+ (tested on 3.9 and 3.12)

See [requirements.txt](requirements.txt) for the packages that are required beyond stock python3 to get this running.

## Installation
Install the necessary system dependencies:

``` sh
sudo apt-get install python3-venv python3-pip
```

Then run the install script:

``` sh
script/setup
```
