# MLX90640-Thermocam

We built a simple Thermal camera using the MLX90640 Sensor, an ESP32, a ILI9341 TFT, a 18650 battery in a 3D printed case. 
It was featured in Netzbasteln #111: http://www.netzbasteln.de/#111 and still lacks interpolation.

Code Based on:
- Thermal Camera with image saving capability https://github.com/wilhelmzeuschner/arduino_thermal_camera_with_sd_and_img_processing
- SparkFun MLX90640 Examples https://github.com/sparkfun/SparkFun_MLX90640_Arduino_Example
- TFT_eSPI Library: https://github.com/Bodmer/ (use settings from Setup_User.h)

Needs an ESP32 core fork:
- https://github.com/sparkfun/SparkFun_MLX90640_Arduino_Example/issues/2
- https://github.com/stickbreaker/arduino-esp32

Hardware:
- ESP32 Devkit 4 (or any other ESP32): https://www.espressif.com/en/products/hardware/esp32-devkitc/overview
- MLX90640 Sensor Breakout Board: https://shop.pimoroni.com/products/mlx90640-thermal-camera-breakout (or the Sparkfun one)
- Display ILI9341 2.8": https://www.amazon.de/gp/product/B07DPMV34R/, https://www.pjrc.com/store/display_ili9341.html 
- Charger TP4056: https://www.watterott.com/de/TP4056-Micro-USB-5V-1A-Lithium-Battery-Charger-with-Protection
- Battery 18650 
- 3D Printed case: 

ESP32 Pins (GND/VCC is obvious ;)
```
SENSOR_SDA 21
SENSOR_SCL 22 
TFT_MISO 19
TFT_MOSI 23
TFT_SCLK 18
TFT_CS   15
TFT_DC    2
TFT_RST   4 
```
