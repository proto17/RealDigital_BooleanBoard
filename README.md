# RealDigital_BooleanBoard
Board configuration files for Vivado 2021.2 for the RealDigital Boolean FPGA development board


This repo contains board files for the RealDigital Boolean FPGA board (https://www.realdigital.org/hardware/boolean).  They have been tested with Vivado 2021.2, but no bitfile has been loaded onto a device.

Most of these files are based off of Digilent Inc. and Xilinx board files from the Xilinx board store (https://github.com/Xilinx/XilinxBoardStore/)

Currently there are no entries for the following:
- Bluetooth (there are no Vivado blocks for UARTs with CTS/RTS lines)
- Servo (there are no Vivado blocks that support PWM)
- Audio Out (there are no Vivado blocks that support PWM)
- Potentiometer (haven't gotten around to it)
