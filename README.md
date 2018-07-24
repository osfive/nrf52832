# nrf52832

Connect UART pins as follows:

| nrf52832          | UART-to-USB adapter  |
| ----------------- | -------------------- |
| P0.08 (RX)        | TX                   |
| P0.07 (TX)        | RX                   |

UART baud rate: 115200

Connect SWD pins as follows:

| nrf52832          | STLink v2 adapter    |
| ----------------- | -------------------- |
| SDO               | SWDIO                |
| SCLK              | SWCLK                |

### Build under Linux

    $ export CROSS_COMPILE=arm-none-eabi-
    $ git clone --recursive https://github.com/osfive/nrf52832
    $ cd nrf52832
    $ bmake

### Build under FreeBSD

    $ setenv CROSS_COMPILE arm-none-eabi-
    $ git clone --recursive https://github.com/osfive/nrf52832
    $ cd nrf52832
    $ make
