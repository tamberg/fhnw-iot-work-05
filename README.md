# IoT Engineering
## Hands-on of lesson 5
For slides and example code, see [lesson 5](../../../fhnw-iot/blob/master/05/README.md)

> *Note: Do not work on this repository right away.*<br/>
> *[Check existing forks to find the specific repository for your class.](../../network/members)*

### a) HRM BLE peripheral, 10'
* Build and run the [nRF52840_HrmBlePeripheral](https://github.com/tamberg/fhnw-iot/blob/master/05/Arduino/nRF52840_HrmBlePeripheral/nRF52840_HrmBlePeripheral.ino) example.
* Use the .ino link on the page to get the example code.
* Explore the HRM example using a smartphone app.<br/>(Try [nRF Connect for Android](https://play.google.com/store/apps/details?id=no.nordicsemi.android.mcp) or [iOS](https://apps.apple.com/us/app/nrf-connect/id1054362403).)
* Try to enable notifications to get value updates.

### b) UART BLE peripheral, 10'
* Build and run the [nRF52840_UartBlePeripheral](https://github.com/tamberg/fhnw-iot/blob/master/05/Arduino/nRF52840_UartBlePeripheral/nRF52840_UartBlePeripheral.ino) example.
* Send data to the device using the [nRF Connect app](https://www.nordicsemi.com/Software-and-Tools/Development-Tools/nRF-Connect-for-mobile).
* Done? Compare the above to Adafruit's [bleuart.ino](https://github.com/adafruit/Adafruit_nRF52_Arduino/blob/master/libraries/Bluefruit52Lib/examples/Peripheral/bleuart/bleuart.ino).

### c) UART BLE central, 10'
* Build and run the [nRF52840_UartBleCentral](https://github.com/tamberg/fhnw-iot/blob/master/05/Arduino/nRF52840_UartBleCentral/nRF52840_UartBleCentral.ino) example.
* Send data to a nRF52840 UART peripheral device.
* Make sure every sent byte arrives at the other side.

### d) Beacons, 10'
* Build and run the [nRF52840_BeaconBleObservable](https://github.com/tamberg/fhnw-iot/blob/master/05/Arduino/nRF52840_BeaconBleObservable/nRF52840_BeaconBleObservable.ino) example.
* Test the beacon with a dedicated [iOS](https://itunes.apple.com/app/nrf-beacons/id879614768?mt=8)/[Android](https://play.google.com/store/apps/details?id=no.nordicsemi.android.nrfbeacon) app.
* Which information is transferred by a beacon?

### e) Scanner BLE central, 10'
* Build and run the [nRF52840_ScannerBleCentral](https://github.com/tamberg/fhnw-iot/blob/master/05/Arduino/nRF52840_ScannerBleCentral/nRF52840_ScannerBleCentral.ino) example.
* Add a checkReportForUuid() for the Battery Service.
* Can you spot the UUID in the advertising data?
