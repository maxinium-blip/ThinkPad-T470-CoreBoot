ThinkPad T480 to T470 — Adaptation Research

1. Purpose

This document investigates the technical differences between the Lenovo ThinkPad T480 and T470 in the context of Coreboot development.

The objective is to understand which parts of the T480 implementation could provide useful reference material for a potential T470 port.

No direct compatibility or successful adaptation is assumed.

2. Reference Platforms

ThinkPad T480

Platform: Intel Kaby Lake Refresh.
Coreboot: Documented in the official Coreboot project.
Architecture: Intel x86-64.
Firmware implementation: Available in the official Coreboot source tree.

ThinkPad T470

Platform: Intel Kaby Lake.
Coreboot: No confirmed official support identified for the standard T470 model.
Architecture: Intel x86-64.
Firmware implementation: Original Lenovo firmware.

3. Areas Requiring Comparison

The following components and subsystems must be investigated before determining whether any code can be reused.

3.1 CPU and Platform Architecture

Both systems belong to the Intel Kaby Lake family or its related generation.

However, sharing a processor architecture does not guarantee firmware compatibility.

Differences in platform configuration and hardware initialization must be considered.

3.2 Motherboard

The motherboard layout and component configuration must be examined independently.

Important information includes:

Motherboard model and revision.
Platform Controller Hub (PCH).
Hardware device configuration.
GPIO configuration.
PCI device layout.

3.3 Embedded Controller (EC)

The Embedded Controller handles platform-specific functions such as keyboard input and power management.

Its firmware and communication interfaces must be investigated separately for each model.

3.4 Memory Initialization

Memory initialization is platform-dependent.

The configuration used by the T480 cannot be assumed to work on the T470.

3.5 Firmware Configuration

Coreboot board configurations contain platform-specific information.

Relevant areas include:

Kconfig configuration.
Devicetree.
Mainboard initialization.
GPIO configuration.
Firmware dependencies.

3.6 Intel Firmware Components

Both platforms require investigation of their Intel firmware dependencies.

The exact requirements and versions must be verified independently.

4. Potentially Reusable Research Material

The T480 implementation can be used as a reference for studying:

Coreboot source code organization.
Mainboard implementation structure.
Kconfig options.
Devicetree configuration.
Hardware initialization concepts.
Documentation and development workflow.

This does not establish that T480-specific code is compatible with the T470.

5. Main Technical Challenges

Potential challenges include:

Differences in motherboard design.
Platform-specific hardware initialization.
Embedded Controller integration.
Memory initialization requirements.
GPIO and device configuration differences.
Firmware dependency differences.
Hardware validation and recovery requirements.

These are research areas, not confirmed incompatibilities.

6. Research Methodology

The investigation will follow these principles:

1. Study the official T480 Coreboot implementation.
2. Identify the hardware and firmware components involved.
3. Collect reliable documentation about the T470.
4. Compare both platforms using verified information.
5. Document similarities, differences and unknowns.
6. Evaluate potential compatibility only after sufficient evidence is available.

All investigation at this stage is read-only.

7. Current Findings

The T480 has an official documented Coreboot implementation.
The standard T470 is not listed alongside the supported models in the referenced Coreboot documentation.
Both systems are related to the Intel Kaby Lake platform generation.
Hardware and firmware differences must be investigated before considering code reuse.
No T470 port or adaptation has been developed or validated.

8. References

https://doc.coreboot.org/mainboard/lenovo/skylake.html
https://github.com/coreboot/coreboot
https://doc.coreboot.org/internals/devicetree.html
https://doc.coreboot.org/getting_started/kconfig.html

9. Research Log

Further findings, comparisons and verified technical information will be added as the investigation progresses.
