## LPC13xx chip support library

This is identical to the official LPCOpen LPC13xx chip support library
which can be found [here][LPCOpen LPC13xx library]

Changes are mostly fixes:

* timer_13xx - added PWMC register
* extern "C" guards in few places
* i2cm_13xx - simple I2C debugging helper: define DEBUG_I2C and inspect i2cdebuginfo buffer in i2cm_13xx.c when stepping through code
* iart_13xx - fixed possible error when calculating mval for dval == 0 in fractional baud rate UART setting


TODO:

* timer_13xx - CRxINT bits have different positions for TIMER0 (4,6) and TIMER1 (4,5)





[LPCOpen LPC13xx library]: http://www.nxp.com/products/software-and-tools/hardware-development-tools/lpcxpresso-boards/lpcopen-software-development-platform-lpc13xx:LPCOPEN-SOFTWARE-FOR-LPC13XX
