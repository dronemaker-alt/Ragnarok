# Project Göndul

**Project name:** Göndul  
**Plain ASCII folder name:** `Project_Gondul`  
**Role:** Airborne command node / mother ship / swarm coordinator / Drone Libre test mule  
**Origin:** Phanvick folding Phantom-to-Mavic-style conversion frame with DJI Phantom donor hardware.

## Concept

Göndul is a large folding UAV platform intended to act as the queen-bee aircraft for the Drone Libre ecosystem. It is not meant to be a pretty shelf queen. It is meant to be a working avionics mule: large enough to carry experimental radios, companion computers, Remote ID hardware, ADS-B receive equipment, data logging, and eventually swarm coordination payloads.

The project starts with known DJI Phantom-era hardware and evolves toward a modular Drone Libre command aircraft.

## Mythology / naming note

Göndul is a named Valkyrie. The name fits the project because Valkyries observe, select, guide, and retrieve warriors from the battlefield. For this UAV, the role is similar in a very nerdy avionics sense: remain overhead, observe the swarm, relay communications, coordinate scouts, and help bring the little aircraft home.

Approximate radio-friendly pronunciation: **GURN-dool**.

## Available donor aircraft

- DJI Phantom 1
- DJI Phantom 2
- DJI Phantom 3

## Preferred starting donor

**Phantom 1 / NAZA-based hardware** is the preferred first donor because it is the most accessible and easiest to instrument:

- Separate NAZA flight controller
- Separate receiver path
- Separate GPS / compass module
- Conventional wiring
- Easier oscilloscope and multimeter troubleshooting
- Less modern DJI ecosystem lock-in

## Project phases

### Phase 0 - Preserve and document the original Phanvick parts

Goal: Capture the rare kit before modification.

Tasks:

- Photograph the Phanvick shell, arms, hinges, locks, motor mounts, and internal volume.
- Measure shell dimensions.
- Identify hardware sizes.
- Record missing, damaged, or fragile parts.
- Treat the original shell as a mold master candidate.

Deliverable: Baseline photo set and measurement sheet.

### Phase 1 - Basic airworthy conversion

Goal: Build a flying Phanvick/Phantom mule with no experimental payload.

Candidate configuration:

- Phanvick folding frame
- Phantom 1 / NAZA flight controller
- Phantom motors and ESCs as appropriate
- Standard receiver and transmitter path
- Standard GPS/compass placement
- Battery mounted for correct CG

Deliverable: Stable basic flight platform.

### Phase 2 - Göndul Mk I: data mule

Goal: Add passive instrumentation without disturbing the flight system.

Payload candidates:

- ESP32 data logger
- Independent power regulator
- Voltage/current logging
- Temperature logging
- Vibration logging
- OLED or small status display

Deliverable: Flight logs and power/performance baseline.

### Phase 3 - Göndul Mk II: comm relay

Goal: Add communication-node features.

Payload candidates:

- ESP32-S3 or Raspberry Pi Zero 2W
- LoRa / ELRS candidate link
- nRF24L01 experiments
- Wi-Fi diagnostic link
- Remote ID node
- Ground-station bridge

Deliverable: Working airborne relay experiments.

### Phase 4 - Göndul Mk III: swarm coordinator

Goal: Test multi-aircraft coordination concepts.

Payload candidates:

- LilyGo P4 or P4 Pro mission interface
- ADS-B SDR receive node
- Mesh radio bridge
- Drone-to-drone messaging
- Scout status dashboard
- Mission logging

Deliverable: Mother ship / scout aircraft demonstration.

## Variant naming

- **Göndul-A:** NAZA / Phantom 1 architecture
- **Göndul-B:** Phantom 3 electronics architecture
- **Göndul-C:** H743 / ArduPilot architecture
- **Göndul-D:** future Drone Libre flight controller architecture

## Companion aircraft naming candidates

- **Mist:** recon scout
- **Sigrún:** mapping/navigation scout
- **Hildr:** aggressive test platform
- **Brynhildr:** flagship/heavy variant

## Design rule

The flight-control system and the experimental payload system should be electrically and logically separated wherever practical. The aircraft should remain flyable even if the experimental payload locks up, reboots, or otherwise decides to become modern art.

## Immediate next actions

1. Photograph and measure the Phanvick shell and frame.
2. Inventory all three Phantom donors.
3. Identify which Phantom has the cleanest NAZA installation.
4. Bench-test the NAZA system before transplanting it.
5. Mock up the Phanvick internal layout with battery, NAZA, receiver, GPS, and power distribution.
6. Record center-of-gravity targets before adding companion hardware.
