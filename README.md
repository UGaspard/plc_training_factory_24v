> If you have any questions, please contact fischertechnik-technik@fischer.de

# fischertechnik Training Factory Industry 4.0 24V (en)
This project contains the PLC programs, the IOT gateway SD card image with Node-RED flows and the TXT gateway C program for the fischertechnik [**Training Factory Industry 4.0 24V**](https://www.fischertechnik.de/en/products/simulating/training-models/554868-sim-training-factory-industry-4-0-24v-simulation).

## Controllers
The standard demo scenario is implemented with the [www.fischertechnik-cloud.com](https://www.fischertechnik-cloud.com). It is also possible to use the PLC program without the fischertechnik cloud. In this case the local Node-RED dashboard can be used.

The following diagram shows the communication between the 3 controllers PLC, TXT controller and IOT gateway (Raspberry Pi 4):
![overview_communication_en](doc/overview_communication_en.png "overview communication")

The following folder structure exist:
* **PLC_S7_1500** (PLC S7 1500 project, TIA Portal v16)
* **PLC_S7_1500_sources** (PLC sources as SCL Structured Control Language)
* **PLC_S7_1500_exercises** (PLC S7 1500 exercises, TIA Portal v16)
* **Node-RED** (SD card image, Node-RED flows)
* **TxtGatewayPLC.cloud** (C program for TXT controller, [TxtGatewayPLC](https://github.com/fischertechnik/plc_training_factory_24v/tree/master/TxtGatewayPLC))

## Network
The next picture shows the network overview with the controllers.
![factory_overview_en](doc/factory_overview_en.png "factory overview")

The factory consists of the following stations:
* **SSC**: Sensor Station with Camera
* **HBW**: High-Bay Warehouse
* **VGR**: Vacuum Gripper Robot
* **DPS**: Delivery and Pickup Station
* **MPO**: Multi-Processing Station with Oven
* **SLD**: Sorting Line with Color Detection

## Node-RED
The [Node-RED](https://nodered.org/) flows for the Training Factory Industry 4.0 24V you can find in [Node-RED](Node-RED/README.md) folder. 

