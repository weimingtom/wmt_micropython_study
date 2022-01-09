# wmt_micropython_study
My micropython study

## ref  
* http://www.lcdwiki.com  
* https://github.com/mcauser/awesome-micropython  
* https://github.com/icopy-site/awesome-cn/blob/master/docs/awesome/awesome-micropython.md  
* http://docs.micropython.01studio.org/zh_CN/latest/  
* http://vcc-gnd.com/PYB/html/index.html  

## GUI  
* https://github.com/peterhinch/micropython-lcd160cr-gui  

## rshell  
* https://github.com/dhylands/rshell  
* https://github.com/tuupola/micropython-ili934x/blob/master/Makefile  

## oled12864, i2c, ssd1306  
* see http://www.lcdwiki.com/0.96inch_OLED_Module_MC096VX  
* wio-rp2040  
see https://github.com/makerportal/rpi-pico-ssd1306/blob/main/micropython/rpi_demo/main.py  
see https://github.com/micropython/micropython/tree/master/drivers/display  
search baidupan, 20220107.rar  
oled12864<->wio-rp2040:  
VCC<->right top 2  
GND<->right top 3  
SCL<->right top 6(GP27)  
SDA<->right top 7(GP26)  

## 信泰微, spi, ili9341, 2.4 inch tft  
* see http://www.lcdwiki.com/2.4inch_SPI_Module_ILI9341_SKU:MSP2402  
* wio-rp2040  
see https://github.com/tabris2015/rpi-pico-oscilloscope  
see https://github.com/mcauser/deshipu-micropython-ili9341  
see https://github.com/tuupola/micropython-ili934x  
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

* m5stack  
see https://github.com/jeffmer/micropython-ili9341  
