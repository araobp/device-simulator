# Device simulator based on HTML5 and AngularJS

## Prerequisite

- [mosquitto](https://mosquitto.org) is runnig somewhere, for example, on RasPi.
- The mosquitto has been made(compiled) with WebSockets option enabled.
- angular.min.js and browserMqtt.js is accesible from a simulator.

Refer to the following links for mosquitto and browserMqtt.js:
- [obtaining mosquitto with WebSockets enabled](https://xperimentia.com/2015/08/20/installing-mosquitto-mqtt-broker-on-raspberry-pi-with-websockets/)
- [building browserMqtt.js](https://github.com/mqttjs/MQTT.js/)

## Architecture

```
[Script    ]                                         [Device simulator node]  
[AngularJS ]---mqtt/WebSocket---[mosquitto]---mqtt---[mqtt client          ]
[HTML5/CSS3]                                         [Node-RED             ]
```

### Hello World

[sample](./index.html)

### Display

[display](./display.html)

### Image 

[image](./display.html)

### Video 

[video](./video.html)

### Elevator

[elavator](./elevator.html)

## Working with one-liner HTTP server

Assuming that mosquitto is running on RasPi and all the files above are also on RasPi, use one-liner HTTP server to use the simulator on another PC.

Installation
```
$ npm install -g http-server
```

Usage
```
$ http-server
```
