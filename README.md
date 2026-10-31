ThinkPad T470 Coreboot Research

An independent research project exploring the possibility of bringing native Coreboot support to the Lenovo ThinkPad T470, while also investigating its potential integration into Libreboot.

The goal is to understand the hardware, study existing firmware implementations, document technical requirements and determine whether supporting this laptop is realistically possible.

Project Overview

Property	Details
Platform	Intel Kaby Lake
Reference device	Lenovo ThinkPad T470
Processor	Intel Core i7-7600U
Graphics	Intel HD Graphics 620
Memory	16 GB RAM
Repository license	GPL-3.0
Project status	Research only

Current Status: Initial Research 

No working T470 firmware port has been developed or validated by this project.

No firmware images are provided.

Do not flash experimental firmware based solely on information in this repository.

This project started with a simple question:

What would it take to bring open-source firmware support to the Lenovo ThinkPad T470?

The T470 is the main focus of this research. I want to understand its hardware architecture, firmware components and differences from other ThinkPad models, especially models that already have Coreboot or Libreboot support.

Rather than assuming that an existing implementation can be adapted, I intend to investigate the technical requirements and document what is known, what remains uncertain and what would need further work.

This is an independent learning and research project.

Project Maintainer and Workflow

This project is currently maintained independently. I carry out the research, organize the documentation and manage the repository myself.

I use Linux as my main working environment and GitHub to document findings, track progress and share research.

I am still learning about firmware development, hardware initialization and low-level system architecture. This project is also an opportunity to develop those skills through practical research.

I work using a combination of my own investigation, technical documentation, source-code analysis and AI-assisted tools.

AI-Assisted Research and Verification

AI tools may be used as assistants for research and learning. They can help explain unfamiliar concepts, understand technical documentation, explore source code and suggest possible directions for investigation.

However, AI-generated information is never automatically considered correct or treated as a definitive technical source.

I personally review and verify technical claims before publishing them. Whenever possible, I will include links to the original documentation, source code, hardware specifications and other reliable references used during the research.

Findings should be supported by evidence and, where applicable, independently verifiable through documentation, source-code analysis or reproducible tests.

The purpose is to keep the research transparent and make it possible for other people to review the information and reach their own conclusions.

Hardware Reference

The main reference machine for this project is:

* Model: Lenovo ThinkPad T470
* Processor: Intel Core i7-7600U
* Platform: Intel Kaby Lake
* Integrated graphics: Intel HD Graphics 620
* Memory: 16 GB RAM

Additional hardware details, including the exact motherboard revision, embedded controller (EC) and firmware configuration, will be documented as they are identified and verified.

Research Areas

1. Hardware Investigation

* Identify the motherboard and hardware configuration.
* Study the platform architecture.
* Investigate the embedded controller (EC).
* Identify relevant firmware components.
* Document hardware differences between T470 configurations.

2. Existing Firmware Projects

* Study the Coreboot source code and documentation.
* Investigate existing Lenovo ThinkPad implementations.
* Look for documented community experiments involving the T470.
* Compare the T470 with related models, including the T470s and T480.
* Identify potentially reusable code and platform-specific requirements.

3. Firmware Architecture

* Understand the structure of the original firmware.
* Study Intel Management Engine and platform initialization.
* Investigate the boot process and hardware initialization requirements.
* Document proprietary components and technical limitations.

4. Development Research

If the research identifies a technically viable path, I will investigate what would be required to develop a T470-specific Coreboot implementation.

Any experimental development will be documented separately from verified results.

5. Compatibility and Validation

Hardware compatibility must be evaluated component by component.

A successful boot alone will not be considered proof of complete hardware support. Findings and limitations should be documented clearly.

Working Principles

* Prefer verified information over assumptions.
* Use original documentation and source code whenever possible.
* Include references for technical claims.
* Document unsuccessful investigations as well as successful findings.
* Keep research organized and reproducible.
* Avoid duplicating existing community work.
* Clearly distinguish confirmed facts from hypotheses.
* Prioritize hardware safety and recovery considerations.

Repository Structure

The repository is organized into the following sections:

ThinkPad-T470-CoreBoot/
├── README.md
├── LICENSE
├── docs/
│   ├── hardware-overview.md
│   ├── motherboard.md
│   └── boot-process.md
├── research/
│   ├── t470-vs-t470s.md
│   ├── t470-vs-t480.md
│   ├── coreboot-analysis.md
│   └── libreboot-analysis.md
├── references/
│   └── sources.md
└── reports/
    └── research-log.md

These files will be added progressively as the research develops. The structure represents the planned organization, not completed research.

Contributions

Although this project is currently maintained independently, contributions and technical feedback are welcome.

Useful contributions may include:

* Verified hardware information about the ThinkPad T470.
* References to existing T470 firmware experiments.
* Technical documentation and specifications.
* Coreboot or Libreboot source-code analysis.
* Information about related ThinkPad platforms.
* Reviews, corrections and suggestions supported by reliable sources.

Please include references or supporting evidence whenever possible.

Firmware Blobs and Proprietary Components

This project does not intend to redistribute proprietary firmware, Intel Management Engine firmware or Lenovo firmware images.

Any investigation involving proprietary components will respect their applicable licenses and distribution restrictions.

The origin, requirements and handling of any necessary firmware components will be documented as the research progresses.

Licensing and Third-Party Work

This repository uses the GNU General Public License v3.0 (GPL-3.0) for original material that I publish and have the right to license under those terms.

Coreboot and Libreboot are separate projects with their own licensing policies. Their licenses are not changed by this repository.

Before reusing or modifying third-party code, its individual license, copyright notices and compatibility with the intended use must be checked. Original licenses and attribution notices must be preserved where required.

Useful references:

* Coreboot source repository
* Libreboot documentation
* GNU GPL FAQ

Disclaimer

This repository is intended for research, learning and documentation.

It does not provide a working firmware port or instructions for installing experimental firmware on the ThinkPad T470.

Firmware development and testing involve hardware-specific risks. No experimental firmware should be installed based solely on information in this repository.

⸻

The objective is to investigate, understand and document what would be required to bring open-source firmware support to the ThinkPad T470, one verified step at a time.
