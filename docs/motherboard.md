ThinkPad T470 — Motherboard Research

1. Purpose

This document collects information about the motherboard used in the Lenovo ThinkPad T470.

The objective is to identify its hardware architecture and understand the components relevant to firmware development and a potential Coreboot port.

This document is part of an ongoing research project. Unverified information is explicitly marked as such.

2. Motherboard Identification

Component	Information
Laptop model	Lenovo ThinkPad T470
Machine type	To be verified
Motherboard model	To be identified
Motherboard revision	Unknown
Platform	Intel Kaby Lake
CPU	Intel Core i7-7600U

3. Relevant Hardware Components

The following components require investigation:

CPU: Intel Core i7-7600U.
Chipset / PCH: Exact platform controller identification pending.
Embedded Controller (EC): Model and firmware version unknown.
SPI flash: Chip model and capacity unknown.
Intel Management Engine (ME): Firmware configuration requires investigation.
RAM: Current detected configuration is 16 GB; original factory configuration unknown.

4. Firmware-Related Components

BIOS / UEFI

The original Lenovo firmware initializes the hardware and provides the platform’s boot environment.

Embedded Controller (EC)

The EC is a dedicated controller responsible for functions such as keyboard input and power management.

Its exact implementation on this motherboard remains to be identified.

SPI Flash

The SPI flash stores platform firmware components. Its exact chip model, capacity and layout have not yet been verified.

Intel Management Engine (ME)

The Intel ME is a platform firmware component that must be considered when studying the original firmware architecture.

5. Information to Verify

Exact machine type and motherboard identification.
Motherboard revision.
Platform controller / PCH model.
Embedded Controller model and firmware version.
SPI flash chip model and capacity.
Original factory RAM configuration.
Available official hardware documentation.

6. Research Notes

This document is preliminary.

No motherboard compatibility with Coreboot is assumed or established at this stage. Information will be updated as reliable documentation and verifiable hardware data become available.

7. References

Lenovo ThinkPad T470 Hardware Maintenance Manual.
Lenovo ThinkPad T470 User Guide.
Official Coreboot documentation.
