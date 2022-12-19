# UCIRP Avionics Flight Sensor (AFS)
v1.0 "Rigel" (a star in Orion's constellation)

The board includes: 
- [Adafruit BMP388](https://www.amazon.com/Adafruit-BMP388-Precision-Barometric-Altimeter/dp/B07JXYK9ZB) Barometric and Pressure Sensor
- [Hitlego MPU-6050](https://www.amazon.com/HiLetgo-MPU-6050-Accelerometer-Gyroscope-Converter/dp/B01DK83ZYQ/ref=pd_ybh_a_1?_encoding=UTF8&refRID=VTDTAEY02AXR1SPZ293G&th=1) Accelerometer and Gyroscope
- [Adafruit Ultimate GPS](https://www.adafruit.com/product/746#description)
- [Digi XBee-PRO XSC S3B](https://www.mouser.com/ProductDetail/Gravitech/XBee-USB?qs=Vxac6xGyzPnMlpwH9hhfHQ%3D%3D) 
- [Adafruit XBee USB Adapter](https://www.adafruit.com/product/247?gclid=Cj0KCQiA1sucBhDgARIsAFoytUtwdYkYjMLGpFy2WvyzD8O8x4Ewsu3eSLwTMnisukgy84cH7zYznMQaAjZiEALw_wcB)
- Teensy 4.1
- [Linear Regulator (9V -> 5V)](https://www.digikey.com/en/products/detail/stmicroelectronics/L7805CV/585964)

Communication Protocols Used:
| Component  | Communication Protocol |
| ------------- | ------------- |
| BMP388  | SPI  |
| MPU-6050  | I2C  |
| GPS  | UART  |
| XBEE  | UART  |



## Used Packages
- Teensy 4.1 [symbol](https://github.com/XenGi/teensy_library) and [footprint](https://github.com/XenGi/teensy.pretty). Related files and license is located under `/teensylib`.


## Notes
- The board requires an external 9V battery to power sensors and the Teensy
- The GPS uses an optional "CR1220 coin cell to keep the RTC running and allow warm starts"
- The XBee module (not on AFS PCB) mounts on top of the XBee USB adapter. The USB adapter board has power and serial pass-through to the XBee module
- The board was renamed from "Avionics Test Payload (ATP)" to "Avionics Flight Sensor (AFS)"
