# ESP8266 Cryptocurrency Price Display Using CoinGecko API and OLED (I2C)
  This project displays real-time prices of multiple cryptocurrencies on a 0.96" OLED screen using an ESP8266 microcontroller.
  The data is fetched from the CoinGecko API, and the display is connected over I2C, providing a compact, low-power solution for tracking crypto prices.

## Features
+  Displays prices for multiple cryptocurrencies (e.g., Bitcoin, Ethereum, etc.).
+  Uses the CoinGecko API to fetch live price updates.
+  OLED display (0.96") connected via I2C for clear, real-time data presentation.
+  Built using an ESP8266 microcontroller for WiFi connectivity and easy web-based API integration.
+  Manage WiFi credentials and Fingerprint settings through a web interface.


## Requirements
1. ESP8266 (NodeMCU or similar).
2. 0.96" OLED display (I2C interface).
3. [CoinGecko Fingerprint](https://fingerprint.com/).

## Setup Instructions
**OLED Display SSD1306 Pin Wiring.**
+  Pin -->	ESP8266
+  Vin -->	3.3V
+  GND	--> GND
+  SCL	--> GPIO 5 (D1)
+  SDA	--> GPIO 4 (D2)

## Configure Credentials:
   Use the web interface to add or remove WiFi credentials and CoinGecko Fingerprint.


## Usage:
   ```bash
   git clone https://github.com/towsif-aktar/Cryptocurrency-Price-Display.git
```

+  Flash the ESP8266 with the provided [Flash Tool](https://www.espressif.com/en/support/download/other-tools).
+  After the ESP8266 connects to your WiFi.
+  You can access the management interface by entering this IP address in a web browser.
+  IP Address: `http://192.168.1.1`


## How It Works
1. The ESP8266 connects to WiFi and fetches cryptocurrency data from the CoinGecko API.
2. Prices are parsed and displayed on the OLED using the I2C protocol.
3. The screen refreshes at regular intervals to update the prices.
4. You can manage the credentials and Fingerprint via the web interface using the device's IP address.
