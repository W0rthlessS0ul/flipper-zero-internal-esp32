## ⚡ Installing ESP32 Inside Flipper Zero ⚡
-----
Welcome to the **ESP32 Installation Guide** for Flipper Zero! 🎉  
This repository will demonstrate how to install an ESP32 inside the Flipper Zero.

## 📚 Table of Contents
- [🚀 What Will This Bring Me?](#-what-will-this-bring-me)
- [🛠️ What Types of Boards Would Be Suitable?](#️what-types-of-boards-would-be-suitable)
- [🧑‍🔧 Let's Get Started with Soldering!](#-lets-get-started-with-soldering)
- [❤️ Thank You for Your Support!](#-thank-you-for-your-support)
- [🌐 Follow Me for Updates](#-follow-me-for-updates)

-----

## 🚀 What Will This Bring Me?
The ESP32 is a module that operates with Wi-Fi and Bluetooth. When connected to the Flipper Zero, it enables various attacks such as deauthentication, handshake capturing, and many other possibilities.

-----

## 🛠️ What Types of Boards Would Be Suitable?
| Board Type          | Compatibility |
|---------------------|---------------|
| esp32-wroom-32      | ✅            |
| esp8266             | ➕➖          |
| esp32-C3 supermini  | ❌           |

*Note: If you're using the ESP8266, you won't be able to access certain features, such as handshake capture.*

-----

## 🧑‍🔧 Let's Get Started with Soldering!
However, please remember that the author bears no responsibility for any potentially damaged boards; you undertake all actions at your own risk!

1. To start, you need to desolder the metal cover from your ESP32 (or ESP8266).  
   ![esp32 metal cover](esp32_cover.png)

2. Now, please open your Flipper Zero and disassemble it down to the main board with the display and buttons. For a detailed example of how to do this, refer to the following video: [video](https://www.youtube.com/watch?v=Jqfxk0_ppBc)

3. Now, arrange the ESP32 and the 5V to 3.3V converter on the motherboard.  
   ![esp32_install](esp32_install)

4. Now, please solder the ESP32 converter to the Flipper Zero as shown.

| esp32 | flipper |
|-------|---------|
|  TX   |  RX     |
|  RX   |  TX     |

| esp32 | converter |
|-------|-----------|
|3.3V   |Vo         |
|GND    |GND        |

| flipper | converter |
|---------|-----------|
|GND      |GND        |
|5V       |Vi         |

5. Now, we need to connect GPIO 0 to GND using tweezers or a wire on the ESP32. Then, switch to the ESP32 flasher on the Flipper and select the Marauder firmware to install.

6. Now, assemble the Flipper and, by entering the ESP32 Marauder, you will be able to utilize the ESP32.

-----

## ❤️ Thank You for Your Support!
If you appreciate this project and want to show your support, consider buying me a cup of coffee! ☕ 

**BTC Address:** `3PpBpNs1wXkhA93g5tfpMf4qierz4m9BCW` (this is a **SegWit** address)

Every donation you make is deeply appreciated and will help in the ongoing development of this project!

-----

### 🌐 Follow Me for Updates
Stay connected and receive the latest updates:

[![GitHub](https://img.shields.io/badge/GitHub-W0rthlessS0ul-181717?style=flat&logo=github&logoColor=white)](https://github.com/W0rthlessS0ul)
