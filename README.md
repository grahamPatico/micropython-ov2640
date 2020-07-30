
# MicroPython class for OV2640 Camera, specifically Pycom

Using this class you can:


## Usage - Hardware Setup

This particular camera has both an i2c and spi interface for setup and
getting data on/off the camera.  A good way to wire up the camera to
the ESP8266 and ESP32 is as follows (note Vcc and GND pins are not included here):

 Camera Pin | ESP8266 Pin  | ESP32 Pin | Pycom Pin
| --------- | ------------ |-----------|-----------
| CS        | GPIO2        |GPIO15     |Pin 'P9'  |
| MOSI      | GPIO13       |GPIO13     |Pin 'P11' |
| MISO      | GPIO12       |GPIO12     |Pin 'P14' |
| SCK       | GPIO14       |GPIO14     |Pin 'P10' |
| SDA       | GPIO4        |GPIO21     |Pin 'P21' |
| SCL       | GPIO5        |GPIO22     |Pin 'P22' |

## Usage - Software

First upload the module 'ov2640.py' into the root filesystem on the
ESP8266 or ESP32 board you are using.  The [ampy](https://github.com/adafruit/ampy)
tool from Adafruit is a useful tool for doing that.  Together with
[esptool](https://github.com/espressif/esptool), you can re-flash your
board and load the code here in one shot with these commands.

First download the latest MicroPython [image from here](http://micropython.org/download#esp8266).

## Credits

The original driver source from Arducam was instrumental in the creation of this pure
MicroPython version.

The overall project was inspired by
[esparducam](https://johan.kanflo.com/building-the-esparducam/), but
getting this to work doesn't require any SMD soldering. :)


