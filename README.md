<h1 align="center">
<img src="https://user-images.githubusercontent.com/83240004/152610107-5a7dc7a1-5672-450c-8c03-67d5b249ba0e.png" width="400" height="auto"/>
</h1>

<p align="center">
<img src="https://user-images.githubusercontent.com/83240004/152610874-a6f50491-0fa8-49ae-8bb3-06131d5f68c3.png" width="720" height="auto"/>
</p>

<h1 align="center">GENERAL INFORMATION</h1>

**BeeHive** is a development board equipped with ESP32-S3-WROOM-1, a general purpose Wi-Fi + Bluetooth LE MCU module that integrates full Wi-Fi and Bluetooth LE functions (datasheet). The "heart" of BeeHive is an ESP32-S3-WROOM-1 module (PCB antenna) with 8 MB of Flash and 8 MB of PSRAM. The ESP32-S3 SoC features a 32-bit Xtensa® LX7 CPU running at up to 240 MHz and a (low-power) coprocessor that can be used to constantly monitor peripherals if needed, after shutting down the CPU. The ESP32-S3 integrates a rich set of peripherals including SPI, LCD, camera interface, UART, I2C, I2S, remote control, pulse counter, PWM LED, USB Serial / JTAG controller, MCPWM, SDIO host, GDMA, TWAI controller ® (compatible with ISO 11898-1), ADC, touch sensor, temperature sensor, timer and watchdog, as well as up to 45 GPIOs. It also includes a USB 1.1 OTG interface (USB1 and USB2).
There are three mutually exclusive ways to provide power to the board:
- USB-UART port and ESP32-S3 USB port (one or both), default power supply (recommended)
- Pin 5V and GND
- Pin 3v3 and GND

<p align="center">
  ⚠️ <b>ATTENTION</b> ⚠️
</p>
<p align="center">
There is currently no support for Arduino IDE or CircuitPython, only for ESP IDF
 </p>
 
<h1 align="center"> SPECIFICATIONS </h1>
 
 |                **CPU e MEMORIA**               | Microprocessore Xtensa® dual-core LX7 a 32 bit, fino a 240 MHz                                                                          |
|||
|                                                | Bus dati a 128 bit e comandi SIMD                                                                                                       |
|                                                | 384 KB ROM                                                                                                                              |
|                                                | 512 KB SRAM, 16 KB SRAM in RTC + 8MB PSRAM                                                                                              |
|                                                | 8 MB SPI flash                                                                                                                          |
|                                                | Interfacce SPI, Dual SPI, Quad SPI, Octal SPI, QPI e OPI                                                                                |
|                                                | È supportato il controller flash con cache                                                                                              |
|                                                | È supportata la programmazione flash in-circuit (ICP)                                                                                   |
|             **INTERFACCE DIGITALI**            | 4 × SPI                                                                                                                                 |
|                                                | 1 × interfaccia LCD (RGB parallelo a 8 bit ~ 16 bit, I8080 e MOTO6800), che supporta la conversione tra RGB565, YUV422, YUV420 e YUV411 |
|                                                | 1 × Interfaccia fotocamera DVP 8-bit ~16-bit                                                                                            |
|                                                | 3 × UART                                                                                                                                |
|                                                | 2 × I2C                                                                                                                                 |
|                                                | 2 × I2S                                                                                                                                 |
|                                                | 1 × RMT (TX/RX)                                                                                                                         |
|                                                | 1 × Contatore di impulsi                                                                                                                |
|                                                | Controller LED PWM, fino a 8 canali                                                                                                     |
|                                                | 1 × USB OTG (USB1 e USB2)                                                                                                               |
|                                                | 1 × Controller USB Seriale/JTAG                                                                                                         |
|                                                | 2 × MCPWM                                                                                                                               |
|                                                | 1 × Controller host SDIO con 2 slot                                                                                                     |
|                                                | Controller DMA generale (GDMA), con 5 canali di trasmissione e 5 canali di ricezione                                                    |
|                                                | 1 × Controller TWAI®, compatibile con ISO 11898-1 (Specifica CAN 2.0)                                                                   |
|            **INTERFACCE ANALOGICHE**           | 2 × ADC SAR a 12 bit, fino a 20 canali                                                                                                  |
|                                                | 1 × sensore di temperatura                                                                                                              |
|                                                | 14 × IO di rilevamento del touch                                                                                                        |
|                    **TIMER**                   | 4 × Timer per uso generico a 54 bit                                                                                                     |
|                                                | 1 × Timer di sistema a 52 bit                                                                                                           |
|                                                | 3 × watchdog timer                                                                                                                      |
|          **GESTIONE A BASSA POTENZA**          | Unità di gestione dell'alimentazione con cinque modalità di alimentazione                                                               |
|                                                | Coprocessori Ultra-Low-Power (ULP): - Coprocessore ULP-RISC-V - Coprocessore ULP-FSM                                                    |
|                  **SICUREZZA**                 | Avvio sicuro                                                                                                                            |
|                                                | Crittografia flash                                                                                                                      |
|                                                | OTP a 4096 bit, fino a 1652 bit per gli utenti                                                                                          |
| **ACCELERAZIONE HARDWARE PER LA CRITTOGRAFIA** | AES-128/256 (FIPS PUB 197)                                                                                                              |
|                                                | Hash (FIPS PUB 180-4)                                                                                                                   |
|                                                | RSA                                                                                                                                     |
|                                                | Generatore di numeri casuali (RNG)                                                                                                      |
|                                                | HMAC                                                                                                                                    |
|                                                | Firma digitale                                                                                                                          |
|                    **WIFI**                    | IEEE 802.11 b/g/n                                                                                                                       |
|                                                | 4 × interfacce Wi-Fi virtuali                                                                                                           |
|                  **BLUETOOTH**                 | Bluetooth LE: Bluetooth 5, rete Bluetooth                                                                                               |
|                                                | Velocità: 125 Kbps, 500 Kbps, 1 Mbps, 2 Mbps                                                                                            |
|                                                | Meccanismo interno di coesistenza tra Wi-Fi e Bluetooth per condividere la stessa antenna                                               |
