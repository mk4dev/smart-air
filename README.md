# smart-air 
A simple school IOT project in health domain The project is a simulation in **Proteus** of system of monitoring and maintaining air quality in hospitals. It contains a raspberry pi, poluttig gas sensors, dispaly, inetnet connection, and it's conncted to air puriffier system to command it.
The sensors are not availabe in Proteus, so a real dataset is feed to the reaspberry oi using seril pins to plau the role or sensors. The data is the concentration if the gases in a period of time to make the simulation stable. the data is sent sent using a pythin script, after concatenating all the dataset in one stream, and sending in fix period.

The monitoring part is also done by sending the data to Azure IOT hub using MQTT lite protocole, then the data is passed to Stream Analytics to do real time processing or, in our case, we just pass it to Power BI, to do simple visualisation.

We used **com0com** to create virualtion link between the serial port of parsspbery pi in Proteus and the port used in the python script. And we added **Paho**  to the debug code in Proteus to allow the simulation of rasspberry pi to send MQTT data to Azure IOT hub.

This is a group school project. When I'll have time I'll add more details how it works.
