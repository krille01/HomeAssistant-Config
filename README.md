# Krille01's Home Assistant Config files
Here is the configuration files for my [Home Assistant](https://home-assistant.io) configuration files. Most of the setup is inspired of some great Home Assistant configuration around here on github and from youtube videos. Some of the stuff are in norwegian but trying to comment etc. in english. My Homme Assistant is under constantly build and changes. I wil try to update the configuration here as often as I got the time. Feel free to send any question to kfosserud@gmail.com.

![My Home Automation Setup](https://github.com/krille01/HomeAssistant-Config/blob/master/images/lovelace/lovelace_images.gif)

## <a name="Home Assistant Hardware and Software">Hardware</a>

* Intel NUC Gen 8 i3 with 8GB of ram
* Running Proxmox as base system on the NUC
* VM in Proxmox with HassOS 4.11
* Home Assistant Core 0.114.4
                                                                              
## <a name="Network">Network</a>                                                                                                     

| Device  | Quantity | Connection | Home Assistant | Notes |
| ------------- | :---: | ------------- | ------------- | ------------- |
| Google Wif | 4 | Cabel/Wifi | [Google Wifi](https://www.home-assistant.io/integrations/google_wifi/)| To get wifi all over the hosue|
| Tp Link Switch | 2 | Cabel | | Google Wifi has only one Lan port |

## <a name="Voice Assistant">Voice_Assistant</a>

| Device  | Quantity | Connection | Home Assistant | Notes |
| ------------- | :---: | ------------- | ------------- | ------------- |
| Google Home | 2 | Wifi| [Google Home](https://www.home-assistant.io/integrations/google_assistant/)| Is used for playing music and play aunouncment from Home Assistant|
| Google Home mini | 4 | Wifi | [Google Home](https://www.home-assistant.io/integrations/google_assistant/) | Manly used to play music in the bedrooms |

I have also bought one Amazone Echo DOT for testing. I wil come back with more when this also is implemented in Home Assistant.

## <a name="Hubs/Controllers">Hubs</a>

| Device  | Quantity | Connection | Home Assistant | Notes |
| ------------- | :---: | ------------- | ------------- | ------------- |
| [IKEA TRÅDFRI](https://www.ikea.com/us/en/p/tradfri-gateway-white-00337813/)| 1 | Ethernet | [IKEA TRÅDFRI](https://www.home-assistant.io/integrations/tradfri/) | This was the first hub i bought for my home automation, Curently not used any more|
| [TELLSTICK ZNET LITE V2](https://telldus.com/produkt/z-wave-gateway-tellstick-znet-lite-ver-2/)| 1 | Ethernet | [MQTT](https://www.home-assistant.io/integrations/mqtt/)| I do not use the official integration any more, as this did not work fast enough. Has instead added an app as with mqtt|
| [VERISURE SMART HOME HUB](https://mypages.verisure.com/no/webshop.html#product/1178)| 1 | Ethernet | [Verisure](https://mypages.verisure.com/no/webshop.html#product/1178) | To comunicate with my Yale Doorman |
| [ConBeeII USB Stick](https://phoscon.de/en/conbee2) | 1 | USB | [add-on for deCONZ](https://www.home-assistant.io/integrations/deconz/)| Is used for connect all my Zigbee diveces to Home Assistant|
| [Broadlink RM3 Pro](https://www.amazon.com/BroadLink-Cable-WiFi-Automation-RM4-pro/dp/B0872P4HX7/ref=sr_1_5?crid=3P51RKXMTUZ2Y&dchild=1&keywords=broadlink+rm+pro+3&qid=1596715143&sprefix=broadlink+rm+pro+3%2Caps%2C249&sr=8-5) | 1 | Wifi/IR/RF | [Broadlink](https://www.home-assistant.io/integrations/broadlink/) | I use this in Node-Red for controlling my Blinds|

## <a name="Lights">Lights</a>

| Device  | Quantity | Connection | Home Assistant | Notes |
| ------------- | :---: | ------------- | ------------- | ------------- |
| [FLOALT LED](https://www.ikea.com/gb/en/p/floalt-led-light-panel-dimmable-white-spectrum-90436314/)| 4 | Zigbee | [deCONZ](https://www.home-assistant.io/integrations/deconz/)| Cealing lamps connected to ConbeeII stick|
| [TRÅDFRI LED bulb E27](https://www.ikea.com/gb/en/p/tradfri-led-bulb-e27-806-lumen-wireless-dimmable-warm-white-warm-white-globe-opal-white-90408797/) | 2 | Zigbee| [deCONZ](https://www.home-assistant.io/integrations/deconz/)| Bulbs connected to ConbeeII Stick 
| [TRÅDFRI LED bulb E14](https://www.ikea.com/gb/en/p/tradfri-led-bulb-e14-470-lumen-wireless-dimmable-white-spectrum-white-spectrum-wireless-dimmable-chandelier-opal-white-chandelier-opal-white-70424312/)| 3 | Zigbee | [deCONZ](https://www.home-assistant.io/integrations/deconz/)| Connected in a group i deCONZ|
| [TRÅDFRI LED bulb GU10](https://www.ikea.com/gb/en/p/tradfri-led-bulb-gu10-400-lumen-wireless-dimmable-white-spectrum-90408603/)| 3 | Zigbee | [deCONZ](https://www.home-assistant.io/integrations/deconz/)| Connected in a group in deCONZ|
| [NEXA BUILD IN DIMMER](https://nexa.se/smarta-hem/systemnexa/inbyggnadsmottagare/cmr101)| 3 | RF 433 Mhz | [MQTT](https://www.home-assistant.io/integrations/mqtt)| This is used to control lights and comunicates with the Tellstick hub and from there to Home Assistant with MQTT|
| [NEXA ON/OFF Switch](https://nexa.se/smarta-hem/systemnexa/inbyggnadsmottagare/lcmr1000)| 1 | RF 433 Mhz | [MQTT](https://www.home-assistant.io/integrations/mqtt)| This is used to control lights and comunicates with the Tellstick hub and from there to Home Assistant with MQTT|
| [SONOFF Mini](https://www.amazon.com/Wireless-Universal-Automation-Compatible-Assistant/dp/B07TRSWY23/ref=sr_1_3?dchild=1&keywords=sonoff+mini&qid=1596715682&sr=8-3)| 1 | WiFI | [ESPHome](https://www.home-assistant.io/integrations/esphome/)| Flashed with ESPHome firmware|

## <a name="Switches">Switches</a>

| Device  | Quantity | Connection | Home Assistant | Notes |
| ------------- | :---: | ------------- | ------------- | ------------- |
| [Aqara Smart Light Switch](https://www.gearbest.com/alarm-systems/pp_610095.html?wid=1527929)| 1 | Zigbee | [deCONZ](https://www.home-assistant.io/integrations/deconz/) | The configuration for this switch is actually in [Appdaemon](https://appdaemon.readthedocs.io/en/latest/#)|
| [Aqara Cube](https://www.gearbest.com/access-control/pp_1845856.html?wid=1433363)| 1 | Zigbee | [deCONZ](https://www.home-assistant.io/integrations/deconz/) | This i only tested for fun. Not in dailu use |
| [TRÅDFRI Remote control](https://www.ikea.com/gb/en/p/tradfri-remote-control-30443124/)| 3 | Zigbee | [deCONZ](https://www.home-assistant.io/integrations/deconz/) | Connected to the ConbeeII Stick|
| [TRÅDFRI Wireless dimmer](https://www.ikea.com/gb/en/p/tradfri-wireless-dimmer-white-00468432/) | 2 | Zigbee | [deCONZ](https://www.home-assistant.io/integrations/deconz/)| Connected to the ConbeeII Stick |
| [DIY HA SwitchPlate](https://community.home-assistant.io/t/ha-switchplate-diy-lcd-touchscreen-wall-switch-replacement/25464)| 2 | Wifi/MQTT | [MQTT](https://www.home-assistant.io/integrations/mqtt/)| This is a DIY Project from [Allen Derusha](https://github.com/aderusha)|

## <a name="Sensors">Sensors</a>

| Device  | Quantity | Connection | Home Assistant | Notes |
| ------------- | :---: | ------------- | ------------- | ------------- |
| [Aqara Temperature Humidity Sensor](https://www.gearbest.com/access-control/pp_626702.html?wid=1433363)| 3 | Zigbee | [deCONZ](https://www.home-assistant.io/integrations/deconz/) | This is used for read my indoor tempratures and Humidity|

I hva some more sensors build on ESP8266 that will come in here later.

## <a name="Climate">Climate</a>

| Device  | Quantity | Connection | Home Assistant | Notes |
| ------------- | :---: | ------------- | ------------- | ------------- |
| [Mill AV600WIFI](https://www.millheat.com/mill-wifi/av600wifi) | 1 | WiFI | [Mill](https://www.home-assistant.io/integrations/mill/)| Mill Wifi is a Panel Heater that you can control from Home Assistant|
| [Systemair vtr 400 Ventilation](https://shop.systemair.com/en/top--connected/c40061)| 1 | ModBus | [Modbus](https://www.home-assistant.io/integrations/modbus/)| This is connect to Home Assistant from a Modbus to wifi bridge [ELFIN-EW11](http://www.hi-flying.com/elfin-ew1x-rs232-rs485-to-wi-fi)|


## Credits
- People ([ccostan](https://github.com/CCOSTAN/Home-AssistantConfig), [Allen Derusha](https://github.com/aderusha/HASwitchPlate), [Thomas Lovén](https://github.com/thomasloven), [Drzzs](https://drzzs.com/), [Isabella Gross Alström](https://github.com/isabellaalstrom/home-assistant-config) among many otthers) for shearing your work and contrubutions to Home Assistant.



