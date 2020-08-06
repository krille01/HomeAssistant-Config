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

## Voice Assistant

| Device  | Quantity | Connection | Home Assistant | Notes |
| ------------- | :---: | ------------- | ------------- | ------------- |
| Google Home | 2 | Wifi| [Google Home](https://www.home-assistant.io/integrations/google_assistant/)| Is used for playing music and play aunouncment from Home Assistant|
| Google Home mini | 4 | Wifi | [Google Home](https://www.home-assistant.io/integrations/google_assistant/) | Manly used to play music in the bedrooms |

I have also baught one Amazone Echo DOT for testing. I wil come back with more when this also is implemented in Home Assistant.
