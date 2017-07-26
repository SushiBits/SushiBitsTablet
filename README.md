# SushiBits Tablet

An open source tablet based on Allwinner V3s platform

## Introduction

This project came from my idea of [trying to create a single board computer
without touching any BGA chips](https://github.com/xcvista/AT91SAM9260-SBC).
During my research talking with folks on the EEVBlog forum, someone pointed me
to the [Allwinner V3s][V3s] microprocessor: it is a microprocessor in LQFP
package, with 64MB DDR2 memory built in. This is definitely a win for this
project, as I can solder this package without an oven.

## Features

*   Connectivity options: wired Ethernet, 802.11b/g/n Wi-Fi and Bluetooth 4.0,
    USB 2.0 OTG, and a UART in another USB port.
*   Display: 7in 1024x600 LCD, capacitive touchscreen.
*   Fully open source: hardware and software.

## Components

The primary components for this project includes:

*   [Allwinner V3s][V3s]: ARM Cortex-A7 MP1 @1.2GHz, with
    64MB DDR2-800 memory built in. The chip supports parallel LCD and MIPI CSI.
*   STMicroelectronics STM32F405RGT6: Embedded platform controller.
*   [Spanson S25FL512S][S25FL512S]: 64MB SPI NOR Flash holding the firmware.
*   Realtek RTL8723BS: 802.11b/g/n SDIO Wi-Fi and Bluetooth module.
*   microSD card slot. The card can be used for storing pictures, or booting the
    board with custom U-Boot, kernel and root filesystem.
*   7in LCD screen with capacitive touch.

## More Information

If you want to contribute to this project, please refer to the [contribution
manual](CONTRIBUTE.md) and [hardware design rules](DESIGN-RULES.md).

This is [open source hardware](http://www.oshwa.org/), licensed under the
[3-clause BSD license](LICENSE.md).

[V3s]: http://linux-sunxi.org/V3s
[S25FL512S]: http://www.cypress.com/file/177971/download
[LCD]: http://www.forlinx.net/products_detail/productId=54.html
