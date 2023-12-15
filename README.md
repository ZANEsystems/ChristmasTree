# ChristmasTree :tw-1f332:

 ESP32 Based WS2812 RGB LED Christmas Tree
 

# Features

- WS2812 RGB LEDs
- ESP32-S2-MINI-1
- User programmable button
- USB Type-C for power and programming
- FTDI connector pins

# Stock Firmware

We ship the ChristmasTree with WLED firmware.
WLED is an open source webserver running on ESP devices made to control NeoPixel LEDs.
You can read more about WLED here:
https://github.com/Aircoookie/WLED

# Building your own firmware

We recommend using PlatformIO:
https://platformio.org/platformio-ide

1. Create a new project in PlatformIO, select board: "esp32-s2-saola-1", framework: Arduino
2. Add NeoPixel library dependency to your platformio.ini file:
    lib_deps =
    https://github.com/adafruit/Adafruit_NeoPixel.git
3. Copy the file main.cpp to your project. (This is our version of NeoPixel example "buttoncycler")
4. Put the board into bootloader mode: Press and hold the button while inserting the USB connector.
5. Build and upload the PIO project.
6. Reset the board by unplugging and plugging the connector in.
7. Press the button to cycle through presets.