# Custom Button Cards

Here is a collection of custom cards used within my LoveLace setup.  I have split each card out with the associated templates to help understand what is needed for each button type.

For further reference see the Custom Button Card Repo: https://github.com/custom-cards/button-card

Some of these are still WIP and can be improved.

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

