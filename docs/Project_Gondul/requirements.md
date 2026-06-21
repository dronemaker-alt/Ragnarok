# Project Göndul - Initial Requirements

## Primary mission

Build a large folding UAV that can serve as an airborne command node, communications relay, and experimental Drone Libre test platform.

## Core requirements

### Airframe

- Use the rare Phanvick folding Phantom conversion frame as the initial physical platform.
- Preserve the original shell as a reference and possible mold master.
- Support future fiberglass or carbon-fiber duplicate shells.
- Maintain access panels or removable sections for avionics service.
- Keep payload modules removable and replaceable.

### Flight control

- First flying version should use accessible, known-good hardware.
- Preferred first configuration: Phantom 1 / NAZA-based architecture.
- Experimental payloads must not be required for safe manual flight.
- The aircraft should be able to fly as a normal quad before add-ons are installed.

### Power

- Separate flight-critical power from experimental payload power where practical.
- Use fused or otherwise protected payload branches.
- Log battery voltage during test flights.
- Record current draw for each add-on module.

### Communications

Candidate payload functions:

- Ground relay
- Scout-drone status relay
- Drone-to-drone messaging experiments
- Remote ID experimentation
- ADS-B receive node
- Mesh-network experiments
- Secure line-of-sight optical/laser communication experiments in later phases

### Software / companion systems

Candidate systems:

- ESP32
- ESP32-S3
- Raspberry Pi Zero 2W
- LilyGo P4 / P4 Pro
- H743 / ArduPilot in later variant

### Documentation

Every hardware change should be documented with:

- Date
- Version / configuration name
- Parts changed
- Wiring changes
- Power source
- Test result
- Failure notes
- Photos when possible

## Non-goals for early phases

- Do not start by modifying DJI firmware.
- Do not depend on the experimental payload for flight stability.
- Do not install all payload concepts at once.
- Do not cut the original Phanvick shell until it has been measured, photographed, and evaluated as a mold master.

## Success criteria

### Phase 1 success

- Aircraft powers up cleanly.
- NAZA or selected flight controller initializes normally.
- Motors arm correctly.
- Controls respond correctly.
- Compass/GPS placement is acceptable.
- Aircraft hovers safely without experimental payload.

### Phase 2 success

- Passive data payload operates independently.
- Payload does not interfere with flight controller.
- Logs are recoverable after flight.
- Battery and CG effects are recorded.

### Phase 3 success

- Airborne relay payload communicates with ground node.
- Communications payload can reboot without affecting flight.
- Relay performance is logged.

### Phase 4 success

- Göndul can coordinate or monitor at least one scout aircraft.
- Scout telemetry/status is visible at the ground station.
- Logs show useful command-node behavior.
