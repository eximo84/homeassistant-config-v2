# Custom Button Cards

Here is a collection of custom cards used within my LoveLace setup.  I have split each card out with the associated templates to help understand what is needed for each button type.

For further reference see the Custom Button Card Repo: https://github.com/custom-cards/button-card

Some of these are still WIP and can be improved.

## Badge Buttons 

These mimic the default Home Assistant badges or HomeKit badges.  Providing subtle information with a tap action to other views or popup cards.  Badge Button is a 5 column grid

![Badge](https://user-images.githubusercontent.com/25502878/113141009-104d2780-9221-11eb-9379-8573967100f0.PNG)

* Used with any entity
* Background illuminates if the entity is on or provides a transparent background with a border when off
* Name/Status/Label can be used to provide more information - here im using a template sensor to count lights on from a specific group then providing that to the button.
* I use a heavily modified custom badge to display music information

Standard button cards are setup in a 3 column grid. View button card is a 2 column grid.

## Light Button

![Light](https://user-images.githubusercontent.com/25502878/101266388-4df3e500-3746-11eb-8c1a-a94d53d3c118.PNG)

* Used with any light entity
* Background illuminates if the light entity state is on
* Light entity status is shown including brightness of light
* Supports secondary information e.g. Window / Door Entity status
* Supports temperature information

## Switch Button

![Switch](https://user-images.githubusercontent.com/25502878/101266390-4e8c7b80-3746-11eb-82a8-e21d7452072c.PNG)

* Used with any switch or input boolean entity
* Background illuminates if the switch is on
* Switch entity status is shown
* Supports secondary information

## Climate Button

![Climate](https://user-images.githubusercontent.com/25502878/101266386-4d5b4e80-3746-11eb-866c-8f8d77d835c5.PNG)

* Used to display climate information for Tado system
* Background changes depending on target temp - same as Tado iOS App
* Climate status is shown
* Climate current temperature is shown
* Climate heating power % is shown
* Icon "should" change depending on heating mode - not working at the moment
* Custom Icons for Tado System

## Dual Button

![Dual Button](https://user-images.githubusercontent.com/25502878/113473576-38779900-9462-11eb-9114-64efcc8e4f9f.PNG)

* Used to display related information from two entities e.g. Person Tracking or Energy Tracking
* Background changes depending on state
* Button shows more-info for entity by default but can easily be adapted to peform different actions
* Adjust width of the grid columns to allow longer names/states

## Garbage Button

![Garbage](https://user-images.githubusercontent.com/25502878/101266387-4df3e500-3746-11eb-8550-8a70817d4e6b.PNG)

Requires custom component Garbage Collection: https://github.com/bruxy70/Garbage-Collection

* Shows upcoming garbage collection type based on calendar
* Supports 2 types of garbage collection e.g. Black Bin and Recylcing
* Background switches between Black and Green depending on upcoming collection type
* Secondary information displays collection due days of both types
* Very custom code (lots of IF statements)

## Animated Button

![Animated](https://user-images.githubusercontent.com/25502878/101266385-4d5b4e80-3746-11eb-8830-53d01766927c.PNG)

* Used with any switch or input boolean entity
* Background illuminates if the switch is on
* Switch entity status is shown
* Supports secondary information
* Icon is animated - example used is a Fan

## Weather Button

![Weather](https://user-images.githubusercontent.com/25502878/101266546-847e2f80-3747-11eb-8755-39dc5d2528c0.PNG)

* Used with DarkSky but any weather should work
* Background changes colour based on day/night
* Icons change based on weather - mostly hard coded based on entity state
* Supports secondary information such as Preciptation

## Music Playback

![Music](https://user-images.githubusercontent.com/25502878/101266389-4df3e500-3746-11eb-805c-87c8727a3956.PNG)

My setup uses Chromecasts for multi room audio with playback from YouTube Music.  Other apps and speakers might also work.

See main LoveLace Overview and look at the Music Tab for full setup - https://github.com/eximo84/homeassistant-config-v2/blob/master/lovelace-dashboards/overview.yaml

* Automation used to determine active speaker - note this can maybe be done within the card variable but not sure.  Automation can be hit and miss....
* Cover art is displayed from current active speaker
* Tap action will toggle play/pause
* Play/Pause icon overlayed cover art
* Used in conjunction with Mini-Media Player allows for a dynamic playback interface

## View Light Button

![View Light Button](https://user-images.githubusercontent.com/25502878/101266384-4cc2b800-3746-11eb-9d7f-cadb77f1ed93.PNG)

Requires lovelace card Slider Entity Row - https://github.com/thomasloven/lovelace-slider-entity-row

* Hue SVG icon support for Colour/White Ambience, White, GU10, LED Light Strips.
* Bulbs icons illuminate correctly when on
* Used to display status of individual light entity
* Used within the Views Dashboard for individual rooms
* Slider for brightness control
* Light status information
* Seperate power toggle button
* Tap of button brings up More-Info dialog

