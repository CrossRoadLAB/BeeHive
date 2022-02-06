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
  
|||
|:--------------------------------------:|:--------------------------------------------------------------------------------------------------------------------------------------:|
| **CPU and MEMORY**                         | 32-bit Xtensa® dual-core LX7 microprocessor, up to 240 MHz                                                                             |
|                                        | 128-bit data bus and SIMD commands                                                                                                     |
|                                        | 384 KB ROM                                                                                                                             |
|                                        | 512KB SRAM, 16KB SRAM in RTC + 8MB PSRAM                                                                                             |
|                                        | 8 MB SPI flash                                                                                                                         |
|                                        | SPI, Dual SPI, Quad SPI, Octal SPI, QPI and OPI interfaces                                                                          |
|                                        | Cached flash controller is supported                                                                                                   |
|                                        | In-circuit flash programming (ICP) is supported                                                                                        |
| **DIGITAL INTERFACES**                     | 4 x SPI                                                                                                                                |
|                                        | 1 x LCD interface (8-bit ~ 16-bit parallel RGB, I8080 and MOTO6800), supporting conversion between RGB565, YUV422, YUV420 and YUV411 |
|                                        | 1 x DVP 8-bit ~ 16-bit camera interface                                                                                                |
|                                        | 3 x UART                                                                                                                               |
|                                        | 2 x I2C                                                                                                                                |
|                                        | 2 x I2S                                                                                                                                |
|                                        | 1 x RMT (TX / RX)                                                                                                                      |
|                                        | 1 x Pulse counter                                                                                                                      |
|                                        | PWM LED controller, up to 8 channels                                                                                                  |
|                                        | 1 x USB OTG (USB1 and USB2)                                                                                                            |
|                                        | 1 x USB Serial / JTAG Controller                                                                                                       |
|                                        | 2 x MCPWM                                                                                                                              |
|                                        | 1 x SDIO host controller with 2 slots                                                                                                  |
|                                        | General DMA controller (GDMA), with 5 transmission channels and 5 reception channels                                                  |
|                                        | 1 x TWAI® Controller, compatible with ISO 11898-1 (CAN Specification 2.0)                                                             |
| **ANALOG INTERFACES**                      | 2 x 12-bit SAR ADC, up to 20 channels                                                                                                  |
|                                        | 1 x temperature sensor                                                                                                                 |
|                                        | 14 x IO touch detection                                                                                                                |
| **TIMER**                                  | 4 x 54-bit general purpose timer                                                                                                       |
|                                        | 1 x 52-bit system timer                                                                                                                |
|                                        | 3 x watchdog timer                                                                                                                     |
| **LOW POWER MANAGEMENT**                   | Power management unit with five power modes                                                                                            |
|                                        | Ultra-Low-Power (ULP) Coprocessors: - ULP-RISC-V Coprocessor - ULP-FSM Coprocessor                                                     |
| **SECURITY**                               | Safe Boot                                                                                                                              |
|                                        | Flash encryption                                                                                                                       |
|                                        | 4096-bit OTP, up to 1652-bit for users                                                                                                 |
| **HARDWARE ACCELERATION FOR CRYPTOGRAPHY** | AES-128/256 (FIPS PUB 197)                                                                                                             |
|                                        | Hash (FIPS PUB 180-4)                                                                                                                  |
|                                        | RSA                                                                                                                                    |
|                                        | Random Number Generator (RNG)                                                                                                          |
|                                        | HMAC                                                                                                                                   |
|                                        | Digital signature                                                                                                                      |
| **WIFI**                                   | IEEE 802.11 b / g / n                                                                                                                  |
|                                        | 4 x virtual Wi-Fi interfaces                                                                                                           |
| **BLUETOOTH**                              | Bluetooth LE: Bluetooth 5, Bluetooth network                                                                                           |
|                                        | Speed: 125 Kbps, 500 Kbps, 1 Mbps, 2 Mbps                                                                                              |
|                                        | Internal mechanism of coexistence between Wi-Fi and Bluetooth to share the same antenna                                                |

<h1 align="center"> PINOUT </h1>

![BeeHive_pinout](https://user-images.githubusercontent.com/83240004/152701905-e9565f18-011b-4155-afdd-153d705dddf1.png)
![BeeHive](https://user-images.githubusercontent.com/83240004/152701933-6a1ecb0d-0810-49ef-bb38-5fc77ad8c0f4.png)

- **AMS117 3.3V**: Power regulator that converts a 4.5 to 12V input power into a 3.3V output.
- **USB to UART Port**: A Micro-USB port used for powering the board, for flashing applications on the chip, as well as for communicating with the chip via the built-in USB to UART bridge.
- **Boot Button**: Download button. Holding down the Boot button and then pressing the Reset button starts the firmware download mode via the serial port.
- **Reset Button**: Press this button to restart the system.
- **ESP32-S3 USB port (USB1 and USB2)**: USB OTG interface compliant with USB 1.1 specification. The interface is used for powering the board, for flashing applications on the chip, for communicating with the chip via USB 1.1 protocols, as well as for JTAG debugging. There are two USB OTG ports (Micro-USB and USB 2.0 type A) in which the use of one excludes the use of the other.
- **USB to UART bridge**: The chip that bridges the USB to UART offers a data transfer rate of up to 3 Mbps.
- **RGB LED**: Addressable RGB LED, driven by GPIO48.
- **3.3V Power LED**: Lights up when USB power is connected to the board.
