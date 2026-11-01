Boot Process — ThinkPad T470 Research

1. Purpose

This document describes the general computer boot process and the firmware initialization stages used by coreboot.

The objective is to understand how hardware initialization takes place before control is transferred to the bootloader or another payload.

This is a general technical overview. It does not describe a validated Coreboot implementation for the Lenovo ThinkPad T470.

2. General Boot Process

When a computer is powered on, the processor begins executing firmware instructions.

The firmware initializes the hardware and prepares the system to load the next stage of the boot process.

In a traditional UEFI-based system, firmware performs hardware initialization and eventually starts a boot manager, which loads an operating system bootloader.

Coreboot follows a different architecture: it performs the necessary hardware initialization and then transfers control to a separate program called a payload.

3. Coreboot Boot Stages

3.1 Bootblock

The bootblock is the first Coreboot stage executed after the CPU reset.

Its main responsibilities include:

Preparing the initial execution environment.
Setting up the stack.
Initializing Cache-as-RAM (CAR).
Performing early CPU initialization.
Loading the next firmware stage.

3.2 Verstage (Optional)

The verstage is used by verified boot implementations.

Its purpose is to establish a chain of trust and verify firmware components before they are executed.

Not every Coreboot configuration uses this stage.

3.3 Romstage

The romstage performs early hardware initialization.

Its main responsibility is initializing system memory (DRAM), allowing later stages to use regular RAM.

3.4 Postcar

The postcar stage handles the transition from Cache-as-RAM to regular DRAM.

It prepares the environment needed to execute the ramstage.

3.5 Ramstage

The ramstage performs most of the platform’s hardware initialization.

Typical responsibilities include:

PCI device initialization.
On-chip device initialization.
CPU configuration.
Optional graphics initialization.
ACPI and SMBIOS table generation.
Preparing the system for the payload.

3.6 Payload

The payload is the software executed after Coreboot finishes its hardware initialization.

Examples include:

SeaBIOS.
edk2.
GRUB2.

The payload provides the functionality needed to continue the boot process and load an operating system.

4. Simplified Boot Flow

Power on - > CPU Reset - > Bootblock - > Verstage (optional) - > Romstage - > Postcar - > Ramstage - > Payload - > Operating System Bootloader / OS

5. Important Concepts

Cache-as-RAM (CAR)

CAR allows early firmware stages to use the CPU cache as temporary memory before DRAM has been initialized.

DRAM Initialization

DRAM initialization is a critical step because later firmware stages require regular system memory.

Payload

A payload is a separate program that receives control after Coreboot completes hardware initialization.

ACPI

ACPI provides standardized information and interfaces that operating systems use to interact with platform hardware and power-management features.

6. Relevance to ThinkPad T470 Research

Understanding the Coreboot boot process is necessary before investigating a potential T470 implementation.

Further research is required to determine:

Which initialization stages are required by the T470 platform.
How the T470 hardware differs from supported Coreboot platforms.
Which platform-specific components and firmware dependencies are involved.
Whether existing implementations provide useful reference material.

No compatibility or working implementation is assumed.

7. References

https://doc.coreboot.org/getting_started/architecture.html
https://doc.coreboot.org/getting_started/
https://doc.coreboot.org/payloads.html
https://doc.coreboot.org/lib/ramstage_bootstates.html
