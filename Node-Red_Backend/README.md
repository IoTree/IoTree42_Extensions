## Advanced Node Red extension
### Installation
Import the flow into your Node-Red running in the backend of your server.
Define credancilas in the configuration node of MQTT.
Define credacials in the function nodes that connect to the DB.
And, if used, define the api token in the weather api function node.

### Features
This is an extended backend for IoTree42 and can be used instead of the python scipts mqttoinfluxdb6.x.py.
It has advanced MQTT message processing for example:
- Limiting certain messages from certain users.
- Connection to openweathermap.org to allow users to retrieve weather data.
- Logging of gateway connection and number of messages per gateway.
	-> Allows admin to debug high traffic load by finding the gateway and user to it.
- Better ping response: sending back the current time of the server.
	-> this can be used to calculate round trip time/delay.

### NOTE:
Pay attention to the protection of Node-red problerly!!!

 