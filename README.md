## RF95_LoRa
### Introduction
This is coming from the Radio Head library and streamlining of, applicable to RF95, support for the Arduino and LinkNode D1 (ESP8266) platform.the library includes 4 examples,```rf95_client```,```rf95_server```,```rf95_reliable_datagram_client```,```rf95_reliable_datagram_server```.

### Arduino UNO
Arduino UNO and Link LoRa Radio,don't need to modify the program.the pin map is:

| Arduino UNO | Linker LoRa radio |
| ------------|:-----------------:|
|   D13       |  SCK              |
|   D11       |  MOSI             |
|   D12       |  MISO             |
|   D10       |  NSS              |
|   D4        |  RST              |
|   D2        |  DIO0             |
|   3.3V      |  VCC              |
|   GND       |  GND              |

### LinkNode D1
LinkNode D1 and Link LoRa Radio,you should change the code like below:
```RH_RF95 rf95(15, 5);```
The pin map is:

| Arduino UNO | Linker LoRa radio |
| ------------|:-----------------:|
|   GPIO14    |  SCK              |
|   GPIO13    |  MOSI             |
|   GPIO12    |  MISO             |
|   GPIO15    |  NSS              |
|   GPIO4     |  RST              |
|   GPIO5     |  DIO0             |
|   3.3V      |  VCC              |
|   GND       |  GND              |