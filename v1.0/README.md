# BOOT MODE
## download
### Flash size 4Mbit: 512KB
    boot_v1.2+.bin              0x00000
    user1.1024.new.2.bin        0x01000
    esp_init_data_default.bin   0x7C000
    blank.bin                   0x7e000 & 0xfe000


> NOTICE: UPDATE is not supported in non-boot mode; 4Mbit Flash is not supported in non-boot mode;

# Update steps
1.Make sure TE(terminal equipment) is in sta or sta+ap mode

    AT+CWMODE=3
    OK

2.Make sure TE got ip address

    AT+CWJAP="ssid","12345678"
    OK
    
    AT+CIFSR
    192.168.1.134

3.Let's update

    AT+CIUPDATE
    +CIPUPDATE:1    found server
    +CIPUPDATE:2    connect server
    +CIPUPDATE:3    got edition
    +CIPUPDATE:4    start start
    
    OK

> NOTICE: If there are mistakes in the updating, then break update and print ERROR.
