# ESP8266_4Mbit_AT_Firmware

This is a backup of the latest AT firmware I found that works with ESP8266 modules with 4Mbit memory and accepts v0.30 commands like "AT+UART_CUR". Default baudrate is 115200kbps.
The original files (AT_V1.0_on_ESP8266_NONOS_SDK_V1.5.3.zip) were downloaded from http://bbs.espressif.com/download/file.php?id=1352

To flash the module on linux just run Flash_AT.sh, the ESP8266 is supposed to be connected through an USB serial adapter on /dev/ttyUSB0.
