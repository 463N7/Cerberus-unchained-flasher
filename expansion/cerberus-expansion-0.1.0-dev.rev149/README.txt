CERBERUS UNCHAINED - WROOM EXPANSION FIRMWARE - EXPERIMENTAL
For ESP32-C5-WROOM-1 / WROOM-1U with at least 4 MB flash.
This is the extra Wardriving radio image. Use the main installer for the onboard C5.
Install one module at a time through a 3.3 V logic USB-to-UART adapter.
Adapter TX -> C5 RX0/GPIO12; adapter RX -> C5 TX0/GPIO11; common GND.
Supply the module with regulated 3.3 V rated for at least 600 mA.
With GPIO27 high, hold BOOT/GPIO28 low and pulse EN low then high.
Flash offsets: bootloader 0x2000, partition table 0x8000, application 0x10000.
Release BOOT and reset EN after verification. UART transfers use 115200 baud.
Runtime SPI pins: SCLK 8, MOSI 10, MISO 9, CS 23; IRQ disabled.
The same image accepts slot configuration 1-6 from Cerberus. Scanning starts disabled.
Expansion protocol 3, capability firmware 1; packaged with Cerberus rev149.
Build checks are not physical expansion-board acceptance. Verify your fitted board.
Retain the included licenses. No board diagnostics or firmware source are included.
