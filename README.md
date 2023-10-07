# 1.9InchESP32Controller

这是一个由ESP32为主控制作的控制器，他的主要硬件包括：
1. ESP32
2. CH340K
3. 1.9Inch IPS屏幕  ST7789_DRIVER 170*320
   
使用了以下的库：
1. TFT_espi
2. LVGL

硬件IO分配：
 #define TFT_CS   27 
 
 #define TFT_DC   14
 
 #define TFT_RST  -1

 #define TFT_WR    12
 
 #define TFT_RD    13

 #define TFT_D0   2
 
 #define TFT_D1   4
 
 #define TFT_D2   16
 
 #define TFT_D3   17
 
 #define TFT_D4   5
 
 #define TFT_D5   18
 
 #define TFT_D6   19
 
 #define TFT_D7   23

 #define TFT_BL   15
 
 #define TFT_BACKLIGHT_ON HIGH
 
 
其余引出的IO已经标识在板子背面
