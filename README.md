# 1.9InchESP32Controller

这是一个由ESP32为主控制作的控制器，他的主要硬件包括：
1. ESP32
2. CH340K
3. 1.9Inch IPS屏幕  ST7789_DRIVER 170*320
   
使用了以下的库：
1. TFT_espi
2. LVGL

硬件IO分配：
#define TFT_CS   27  // Chip select control pin (library pulls permanently low
#define TFT_DC   14  // Data Command control pin - must use a pin in the range 0-31
#define TFT_RST  -1  // Reset pin, toggles on startup

#define TFT_WR    12  // Write strobe control pin - must use a pin in the range 0-31
#define TFT_RD    13  // Read strobe control pin

#define TFT_D0   2  // Must use pins in the range 0-31 for the data bus
#define TFT_D1   4  // so a single register write sets/clears all bits.
#define TFT_D2   16  // Pins can be randomly assigned, this does not affect
#define TFT_D3   17  // TFT screen update performance.
#define TFT_D4   5
#define TFT_D5   18
#define TFT_D6   19
#define TFT_D7   23

#define TFT_BL   15            // LED back-light control pin
#define TFT_BACKLIGHT_ON HIGH  // Level to turn ON back-light (HIGH or LOW)
