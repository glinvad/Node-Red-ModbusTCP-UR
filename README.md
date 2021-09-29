# Node-Red-ModbusTCP-UR
 Node-Red Dashboard to send and recived data via Modbus TCP. Data provicede here is a Universal robot.


**Tested Node-red Version**
- 2.0.6

**Requied Node-red nodes:**
- node-red-contrib-bitunloader
- node-red-dashboard
- node-red-contrib-modbus
- node-red-contrib-ui-artless-gauge

**A overview of the Node-red Dashboard**
![Dashboard overview](https://github.com/glinvad/Node-Red-ModbusTCP-UR/blob/main/Pictures/OverviewDashboard.gif)

**A overview of the Node-red flow**
![Flow overview](https://github.com/glinvad/Node-Red-ModbusTCP-UR/blob/main/Pictures/OverviewFlow.jpg)

**How to setup**

Modbus can be used for a wide variety of equitment.

For simpel testing, I used URSim, an virtual mashine with the UR Polyscope software build in (It can be downloaded from Universal robots homepage) that runs a Modbus TCP Server.

REMEMBER TO CHANGE THE IP TO A MODBUS SERVER THAT HAVE RELEVANT DATA AVALIABLE

![Modbus server](https://github.com/glinvad/Node-Red-ModbusTCP-UR/blob/main/Pictures/ModbusTCPserver.jpg)

**How to import the code**
- Install Node-Red on your platform
- Install the Nodes
- Go to Import in the top corner 
![Import Node-red](https://github.com/glinvad/Node-Red-ModbusTCP-UR/blob/main/Pictures/NodeRedImport.jpg)
- Inset the code from the **Node-Red Code**
- Setup the Modbus server, this setup is made for the adresses of the FC3: Holding register that fits a Universal Robot.
- Have some fun with the data :)

**Change the pull from holding register**
![FC3 holding register](https://github.com/glinvad/Node-Red-ModbusTCP-UR/blob/main/Pictures/SettingUpGetHOLDING.jpg)

**Sending the data to OPC UA Server**

In this flow, the data is comming from the Universal robot via Modbus TCP and are displayed on the Dashboard. But the data is also sent to another flow and are stored on a OPC UA server via Node-red. You can finde more on this on an upcomming github.
![Sending data to another flow](https://github.com/glinvad/Node-Red-ModbusTCP-UR/blob/main/Pictures/SendingDataToOPCUAflow.jpg)
![Sending data to another flow](https://github.com/glinvad/Node-Red-ModbusTCP-UR/blob/main/Pictures/SendingDataToOPCUAflow2.jpg)


