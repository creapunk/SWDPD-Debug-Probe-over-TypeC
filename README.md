# SWDPD-Debug-Probe-over-TypeC

Board with online and offline firmware flashing via SWD, power control via PD and communication via USB.

## Overview

SWDPD is a universal, multifunctional, and compact programmer and debugger that offers a fundamentally new approach to the development of embedded systems using the versatility of the USB Type-C standard. The programmer combines a range of very advanced features, such as support for SWD protocols for programming and UART/SPI/I2C/UART/PD for communication with the programmable device, integrated power control and monitoring systems, protection against overload/voltage surges/electrostatics, and compatibility with 3.3V/5V logic. The presence of built-in memory and an OLED display allows saving firmware or interface testing protocols on the programmer and using it offline without a computer.

------

## ✨ Features

- Reset via power supply reboot
- logging to internal memory
- OLED display for interaction

------

## 💻 Applications

- 🔧 **Ontline or Offline SWD programmer and debuger**
- 🔌 **PD trigger with message interception**
- ⚡ **Portable Laboratory Power Supply (LPS) with:**
	- **5-21V:** 20mV steps in SPR PPS Mode
	- **20-48V:** 100mV steps in EPR AVS Mode
- 🔋 **Battery Charger Controller** (an external BMS may be required)
- 📈 **Portable power meter**

------

## ⚡Electrical characteristics

- **Input voltage:** 5-50VDC with surge protection
- **Current ratings:** 5A continuous with overcurrent protection
- **VBUS Line Resistance:** 70mΩ max (40mΩ contact resistance + 15mΩ mosfet RDSON + 10mΩ current sensing resistor + 5mΩ traces resistance)
- **System voltage source:** internal synchronous DC-DC converter
- **System power consumption:** <100mW
- Integrated load switch
- Integrated power meter resolution: 
	- Voltage: 0-48V with 0.1mV step
	- Current: 0-6A with 0.1mA step
	- Power: 240W with 0.01mW step

------

## 🔄 Programming capabilities

- **Supported target communication interfaces**:
	- SWD (DIO and CLK) with line auto detection
	- Power Delivery 2.0 / 3.0 / 3.1 with SPR and EPR support on both connectors
	- QuiqCharge 
	- Half duplex SPI 2 wire (DIO and SCL)
	- Classic UART and UART Single Wire
	- I2C with digital controlled 3.3V 2.2kΩ pull-up
- **Program-Selectable USB2.0 endpoint:** SWDPD Programmer or Target Device
- **Interface frequency:** up to 30MHz
- **External FLASH memory size**: 16MB для хранения прошивок и инструкций тестирования

------

## 🖥️ MCU Performance and External interfaces

**MCU:** High-performance Arm Cortex-M4 MCU **STM32G431CB** running at **170MHz** with:

- **128KB Flash** memory and **32KB SRAM** memory and **1Kb OTP**
- Math accelerator with trigonometric functions calculations support;
- True random number generator
- Internal HSI and RTC with external oscillator option

**I/O protection features**:

- ESD protection (persistent against electrostatic discharge)
- All interfaces are 5V-tolerant
- Reverse polarity signal protection
- Overcurrent protection

**User interaction:**

- **3** programmable custom **user buttons** (one can be used as reset button)
- **1.3" OLED Display** for user interface

------

## 📏 Mechanical data

- **Size dimensions:** 22.5x57x12 mm
- Weight: <15 gramms

------

## 🔥 Operating conditions

- **Working temperature range:** **-25 to +80** degrees Celsius
- **Environment humidity range:** 0 to 90%
- **Environmental safety:** **Lead-Free** and **RoHS** compliance
- **Maximum heat dissipation**: 1.9W

------

## 📝 TODO

- WiFi for wireless access
- 1Gbyte memory
- Dual direction power mosfet
- Programmable logic level
- JTAG pogo
