# ESP32-CAM-ESP-IDF-Live-Streaming-Web-Server

For details visit this link:
https://esp32tutorials.com/esp32-cam-esp-idf-live-streaming-web-server/

# Configuration

Open a [PlatformIO Core CLI](https://docs.platformio.org/en/latest/integration/ide/vscode.html#platformio-core-cli) and execute
```
pio run -t menuconfig
```

to enter the menuconfig. Select your target WiFi and camera board type in the "Application settings".

(move around with J/K keys if needed.)

![config](config.png)

The default ist `CONFIG_BOARD_ESP32CAM_AITHINKER` (esp32cam). Double check the pins in `camera_pins.h` if needed.

After the example is uploaded, it should connect to the configured WiFi and open a HTTP server at `http://<ip of your esp32>/`.