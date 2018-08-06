Autonomous Green House System.

Implementation is done using Arduino, Raspberry Pi, Zigbee, Android App and Amazon Web Services to get the data visualization. 

Raspberry Pi serves as the base station to update the info to the cloud. 
The data collected will render the owner to set the thresholds for watering and Sunlight. 
Sensors used are LDR, Temperature and Humidity, pH, Soil Moisture. 

1) Each plant has a sensor node to get the information about the conditions it's living in. 
2) This information, using Zigbee protocol, is transferred to the base station, which acts as a coordinator. 
3) The base station decides on the control of water and sunlight to that respective plant. 
4) If the plant is in need, the base station transfers a packet to irrigation system or lighting system to turn on. The duration of the system till it stays on can be controlled either by the App.
5) Each time the data and status of the system is stored in the local database of base station and populates into AWS.
6) Visualization tools help to get the insights of that particular plant to calculate the best conditions for its sustainable and healthy growth.
7) The data from AWS is fetched by the Android Application to display the status. User can control the threshold of Soil moisture and Light to trigger the system via the App itself. 
8) User has the option of controlling the system either in an autonomous or manual state. 