# Ragnarok

Class work and beginnings of my drone, avionics, electronics, and embedded systems projects.

This repository is organized as a working project vault: hardware notes, firmware experiments, CAD/3D-print files, software tools, project logs, and reference material can live together without stepping on each other.

## Repository map

```text
Ragnarok/
├── assets/              # Images, diagrams, screenshots, and media used by docs
├── cad/                 # 3D models, printable parts, drawings, and mechanical layouts
├── data/                # Captured logs, test data, calibration data, and sample files
├── docs/                # Project notes, build guides, design decisions, and references
├── firmware/            # Microcontroller firmware projects and sketches
├── hardware/            # Wiring, schematics, BOMs, pinouts, and electronics notes
├── inventory/           # Parts inventory, module lists, and project-specific materials
├── project_logs/        # Build logs, test notes, issue notes, and dated progress
├── software/            # Host-side software, utilities, scripts, and UI experiments
├── tests/               # Test plans, bench checks, validation notes, and fixtures
└── tools/               # Helper utilities, setup scripts, and maintenance tools
```

## Working rules

- Keep mirrored repositories separate; do not copy or modify mirrored code here unless intentionally vendored.
- Put early experiments in `firmware/experiments/` or `software/experiments/` before promoting them into project folders.
- Use dated notes in `project_logs/` when testing hardware or changing wiring.
- Store project-specific wiring and pinouts in `hardware/` before writing firmware against them.

## Current status

Initial structure created for active hardware, firmware, drone, and electronics projects.
