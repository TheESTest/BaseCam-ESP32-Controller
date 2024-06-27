# BaseCam-ESP32-Controller
This project uses the BaseCam Serial API with an ESP32-S3 dev board to read and send signals from an ESP32 to a BaseCam SimpleBGC 32-bit Extended Long controller.
There are two cases:
1. Case #1 - using 1 x ESP32-S3 dev board directly reading from 3 x single-axis joystick modules, and connected directly to the BaseCam controller. Run the PlatformIO code on the ESP32.
2. Case #2 - using 1 x ESP32-S3 dev board to read from 3 x single-axis joystick modules, and sending those readings over BLE to a secondary ESP32-S3 board, which receives the signals and relays them to the BaseCam controller. For this case, run the Arduino code (.ino) on the joystick-connected ESP32, and run the PlatformIO project on the ESP32 connected to the BaseCam controller.

Feel free to check out my blog post about this project to see more details and a demonstration of the code in action.
