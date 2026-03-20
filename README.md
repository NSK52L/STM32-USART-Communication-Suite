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

## 📁 Repository Structure
* `/Config1-UART-to-PC`: Source code for PC-based communication.
* `/Config2-Internal-USART`: Source code for inter-peripheral communication.
* `/Documentation`: Technical report (French) and project presentation.

## 🔧 Tools Used
* **Hardware:** STM32F411 DISCOVERY, USB-TTL Module, Multimeter.
* **Software:** STM32CubeIDE, PuTTY.

## 📺 Project Demonstrations
To see the hardware validation in action without downloading the source files, you can view the testing videos here:
* 🔗 [**View Project Media on Google Drive**](https://drive.google.com/drive/folders/12nkhgyfenuASvPNbNkTc4bNq4IbpNtzI?usp=sharing)
