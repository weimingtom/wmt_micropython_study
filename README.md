# wmt_micropython_study
My micropython study

## oled12864, i2c, ssd1306  
<> wio-rp2040  
see https://github.com/makerportal/rpi-pico-ssd1306/blob/main/micropython/rpi_demo/main.py  
search baidupan, 20220107.rar  
oled12864<->wio-rp2040:  
VCC<->right top 2  
GND<->right top 3  
SCL<->right top 6(GP27)  
SDA<->right top 7(GP26)  

## 信泰微, spi, ili9341, 2.4 inch tft  
<> wio-rp2040  
see https://github.com/tabris2015/rpi-pico-oscilloscope  
search baidupan, 20220109.rar   
ili9341 2.4inch tft<->wio-rp2040  
VCC<->right top 2  
GND<->right top 3  
SCK<->right bottom 6  
MOSI(SDI)<->right bottom 7  
MISO(SDO)<->right bottom 4(not necessary)  
CS<->left bottom 5(or GND, left bottom 3)  
RST(RESET)<->left bottom 4  
DC<->left bottom 2  
LED(power)<->left bottom 1  
