# RealDigital_BooleanBoard
Board configuration files for Vivado 2021.2 for the RealDigital Boolean FPGA development board


This repo contains board files for the RealDigital Boolean FPGA board (https://www.realdigital.org/hardware/boolean).  They have been tested with Vivado 2021.2, but no bitfile has been loaded onto a device.

Most of these files are based off of Digilent Inc. and Xilinx board files from the Xilinx board store (https://github.com/Xilinx/XilinxBoardStore/)

Currently there are no entries for the following:
- Bluetooth (there are no Vivado blocks for UARTs with CTS/RTS lines)
- Servo (there are no Vivado blocks that support PWM)
- Audio Out (there are no Vivado blocks that support PWM)
- Potentiometer (haven't gotten around to it)

Headers J1 and J2 contain the four PMOD ports, but also contain 12 GPIO pins (6 on each header).  These pins fall between the PMOD ports.  They have been numbered in the board files to match how the PMOD ports are numbered (circular numbering).

There is no "reset" port on this board, so when creating block designs the user will need to specify a reset port by hand.  If using one of the push buttons, be sure not to use the push button GPIO entry!
