# Serpente

A tiny and cheap CircuitPython development board, perfect for quick projects and prototyping!

Comes in two versions: USB Type-C and bare PCB USB A plug.

## Hardware
- ATSAMD21E18A Cortex-M0+ @ 48MHz, 256KB FLASH, 32KB RAM
- 4MB Flash for storing Python files
- 6 GPIOs
- 250mA LDO
- User-controlled RGB LED

## GPIOs

All 6 GPIOs are PWM-capable.

Additionally, the GPIOs can be configured as the following protocol combos:

- SPI + 2 GPIOs (3 if you skip CS)
  - D0 - GPIO
  - D1 - GPIO
  - D2 - CS
  - D3 - MISO
  - D4 - SCK
  - D5 - MOSI
- I2C + 4 GPIOs
  - D0 - SCL
  - D1 - SDA
  - D2 - GPIO
  - D3 - GPIO
  - D4 - GPIO
  - D5 - GPIO
- UART + 4 GPIOs
  - D0 or D4 - RX
  - D1 or D5 - TX
  - D2 - GPIO
  - D3 - GPIO
- 2x UART + 2 GPIOs
  - D0 - RX2
  - D1 - TX2
  - D2 - GPIO
  - D3 - GPIO
  - D4 - RX0
  - D5 - TX0
- SPI + I2C (+ 1 GPIO if you skip CS)
  - D0 - SCL
  - D1 - SDA
  - D2 - CS
  - D3 - MISO
  - D4 - SCK
  - D5 - MOSI
- SPI + UART (+ 1 GPIO if you skip CS)
  - D0 - RX2
  - D1 - TX2
  - D2 - CS
  - D3 - MISO
  - D4 - SCK
  - D5 - MOSI
- I2C + UART + 2 GPIOs
  - D0 - SCL
  - D1 - SDA
  - D2 - GPIO
  - D3 - GPIO
  - D4 - RX
  - D5 - TX
