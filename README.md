# Serpente

A tiny and cheap CircuitPython development board, perfect for quick projects and prototyping!

## Hardware
- ATSAMD21E18A Cortex-M0+ @ 48MHz, 256KB FLASH, 32KB RAM
- 4MB Flash for storing Python files
- 6 GPIOs
- 250mA LDO
- User-controlled RGB LED
- USB Type-C receptacle

## GPIOs

All 6 GPIOs are PWM-capable.

Additionally, the GPIOs can be configured as the following protocol combos:

- SPI + 2 GPIOs (3 if you skip CS)
- I2C + 4 GPIOs
- UART + 4 GPIOs
- 2x UART + 2 GPIOs
- SPI + I2C (+ 1 GPIO if you skip CS)
- SPI + UART (+ 1 GPIO if you skip CS)
- I2C + UART + 2 GPIOs

TODO: Add pin mappings for each combo
