
Course : DEV302x: Microsoft Professional Capstone: Internet of Things

I've submitted the project challenging activites as described in the course. In this regard, I would like to mention the following points to clarify some of the issues  found and approach followed in resolving them.

 
Challenge #1 : Weather Station Pov

1. I've added Azure  function "iot-func2-4C2C5A3B" to  store  telemetry data to the  cosmos db in warm path route.  This function receives IOT Hub message as Input and outputs the same to the Cosmos DB.
This is  just to demonstrate the data transofrmation approach to send iot data to cosmos DB as given in the reference architecture. Also, please note  the function "iot-func2-4C2C5A3B" is saved to the Lab2 azure resources template (WeatherStationThreatModel-4C2C5A3B) and not in  Lab1. I've added this later in the process and hope this is not an issue.

Challenge #2: Wind Farm Pov:

2.  I was not able to generate a Date heirarchy in Power BI Desktop graph  "PowerBIDashboard-4C2C5A3B.png" saved in  Lab2 folder. I am  not sure but it appears to be a power BI desktop issue. I've reported this to the Microsoft MPP academy support and edx user group and I am waiting for their reply.

3. I was not able to provision the devices  using Device proivsioning service (Enrollement Group with x.509 attestation.) The device connection  string requried to configure the Wind farm POV was disabled in the portal, so I created the devices directly in the azure iot hub.

4. Windfarm POV SImulator generated data with "lowSpeedShaftRpm" as "zero" and  thus resulting in power ratio as infinity. I've filtered the data to exclude records where "lowspeedshaftRPM" is zero in the query to generate a graph.


Threat Model tool:

5.  The stencil elements " MQTT data link" and  "Azure Time Series service" were not available in the template used for Threat Modelling tool. I've used the Generic elements in place of those.



