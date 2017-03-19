This project is a port of the [Lora-net LoRaWAN stack implementation](https://github.com/Lora-net/LoRaMac-node) to work on the EFM32 Giant Gecko (STK3700) hardware with a HopeRF RFM95W radio (which is compatible with the SX1276).

Note that some parts were not ported (e.g. I2C and GPS), only the code required to use the radio and the uart are implemented.

To compile one of the apps, update `Makefile.local` (or set the `TARGET` environment variable) and run `make` from the root directory. To compile e.g. the class A end-device code from `src/apps/LoRaMac/classA/EFM32GG_STK3700`, the `TARGET` variable should be `LoRaMac/classA`.
