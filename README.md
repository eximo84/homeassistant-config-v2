# homeassistant-config-v2
Second Version of Home Assistant Config including LoveLace Yaml.  Home Assistant Core runs via Docker on a custom built Debian Linux Server.

This currently only shows the raw LoveLace Yaml config, my other config files are not shared at this time as a tidy up is needed.

## Devices (including IoT):

 - iOS Devices for Location Tracking using iOS Companion App
 - Tado Smart Thermostat v3
 - Tado Smart Radiator Thermostat
 - Philips Hue Hub v2
 - Philips Hue Bulbs
 - Philips Hue Motion Sensor
 - Philips Hue Dimmer Switches
 - Ikea Tradfri Bulbs
 - NodeMCU (ESP8266) Development Boards
 - Raspberry Pi 1B Running PiHole
 - Samsung Smart TV
 - Logitech Harmony Elite Remote and Hub
 - Raspberry Pi 3B Running Kodi (OSMC)
 - Sonoff Basic: iTead WiFi Wireless Smart Switches
 - YiHome Cameras with YiHack v4 Firmware
 - CC2531 flashed with Zigbee2Mqtt
 - Xiaomi Door/Window Sensors
 - Broadlink RM Mini 3
  

 
## Home Assistant LoveLace Dashboards:

The majority of access to the LoveLace UI is done via the Home Assistant iOS App, as such an approach was taken to mimic the homekit style with buttons for each element.

#### LoveLace Custom Cards:

The following cards are used as part of my LoveLace setup:

 - [Simple Thermostat](https://github.com/nervetattoo/simple-thermostat)
 - [Mini Media Player](https://github.com/kalkih/mini-media-player)
 - [Slider Entity Row](https://github.com/thomasloven/lovelace-slider-entity-row)
 - [Mini Graph](https://github.com/kalkih/mini-graph-card)
 - [Simple Weather](https://github.com/kalkih/simple-weather-card)
 - [Button Card](https://github.com/custom-cards/button-card)
 - [Browser Mod](https://github.com/thomasloven/hass-browser_mod)

### Overview Dashboard:

 - The first section is still WIP, allows quick access to the Alarm Arming/Disarming as well as current weather forcast.
 - The second section is a conditional area where qucik buttons are viewable depending on specfic states, e.g. All Lights off toggle if any lights are currently.
 - The thrid section (main area) shows a button card for each room or device that requires control. Each card is a toggle for the respective lights/switches in that room, a long press will take you to the views page for that room which then expands out each device for more control.
 
#### Additional Pages include:

 - Media Playback showing Active Chromecast Devices
 - Video Playback including Harmony Remote activites (WIP)
 - CCTV Playback

![Overview](https://user-images.githubusercontent.com/25502878/99859691-b2c91000-2b88-11eb-81e0-13abda1e7a1e.PNG)

### Views Dashboard:

The views dashboard is a room overview, each page represnets a room/area with all the devices expanded out.

 - If the room as more than 1 light a master control is added at the top which controls the light group
 - All individual lights are given a card with brightness control, a custom Hue Bulb SVG is used here.
 - Any additional devices/sensors/temperature cards are added here for more information on the room.
 - Any scenes are added below the cards for quick toggling.
 - A back button returns you to the main overview page.

![Views-Lounge](https://user-images.githubusercontent.com/25502878/81858934-6e671280-955c-11ea-8dda-87a23f746384.png)

![Views-Office](https://user-images.githubusercontent.com/25502878/81858939-6f983f80-955c-11ea-84d7-e0aef923c0a5.png)

### Tablet Dashboard:

An Amazon Fire 7 (2017) tablet is wall mounted to function as an alarm panel when the alarm is armed, this is mainly for guests however when the alarm is disarmed the same homekit style buttons are shown on the tablet.  Due to the screen size only the nessessary buttons and information are shown on this dashboard to avoid having to scroll to much.

![Tablet-Dashboard](https://user-images.githubusercontent.com/25502878/81858943-70c96c80-955c-11ea-8181-194ddb5d46c9.png)
