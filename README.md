# KEX a Rapid Deployment ESP32 Board
A fast and feature-rich implementation of an ESP32 board with NeoPixel Led (WS2812B, WS2811, SK6812), I2S (Digital microphone) and I2C outputs.

<img src="/images/Bottom.png" width="50%"><img src="/images/Top.png" width="50%">


## ⚙️ Features
- Supports USB C to USB C cables at 5V 3A 
- 3 Capacitive Touch Buttons
- Designed for PCB Assembly by JLCPCB 
- 3A Resettable Fuse on both the 3.3v and 5v Rails
- Programming using the CH30-c IC
- Electrostatic Discharge Protection on USB and LED Output
- Auto Reset for easy programming
- Solder Pad connections with Strain relief slots 
- High-Speed Level shifted I2S and I2C ports using BSS138 with cuttable solder pads to select between 3.3v and 5v 
- LED indicators on all outputs and inputs
- Easy soldering of led strips directly to the PCB with Strain Releaf slots


## 📲 Quickstart for WLED
1. Solder the ESP32 to the footprint on the PCB

2. Connect up to 120 NeoPixels (WS2812B, WS2811, SK6812) to the output pads (IO2). 

3. Flash the software to your ESP module! There are two options for this step:

[I just want to use WLED! (install release binary)](https://install.wled.me/)

[I want to modify WLED (compile from source code)](https://kno.wled.ge/advanced/compiling-wled/)

If set up correctly, the first thirty LEDs will light up!

4. Use a WiFi device to connect to the access point WLED-AP using the default password wled1234. You can also scan this QR code:

![Wifi Connect QR Code](https://i.ibb.co/h2YswXK/WLED-QR-Connect-WB.png)

5. Click on the cog icon to edit settings like connecting the module to your home WiFi.
6. Upload Config File (Coming soon...)

## 💾 Pinout
Pin | IO2 | IO4 | IO14 | IO15 | IO21 | IO22 | IO27 | IO32 | IO33 | IO36
--- | --- | --- | --- |--- |--- |--- |--- |--- |--- |---
Usage | LED Output | Down TouchPad | SCK | WS | SDA | SCL | Middle TouchPad | SD |  Up TouchPad | Analog Input 
LED | Yellow | | White | White | Red | Green | | White | | |
Level Shifted | | |✅|✅|✅|✅| |✅| 


## ✌️ Other

[Licensed under the MIT license](https://github.com/git/git-scm.com/blob/main/MIT-LICENSE.txt)

Designed by Chris Dirks (@CD_FER)

You can also send me mails to [cdirksfer@gmail.com](mailto:dev.cdirksfer@gmail.com), but please only do so if you want to talk to me privately.
