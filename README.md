# azure-iot-raspi
Starter app to connect a Raspberry Pi to Azure IoT Hub.

## Setup

1. follow instructions in https://github.com/Azure-Samples/azure-iot-samples-node/tree/master/iot-hub/Samples/device to setup Azure IoT Hub instance
2. create device in Azure IoT Hub:
   - Click on IoT Devices in the Azure IoT Hub and select New to create a new device
   - Enter a device ID and select Save
   - Click on the device and copy the Primary Connection String
3. Deploy app to Raspberry Pi. Login to the Raspberry Pi and :
```
cd /usr/local
git clone https://github.com/jimareed/azure-iot-raspi
cd azure-iot-raspi
node install
export DEVICE_CONNECTION_STRING="<connection_string>"
node index.js
```
## Sources
- https://github.com/Azure-Samples/azure-iot-samples-node
