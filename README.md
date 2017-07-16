# homebridge-dyson-link

## Introduction
This is just a hobby project as I just bought my Dyson Link device and would like to use Siri and Home App to control that. I decided to share here just in case if this can be somewhat useful to others, that will be great. :)

## Installation

Assuming you have homebridge installed and set up, you can run below command to install this plugin

`npm install -g homebridge-dyson-link`

Then, you can add the platform configuration to your config.json

## Configuration

See config-sample.json for example

We will need to input the IP, display name, serial number and password to the config

The serial number(DYSON-XXX-XX-XXXXXXXX-XXX) and password(normally 8 characters) of your device can be found on the device and the manual.

```
"platforms": [
      // This is the config    
    {
      "platform": "DysonPlatform",
      "name": "DysonPlatform",
      "accessories": [
        {
          "ip": "ip of your device",
          "displayName": "Name to be shown on Home App",
          "serialNumber": "DYSON-XXX-XX-XXXXXXXX-XXX",
          "password": "password of your device"
        }
      ]
    }
  ],
```
