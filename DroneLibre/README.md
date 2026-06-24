# Drone Libre Archive

This directory is the working archive for DJI reverse-engineering references, repair workflow notes, depot records, board photos, and replacement-hardware experiments.

## Purpose

The goal is not just to collect files. The goal is to build a usable avionics-style maintenance and engineering record for small DJI aircraft, especially the Mavic Mini / Mini 2 family, while keeping source attribution clear.

## Structure

```text
DroneLibre/
├── Upstream_Archive/
│   └── o-gs_dji_hardware_schematics/
├── Reference_Library/
│   ├── DJI_Manuals/
│   ├── FCC_Filings/
│   ├── Teardowns/
│   └── External_Links/
├── Mini_Depot/
│   ├── Intake_Records/
│   ├── Electrical_Troubleshooting/
│   ├── Gimbal_Repair/
│   ├── Corrosion_Recovery/
│   ├── Motor_ESC_Checks/
│   └── Flight_Test_Records/
├── Board_Photos/
│   ├── Mini/
│   ├── Mini_2/
│   ├── Phantom_2/
│   └── Controllers/
├── Connector_Library/
├── Failure_Library/
├── Battery_Research/
├── Backpack_Interface/
└── Replacement_Hardware/
```

## Archive Rules

1. Keep upstream material separate from original Drone Libre notes.
2. Preserve source URLs, access dates, and licenses when known.
3. Do not overwrite upstream files with modified versions.
4. Put personal measurements, repair findings, and photos in the depot folders.
5. Use one intake record per aircraft.
6. Treat every crashed drone like an aircraft maintenance record, not a random pile of parts.

## Current Priority

1. Mirror `o-gs/dji-hardware-schematics` locally and place a copy under `Upstream_Archive/o-gs_dji_hardware_schematics/`.
2. Build Mini / Mini 2 repair workflows.
3. Document connector pinouts and board photos.
4. Add failure records for each aircraft: CFIT, Davey Jones, Mini #2, and future repair candidates.
5. Use the archive to support a future Mini backpack interface board and replacement flight-controller project.
