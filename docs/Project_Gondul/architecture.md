# Project Göndul - System Architecture

## Architecture principle

Göndul should be built as two mostly independent systems sharing an airframe:

1. **Flight-critical aircraft system**
2. **Experimental payload / command-node system**

The experimental system may observe and report, but it should not be able to take the aircraft down during early phases.

## Layered layout concept

### Bottom layer

- Main flight battery
- Battery retention
- Possible current sensor
- CG adjustment area

### Middle layer

- Flight controller
- Power distribution
- ESC wiring
- Receiver
- PMU / BEC hardware
- Flight-critical wiring

### Top layer

- Payload bay
- ESP32 / Pi / LilyGo modules
- Radio payloads
- Data logger
- Remote ID node
- ADS-B receiver
- Antenna mounts

## Flight-control candidate stack

### Göndul-A: NAZA / Phantom 1

Purpose: first flying proof of concept and easiest wiring/debug path.

Expected strengths:

- Accessible wiring
- Known behavior
- Easy bench testing
- Reduced modern DJI integration issues

Expected limitations:

- Old ecosystem
- Limited native telemetry
- Limited autonomous capability compared with ArduPilot

### Göndul-B: Phantom 3 electronics

Purpose: compare more integrated DJI architecture in the same general airframe style.

Expected strengths:

- More authentic to the Phanvick conversion era
- Better camera/gimbal integration if retained

Expected limitations:

- More integrated system
- More dependency on DJI ecosystem
- Harder to instrument cleanly

### Göndul-C: H743 / ArduPilot

Purpose: open experimental control stack.

Expected strengths:

- Strong autonomy support
- Better telemetry flexibility
- Easier integration with companion systems

Expected limitations:

- Requires full configuration and tuning
- More setup risk than known Phantom hardware

### Göndul-D: Drone Libre flight controller

Purpose: future domestic/open replacement avionics platform.

Expected strengths:

- Maximum control
- Project-owned architecture
- Best long-term alignment with Drone Libre

Expected limitations:

- Not an early-phase deliverable
- Requires hardware validation first

## Payload architecture

### Passive payloads first

Early payloads should only listen, log, or transmit their own status.

Examples:

- Voltage logger
- Temperature logger
- Vibration logger
- GPS mirror logger
- OLED status display

### Relay payloads second

Once the airframe is stable, add communications payloads.

Examples:

- ESP32 telemetry relay
- LoRa / ELRS experiment
- nRF24L01 experiment
- Wi-Fi diagnostic bridge
- Remote ID node

### Command-node payloads third

Once relay behavior works, add coordination features.

Examples:

- Scout status dashboard
- ADS-B receiver
- LilyGo P4 display
- Ground-station messaging
- Mission event logger

## Electrical separation guideline

Where practical:

- Flight controller and receiver get their own stable power path.
- Payload electronics get a separate regulated and fused power branch.
- Payload ground should be planned deliberately to reduce noise and ground-loop weirdness.
- High-current motor wiring should be kept physically separate from RF and sensor wiring.
- Antennas should be separated as much as the shell allows.

## Failure philosophy

A payload failure should create a line in the log, not a smoking hole in the grass.

Acceptable early failure:

- Payload reboot
- Lost payload telemetry
- Bad data log
- Frozen display

Unacceptable early failure:

- Flight controller reset caused by payload
- Receiver brownout caused by payload
- Motor desync caused by payload wiring/noise
- GPS/compass corruption from poor payload placement

## Ground segment concept

Göndul should eventually connect to a ground station made from existing Drone Libre hardware:

- LilyGo P4 / P4 Pro handheld
- ESP32 bridge modules
- Laptop/tablet when needed
- SDR/ADS-B receiver chain
- Future controller backpack modules

## Scout aircraft concept

Scout aircraft can include:

- DJI Mini / Mini 2 repair birds
- Drone Libre test frames
- Future small H743/ArduPilot quads

Göndul's job is not to replace the scout. Göndul's job is to watch, relay, log, and coordinate while the scout does the risky little-drone work.
