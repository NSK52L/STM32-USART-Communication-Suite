# STM32 USART Communication Suite

This project demonstrates the implementation of serial communication using the **USART** protocol on the **STM32F411** microcontroller. It covers two distinct hardware configurations developed using **STM32CubeIDE** and **HAL drivers**.

## 🛠️ Project Configurations

### 1. USART to PC Communication
* **Objective:** Establish a serial link between the STM32 board and a PC terminal.
* **Setup:** Uses a USB-TTL module connected to PA2 (TX) and PA3 (RX).
* **Verification:** Data is monitored via PuTTY at a baud rate of 115200.

### 2. Internal USART1 ↔ USART2 Bridge
* **Objective:** Validate internal peripheral communication by cross-connecting two USART units on the same board.
* **Wiring:** PA9 (TX1) → PA3 (RX2) and PA10 (RX1) → PA2 (TX2).
* **Verification:** Validated via multimeter voltage checks (~3.3V) on RX pins to confirm active transmission.

## 🚀 Getting Started
1. Clone the repository.
2. Open the desired configuration folder in **STM32CubeIDE**.
3. Compile and flash the code to your STM32F411 board.
4. Refer to the `Documentation/` folder for the full technical presentation.

## 📁 Repository Structure
* `/Config1-UART-to-PC`: Source code for PC-based communication.
* `/Config2-Internal-USART`: Source code for inter-peripheral communication.
* `/Media`: Demonstration videos of the hardware in action.
* `/Documentation`: Technical report (French) and project presentation.

## 🔧 Tools Used
* **Hardware:** STM32F411 (BlackPill/Nucleo), USB-TTL Module, Multimeter.
* **Software:** STM32CubeIDE, PuTTY.
