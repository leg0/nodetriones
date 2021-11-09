
For the BLE adapter to work properly, you need to make sure that the adapter is one
of the following:

| Name | USB VID | USB PID |
|:---- | :------ | :-------|
| BCM920702 Bluetooth 4.0 | 0x0a5c | 0x21e8 |
| BCM20702A0 Bluetooth 4.0 | 0x19ff | 0x0239 |
| CSR8510 A10 | 0x0a12 | 0x0001 |
| Asus BT-400 | 0x0b05 | 0x17cb |
| Intel Wireless Bluetooth | 0x8087 | 0x07dc |

Then use [Zadig tool](http://zadig.akeo.ie) to replace the driver for your adapter with WinUSB driver.

This project uses noble for connecting to a bluetooth RGB LED controller.
Change the ID of your Bluetooth device in index.js - mine is 10324c7682484bc7acbd4d87a40f5950.

This project is based on this amazing work:
https://github.com/madhead/saberlight/blob/master/protocols/Triones/protocol.md
