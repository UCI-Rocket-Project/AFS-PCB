# UCIRP Avionics Test Payload (ATP)
The board includes: 
- [Adafruit BMP388](https://www.amazon.com/Adafruit-BMP388-Precision-Barometric-Altimeter/dp/B07JXYK9ZB) Barometric and Pressure Sensor
- [Hitlego MPU-6050](https://www.amazon.com/HiLetgo-MPU-6050-Accelerometer-Gyroscope-Converter/dp/B01DK83ZYQ/ref=pd_ybh_a_1?_encoding=UTF8&refRID=VTDTAEY02AXR1SPZ293G&th=1) Accelerometer and Gyroscope
- [Adafruit Ultimate GPS](https://www.adafruit.com/product/746#description)
- [Xbee-PRO XSC S3B](https://www.mouser.com/ProductDetail/Gravitech/XBee-USB?qs=Vxac6xGyzPnMlpwH9hhfHQ%3D%3D) 

Communication Protocols Used:
| Component  | Communication Protocol |
| ------------- | ------------- |
| BMP388  | I2C  |
| MPU-6050  | I2C  |
| GPS  | UART  |
| XBEE  | UART  |

## Used Packages
* Teensy 4.1 [symbol](https://github.com/XenGi/teensy_library) and [footprint](https://github.com/XenGi/teensy.pretty). Related files and license is located under `/teensylib`.
