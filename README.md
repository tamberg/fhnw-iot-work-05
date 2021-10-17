# IoT Engineering
## Hands-on of lesson 5
For slides and example code, see [lesson 5](../../../fhnw-iot/blob/master/05/README.md)

> *Note: Do not work on this repository right away.*<br/>
> *[Check existing forks to find the specific repository for your class.](../../network/members)*

### a) HRM BLE peripheral, 10'
* Build and run the [nRF52840_HrmBlePeripheral](https://github.com/tamberg/fhnw-iot/blob/master/05/Arduino/nRF52840_HrmBlePeripheral/nRF52840_HrmBlePeripheral.ino) example.
* Explore the HRM example using a smartphone app,<br/>e.g. [nRF Connect for Android](https://play.google.com/store/apps/details?id=no.nordicsemi.android.mcp) or [iOS](https://apps.apple.com/us/app/nrf-connect/id1054362403).
* Try to enable notifications to get value updates.

### b) UART BLE peripheral, 10'
* Build and run the [nRF52840_UartBlePeripheral](https://github.com/tamberg/fhnw-iot/blob/master/05/Arduino/nRF52840_UartBlePeripheral/nRF52840_UartBlePeripheral.ino) example.
* Write bytes to RX with a generic BLE explorer app.
* Check the serial monitor to see the received bytes.
* Why do some bytes not show up?

### c) UART BLE central, 10'
* Build and run the [nRF52840_UartBleCentral](https://github.com/tamberg/fhnw-iot/blob/master/05/Arduino/nRF52840_UartBleCentral/nRF52840_UartBleCentral.ino) example.
* Open the Arduino serial monitor to enter a message.
* Use a second nRF52840 as a UART peripheral.

### d) Beacons, 10'
* Build and run the [nRF52840_BeaconBleObservable](https://github.com/tamberg/fhnw-iot/blob/master/05/Arduino/nRF52840_BeaconBleObservable/nRF52840_BeaconBleObservable.ino) example.
* Test the beacon with a dedicated [iOS](https://itunes.apple.com/app/nrf-beacons/id879614768?mt=8)/[Android](https://play.google.com/store/apps/details?id=no.nordicsemi.android.nrfbeacon) app.
* Which information is transferred by a beacon?
* Start a scan in a public place, e.g. Zürich HB.

### e) Scanner BLE central, 10'
* Build and run the [nRF52840_ScannerBleCentral](https://github.com/tamberg/fhnw-iot/blob/master/05/Arduino/nRF52840_ScannerBleCentral/nRF52840_ScannerBleCentral.ino) example.
* Add a _checkReportForUuid()_ for the Battery Service.
* Can you spot the UUID in the advertising data?

### f) Challenge, 1h+
* Design and implement an API for the [DHT11 sensor](https://github.com/tamberg/fhnw-iot/wiki/Grove-Sensors#temperature--humidity-sensor-dht11).
* [Create UUIDs](https://ddg.co/?q=uuid) for your service and its characteristics.
* Allow the central to read temperature and humidity.
* Chose a data format that fits the sensor value range.
* Test your peripheral with a generic BLE explorer.
* Done? Consider adding support for notifications.
