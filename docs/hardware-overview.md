ThinkPad T470 – Hardware Overview

1. Purpose

This document provides an overview of the hardware found in the Lenovo ThinkPad T470.

The goal is to identify the main hardware components and understand their roles in the system. This information will serve as a reference for the Coreboot compatibility research.

2. System Information

Component	Information
Manufacturer	Lenovo
Model	ThinkPad T470
CPU	Intel Core i7-7600U
CPU Generation	7th Generation Intel Core
CPU Architecture	Kaby Lake
Integrated Graphics	Intel HD Graphics 620
RAM	16 GB (currently detected; original configuration unknown)
Storage	SSD

3. Main Hardware Components

3.1 Processor (CPU)

The system uses an Intel Core i7-7600U processor, based on the Kaby Lake microarchitecture.

The processor is responsible for executing instructions and coordinating system operations.

Further research is needed to understand its firmware initialization requirements.

3.2 Integrated Graphics

The processor includes Intel HD Graphics 620.

Its initialization and compatibility requirements will need to be investigated during the firmware research.

3.3 Memory (RAM)

The laptop currently has 16 GB of RAM.

The exact memory configuration and motherboard specifications still need to be verified.

3.4 Storage

The system uses an SSD for storage.

Storage configuration is documented for hardware identification purposes and is not a primary focus of the Coreboot investigation.

4. Firmware-Related Components

The following components are important areas of investigation:

BIOS/UEFI: Existing system firmware and its responsibilities.
Embedded Controller (EC): Controller responsible for various laptop-specific functions.
SPI Flash: Non-volatile memory used to store firmware components.
Intel Management Engine (ME): Intel platform management subsystem.
Chipset / Platform Controller: Platform hardware responsible for connecting and managing system devices.

The exact components, revisions and configurations of this particular T470 motherboard have not yet been verified.

5. Information Still to Verify

Exact motherboard model and revision.
Exact machine type.
Embedded Controller model and firmware version.
Chipset identification.
SPI flash configuration.
Existing BIOS/UEFI version.
Available hardware documentation.
Original factory RAM configuration.
Whether the RAM was upgraded after purchase.
Current RAM module configuration.

7. Research Notes

This document is a preliminary hardware overview.

Information will be updated as reliable documentation and hardware identification results become available.

No Coreboot compatibility or support is assumed at this stage.
