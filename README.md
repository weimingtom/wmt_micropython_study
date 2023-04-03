# wmt_micropython_study
My micropython study

## ref  
* http://www.lcdwiki.com  
* https://github.com/mcauser/awesome-micropython  
* https://github.com/icopy-site/awesome-cn/blob/master/docs/awesome/awesome-micropython.md  
* http://docs.micropython.01studio.org/zh_CN/latest/  
* http://vcc-gnd.com/PYB/html/index.html  

## Thonny 3.3.13   
* https://thonny.org/  
* main.py, not need if only run with Thonny  

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

## 中景园 IPS 240x240, st7789, 1.54inch, 240x240  
* wio-rp2040  
see https://gitee.com/eetree-git/RP2040_Game_Kit  
see https://www.eetree.cn/project/detail/698  
search game2040-V3-20211228.pdf  
search baidupan, 20230402.rar, 20230402.zip    
st7789 1.54inch 240x240 tft<->wio-rp2040, usb type c and run button on top left, chip face to me  
GND<->right top 3  
VCC<->right top 2  
SCL<->IO2 //left top 4, spi0_sck  
SDA<->IO3 //left top 5, spi0_tx  
RES<->IO0 //left top 1 //see st7789_res=0  
DC<->IO1  //left top 2 //see st7789_dc=1  
BLK<->NC  

## waveshare st7789 2.0inch lcd module 320x240  
* rpi pico  
rpipico_v2_dino_success_use_waveshare_rp2040_zero.rar  
waveshare st7789 2.0inch lcd module 320x240 tft<->rpi pico  
VCC<->right top 2  
GND<->right top 3  
DIN(SDA)<->IO3 //left top 5, spi0_tx  
CLK(SCL)<->IO2 //left top 4, spi0_sck  
CS<->IO5//left top7  
DC<->IO1  //left top 2 //see st7789_dc=1  
RST(RES)<->IO0 //left top 1 //see st7789_res=0  
BL(BLK)<->IO13 //left bottom 4  
