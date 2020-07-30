
# MicroPython class for OV2640 Camera, specifically Pycom

## Usage - Hardware Setup

(Vcc and GND pins are not included here):
I2C and SPI pins

 Camera Pin | ESP8266 Pin  | ESP32 Pin | Pycom Pin
| --------- | ------------ |-----------|-----------
| CS        | GPIO2        |GPIO15     |Pin 'P9'  |
| MOSI      | GPIO13       |GPIO13     |Pin 'P11' |
| MISO      | GPIO12       |GPIO12     |Pin 'P14' |
| SCK       | GPIO14       |GPIO14     |Pin 'P10' |
| SDA       | GPIO4        |GPIO21     |Pin 'P21' |
| SCL       | GPIO5        |GPIO22     |Pin 'P22' |

![](images/camera.jpg)
## Credits

The original driver source from Arducam was instrumental in the creation of this pure
MicroPython version.

The overall project was inspired by
[esparducam](https://johan.kanflo.com/building-the-esparducam/), but
getting this to work doesn't require any SMD soldering. :)


