# Krille01's Home Assistant Config files
Here is the configuration files for my [Home Assistant](https://home-assistant.io) configuration files. Most of the setup is inspired of some great Home Assistant configuration around here on github and from youtube videos. Some of the stuff are in norwegian but trying to comment etc. in english. My Homme Assistant is under constantly build and changes. I wil try to update the configuration here as often as I got the time.

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
| [IKEA TRÅDFRI](https://www.ikea.com/us/en/p/tradfri-gateway-white-00337813/)| 1 | Ethernet | [IKEA TRÅDFRI](https://www.home-assistant.io/integrations/tradfri/) | This was the first hub i baught for my home automation, Curently not used any more|
| [TELLSTICK ZNET LITE V2(https://telldus.com/produkt/z-wave-gateway-tellstick-znet-lite-ver-2/)| 1 | Ethernet | [MQTT](https://www.home-assistant.io/integrations/mqtt/)| I do not use the official integration any more, as this did not work fast enough. Has instead added an app as with mqtt|
| [VERISURE SMART HOME HUB](https://mypages.verisure.com/no/webshop.html#product/1178)| 1 | Ethernet | [Verisure](https://mypages.verisure.com/no/webshop.html#product/1178) | To comunicate with my Yale Doorman |
| [ConBeeII USB Stick](https://phoscon.de/en/conbee2) | 1 | USB | [add-on for deCONZ](https://www.home-assistant.io/integrations/deconz/)| Is used for connect all my Zigbee diveces to Home Assistant|


