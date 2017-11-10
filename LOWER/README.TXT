this is the project for lower part;
build on Keil.
device:
	Minimum developer board with STM32F103.
function:
	1. ADC captures wave data; 
	2. Upload data to the upper Master part(Android device);
	3. Show the status of the lower part ;

硬件资源:	
	1,DS0(连接在PA8),DS1(连接在PD2)
	2,串口1(波特率:9600,PA9/PA10连接在板载USB转串口芯片CH340上面)
	3,ALIENTEK 2.8/3.5/4.3/7寸TFTLCD模块(通过GPIO驱动,连接关系见lcd.h) 	
	4,串口2(波特率:9600,PA2/PA3接蓝牙模块的RXD和TXD)
	5,按键KEY0(PC5)/KEY_UP(PA0,也称之为WK_UP)
	6,ATK-HC05蓝牙模块，同Mini板的连接关系如下:
	STM32开发板-->ATK-HC05蓝牙模块
			PA2-->RXD
			PA3-->TXD
			PC4-->KEY
			PA4-->LED
			GND-->GND
		5V/3.3V-->VCC 
			 
 
