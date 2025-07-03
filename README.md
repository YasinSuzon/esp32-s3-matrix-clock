ESP32-S3 LED Matrix Codes
A customizable matrix clock powered by the ESP32-S3 Matrix 8x8 RGB-LED-WiFi-Bluetooth board. This ESPHome-based project scrolls the current time, custom messages, sensor data across a vibrant LED grid, integrated with Home Assistant. Minimal hardware, maximum pixel flair.

Features
- Displays current time using Home Assistant integration
- Scrolls text like "HELLO THERE" in pixel font
- Showing current weather from Home Assistant sensors
- Showing a door status from HA sensors with text 'Door is Open'
- Uses ESPHome with addressable light platform
- Color effects using FastLED (rainbow, twinkle, scan, etc.)
- OTA updates and Wi-Fi signal monitoring
- Future potential: add gesture/motion interaction with QMI8658C

Hardware
- Board: ESP32-S3 Matrix 8x8 RGB-LED-WiFi Bluetooth (QMI8658C sensor)
- LED: 8x8 RGB matrix (WS2812-compatible)
- Power: USB-C or 5V input

Setup
- Place .yaml and font files into your ESPHome folder
- Add your credentials to secrets.yaml (never commit this file):

wifi_ssid: "YOUR_WIFI_SSID"
wifi_password: "YOUR_WIFI_PASSWORD"
api_key: "YOUR_API_KEY"
ota_password: "YOUR_OTA_PASSWORD"

- Flash using ESPHome or dashboard
- Add to Home Assistant
- Watch the magic scroll!

File Structure
- esp32-s3-matrix-clock.yaml
- fonts/pixelmix.ttf
- secrets.example.yaml

License
MIT – Free to use, remix, and share.
