ThinkPad T470 — Coreboot Compatibility Findings

1. Purpose

This document records research findings related to the potential compatibility of the Lenovo ThinkPad T470 with Coreboot.

Its purpose is to distinguish verified information from assumptions, open questions and unresolved technical challenges.

No working Coreboot implementation for the standard T470 is claimed.

2. Current Compatibility Status

Status: Under investigation

The standard Lenovo ThinkPad T470 is not listed among the models covered by the referenced official Coreboot documentation for Lenovo Skylake/Kaby Lake platforms.

The ThinkPad T470s is listed, but it is a different laptop model and must not be treated as equivalent to the standard T470.

3. Verified Information

Area	Finding
Laptop model	Lenovo ThinkPad T470
CPU	Intel Core i7-7600U
CPU generation	Intel Kaby Lake
Graphics	Intel HD Graphics 620
Official Coreboot documentation	T470s is listed; standard T470 is not
T480 support	Documented in the official Coreboot project
T470 native port	Not established by this research

4. Areas Requiring Further Investigation

4.1 Motherboard Identification

The exact motherboard model and revision must be identified.

4.2 Embedded Controller

The EC model, firmware version and communication interfaces remain to be investigated.

4.3 Memory Initialization

The memory initialization requirements of the T470 must be understood independently.

4.4 Intel Firmware Dependencies

The platform’s Intel firmware components and their requirements need further research.

4.5 Hardware Configuration

GPIO, PCI devices, chipset configuration and other platform-specific details must be documented.

4.6 Boot Process

The original T470 firmware boot process should be studied to understand its initialization sequence.

5. Compatibility Assessment

At the current stage, there is insufficient evidence to determine whether a native Coreboot port for the standard T470 is technically feasible.

The T480 implementation provides useful research material, but its board-specific configuration cannot be assumed to work on the T470.

Further hardware identification, source-code analysis and platform comparison are necessary.

6. Known Limitations

No native T470 implementation has been developed.
No experimental firmware has been validated.
The exact motherboard configuration has not yet been established.
Hardware-level compatibility remains unknown.
No firmware flashing or modification has been performed as part of this research.

7. Next Research Steps

1. Identify the exact T470 motherboard.
2. Investigate the Embedded Controller.
3. Study the T480 mainboard implementation.
4. Compare relevant platform configuration files.
5. Collect reliable technical documentation.
6. Update this assessment as new evidence becomes available.

8. Conclusion

The Lenovo ThinkPad T470 remains an unexplored target in this research project.

Existing Coreboot support for related Lenovo models provides a starting point for investigation, but it does not establish compatibility with the standard T470.

All conclusions will be updated as verified information becomes available.

9. References

https://doc.coreboot.org/mainboard/lenovo/skylake.html
https://github.com/coreboot/coreboot
https://doc.coreboot.org/mainboard/
