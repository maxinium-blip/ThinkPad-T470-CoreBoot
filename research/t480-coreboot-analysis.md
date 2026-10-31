ThinkPad T480 — Coreboot Analysis

1. Purpose

This document investigates the existing Coreboot implementation for the Lenovo ThinkPad T480.

The T480 will serve as the initial reference platform for studying whether parts of its firmware implementation could be relevant to the Lenovo ThinkPad T470.

No compatibility between these models is assumed.

2. Research Objectives

Identify the T480 motherboard and platform configuration.
Locate its official Coreboot board configuration.
Study the source code and build configuration.
Understand its hardware initialization requirements.
Identify components that may differ from the T470.
Document potential obstacles to reusing or adapting existing code.

3. Coreboot Implementation

Research status: Not yet analyzed.

Official board configuration:
Mainboard directory:
Supported processor platforms:
Chipset:
Embedded Controller (EC):
Firmware requirements:

4. Hardware Architecture

The following components require investigation:

CPU and platform architecture
Chipset and system management
Embedded Controller (EC)
GPIO configuration
SPI flash and firmware layout
Intel Management Engine (ME)
Boot process and hardware initialization

5. Source Code Analysis

Relevant source-code files and configuration details will be recorded here.

File or component	Purpose	Findings
Mainboard configuration	To investigate	Pending
Kconfig	To investigate	Pending
Devicetree	To investigate	Pending
GPIO configuration	To investigate	Pending
EC implementation	To investigate	Pending

6. Relevance to the T470

The T480 implementation is being studied as a reference.

Potentially reusable components must be evaluated individually. Differences in motherboard design, chipset, EC, GPIO and firmware configuration may require substantial changes.

No reusable code has been confirmed yet.

7. Sources

Official sources will be added as each technical claim is verified.

Coreboot documentation
Coreboot source code
Coreboot supported mainboards

8. Findings and Research Log

Current status: Initial document created. Technical analysis pending.

Verified findings, unresolved questions and unsuccessful investigations will be documented here.

Last updated: 2026-10-31
