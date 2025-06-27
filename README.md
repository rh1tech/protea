# Protea

Protea is a custom development board designed in KiCad that bridges the gap between vintage computing and modern connectivity. Named after the protea flower, which itself derives from Proteus, son of Poseidon in Greek mythology, this board embodies the shape-shifting adaptability that made the mythological Proteus legendary. Just as the protea flower has survived and adapted for over 300 million years, becoming a symbol of longevity and endurance, the Protea development board is designed to endure and adapt across different technological eras.

The protea’s incredible diversity of forms - which inspired Carl Linnaeus to name it after the shape-shifting Proteus - mirrors this board’s versatility in connecting vintage computing with modern internet capabilities.

Documentation: [rh1.tech](https://rh1.tech/projects/protea)

## Hardware Specifications

### Primary Controller:

- RP2040 Microcontroller - directly soldered on board
- Dual-core ARM Cortex-M0+ processor running up to 133 MHz
- 264kB on-chip SRAM for program execution
- 8 Programmable I/O (PIO) state machines for custom peripheral support

### Connectivity Controller:
- ESP8266 Microcontroller - integrated Wi-Fi-to-Serial modem functionality
- 802.11 Wi-Fi support for internet connectivity
- AT command compatibility for seamless vintage computer integration

### Interface Ports:

- USB Port - keyboard input support with hub compatibility
- DB9 Serial Port - RS232 connectivity for vintage computers and external devices
- HDMI Port - native digital video output without conversion
- Power Input - USB-powered operation

## Firmware Ecosystem

Protea operates using two complementary firmware components:

### [Iris](https://github.com/rh1tech/iris) Terminal Software

- VT100/VT102 terminal emulation with full attribute support
- Instant-on operation with no boot time
- Configurable fonts and display settings
- PETSCII mode for Commodore compatibility

### [Hermes](https://github.com/rh1tech/hermes) Wi-Fi Modem

- Hayes-compatible AT command set
- Telnet protocol support for internet connectivity
- Transparent Wi-Fi-to-Serial bridge operation
- BBS and vintage online service access

## Use Cases

Protea enables seamless connection of classic computers to modern internet resources, providing access to text-mode BBS systems and online communities that maintain the spirit of early computing culture. The board serves as a bridge between RS232 devices and Wi-Fi networks, ensuring that vintage computing enthusiasts can maintain an authentic retro computing experience while leveraging contemporary internet connectivity.

The platform supports text-mode internet browsing for those who prefer minimalist computing approaches, while also serving as a foundation for terminal-based development environments. Protea is particularly well-suited for retrocomputing projects that require modern connectivity solutions, and functions as an educational platform for understanding the fundamentals of serial communications and terminal operations.

## Design Philosophy

Like the protea flower that has endured and adapted for over 300 million years, and the shape-shifting Proteus of Greek mythology, this development board embodies longevity, adaptability, and transformation. The board’s dual-microcontroller architecture ensures optimal performance for both local terminal processing and network communications, demonstrating the same versatility that characterizes its mythological and botanical namesakes.

The custom PCB design prioritizes signal integrity and reliable connectivity, making it suitable for both hobbyist projects and professional applications requiring robust serial terminal functionality.

## Getting Started

1.	Flash Firmware - Load [Iris](https://github.com/rh1tech/iris) onto the RP2040 and [Hermes](https://github.com/rh1tech/hermes) onto the ESP8266
2.	Connect Display - Attach HDMI monitor for terminal output
3.	Add Keyboard - Connect USB keyboard for input
4.	Configure Wi-Fi - Set up wireless connectivity through Hermes
5.	Connect Devices - Use DB9 port for vintage computer or RS232 device connections
