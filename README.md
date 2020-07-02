# Note
This board is still under test, we will be updating system operational status as tests are completed.

# BFC
The BeaverCube Flight Computer, or CASTOR Pi Board, is an open-source flight computer for CubeSats. Designed for the MIT BeaverCube CubeSat mission, the board supports an imaging payload with 3 cameras over USB as well as subsystem boards over UART, I2C and SPI buses. 

CASTOR Pi Board: CubeSat Atmospheric and Sea-surface Temperature Optical Observation Raspberry Pi Board

# Known Issues, Testing Progress
The BFC rev 1.0 is currently being tested, with rev 2.0 expected to be manufactured and testing started by the end of August 2020. The power system has been characterized under expected loads and is fully operational with no errors detected. The RPI recovery system (see schematic Sheet 3) that controls which RPI is running and SD card is selected has been fully tested, and no errors detected.

The USB hub is currently under test to verify all ports can communicate with the compute module. Additional tests to be completed by mid-July 2020 include running flight software to verify all onboard devices (RTC, IMUs) function nominally, and interfacing the BFC with devices to test external connections including RS-485, TTL UART, I2C, SPI.

Known errors on rev 1.0 that will be fixed in rev 2.0
- SD card MUXs U4, U11, U13, U14 have incorrect footprints. The compute module cannot access the SD card slots.
- The USB line is routed to the incorrect GPIO pin on the compute module. A temporary fix was made to continue testing.

# project
Eagle CAD Project, Board, Schematic files.

# libraries
Ealgle CAD Library files.


