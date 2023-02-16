# ST25DV Driver
WARNING!!!

This repository is now deprecated and not maintained any more!

WARNING!!!

This is a driver needed by `NFCEEPROOM` constructor for the ST25DV NFC chip.

## Requirements

This driver requires the ST25DV NFC chip. This is present on the X-NUCLEO-NFC04A1 expansion board.

## Configuration

Driver needs to be instantiated with valid pin names for I2C communication, GPO and RF disable pin.

If you are using an X-NUCLEO-NFC04A1 expansion board please edit `mbed_lib.json` and set the value of `X_NUCLEO_NFC04A1` to `true`. This will set appropriate defaults for you.

Otherwise, the driver will require passing valid pin names during instantiation explicitly.

## Building instructions

Driver will be built as part of the mbed-os build. Place the driver in the root directory of the mbed-os application. This can be done by placing a `.lib` file in the root of your application with a repository address with the driver. For example, to include this driver you can create a file called `eeprom_driver.lib` with these contents:

```
https://github.com/STMicroelectronics/mbed-nfc-st25dv
```
