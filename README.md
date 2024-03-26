# MQTT-publisher-implementation-in-Python
This code is a Python script that connects to an MQTT broker (broker.mqttdashboard.com), publishes messages to a specific topic (Building/Temperature).

Here's a breakdown of what each part of the code does:

Importing Libraries: The script imports necessary libraries, including random, time, and paho.mqtt.client.

Setting MQTT Parameters: The script defines the MQTT broker's address (broker.mqttdashboard.com), port (1883), topic (Building/Temperature), client ID (generated randomly using random.randint(0, 1000)), username (websocket), and password (public1).

Function connect_mqtt(): This function sets up the MQTT client, configures authentication with username and password, and connects to the MQTT broker. It also defines a callback function on_connect() to handle the connection status.

Function publish(client, num_messages): This function publishes a specified number of messages (num_messages) to the MQTT topic. It uses a loop to send messages every second. The message content is formatted as messages: {msg_count}, where msg_count is the message count.

Function run(): This function sets the number of messages to be published (num_messages), connects to the MQTT broker using connect_mqtt(), starts the MQTT client loop, and publishes messages using publish(client, num_messages).

Main Block: The script checks if it's being run directly (__name__ == '__main__') and calls the run() function to execute the MQTT publishing process.

Overall, this script demonstrates a basic MQTT publisher implementation in Python using the paho.mqtt.client library. It's a simple example and can be extended or modified as needed for specific MQTT publishing requirements.

![MQTT](https://github.com/IndikaAnuradha/MQTT-publisher-implementation-in-Python/assets/122884553/8bed5399-9fb2-4934-9800-457e7eabae21)

To learn more about the topic refer below links....

https://public.dhe.ibm.com/software/dw/webservices/ws-mqtt/MQTT_V3.1_Protocol_Specific.pdf

https://www.alvasys.ch/files/v220128200104/shop/MQTT-BROKER100_Basic_von_HiveMQ.pdf
