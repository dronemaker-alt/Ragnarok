# Parts and References to Collect

This is the active hunt list for building the Drone Libre Mini / Mini 2 repair and reverse-engineering bench.

## Highest-Value Reference Material

### Public Documentation

- DJI Mini user manuals
- DJI Mini 2 user manuals
- DJI Mini SE user manuals
- DJI Mini 3 user manuals for architecture comparison
- Quick-start guides
- Battery safety guides
- Controller manuals
- Firmware release notes

### FCC / Regulatory Material

Collect FCC filings for:

- DJI Mavic Mini
- DJI Mini 2
- DJI Mini SE
- DJI Mini 3
- DJI RC-N1 controller
- DJI batteries if listed separately

Look especially for:

- Internal photos
- RF exposure reports
- Test reports
- Antenna location photos
- Block diagrams
- Operational descriptions

### Reverse-Engineering References

- O-GS DJI hardware schematics
- KiCad projects
- Board images
- Boardviews if found
- Connector pinouts
- Component ID lists
- Battery protocol notes
- UART / USB captures
- DJI Assistant logs and error-code notes

## Highest-Value Donor Parts

### Mini / Mini 2 Airframes

Good donor candidates:

- Account-bound but physically intact aircraft
- Broken gimbal but good power-up aircraft
- Broken arms with intact boards
- Water-damaged aircraft for component mapping, not immediate flight repair
- Update-failure aircraft that still power on

Avoid overpaying for:

- Saltwater aircraft unless cheap
- Missing gimbal/camera unless buying for boards
- Burned battery bay aircraft unless buying for mechanical parts

### Boards

Collect dead and working examples of:

- Mini ESC / power board
- Mini 2 ESC / power board
- Mini / Mini 2 core board
- GPS / compass board
- Gimbal board
- Camera module board
- Battery BMS board
- RC-N1 controller boards
- Phantom 2 center board
- Phantom 3 ESC center board
- Mavic Pro power / FC boards

Dead boards are still useful for:

- Component identification
- Connector measurements
- Trace routing
- Shield-can layout
- Donor connectors
- Failure comparison

## Mechanical Parts

Stockpile:

- Mini / Mini 2 arms
- Midframes
- Top shells
- Bottom shells
- Battery doors
- Gimbal dampers
- Gimbal mounting plates
- Yaw arms
- Camera ribbon cables
- Props
- Screws
- Motor screws
- Arm hinge hardware

## Motors

Collect and document:

- Mini motors
- Mini 2 motors
- Mini SE motors
- Known-good matched sets
- Dead motors for teardown

For each motor type, record:

```text
Part number:
Diameter:
Height:
Mount pattern:
Shaft size:
Wire length:
Connector / solder style:
Phase resistance:
Weight:
Aircraft model:
```

## Battery Research

Collect:

- Dead batteries
- Working batteries
- Swollen batteries for teardown only
- Battery BMS boards
- Battery terminal photos
- Battery connector measurements
- Thermistor readings
- Cell voltage notes

Document:

- Pack voltage
- Cell count
- BMS chip markings
- Fuel-gauge chip markings
- Temperature sensor locations
- Communication pins
- Authentication behavior if discovered

## Connector Library Targets

Build one page per connector:

- Battery connector
- FC to ESC / power board
- FC to gimbal
- Camera ribbon
- GPS / compass
- USB port
- Motor solder pads / connectors
- Controller internal connectors

For each connector:

```text
Connector name:
Aircraft model:
Pin count:
Pitch:
Mate part if known:
Pinout:
Measured voltage:
Signal type:
Photo top:
Photo side:
Notes:
```

## Test Equipment Useful for This Project

Already useful:

- Microscope
- Hot air station
- Soldering station
- FNIRSI scope / meter
- Bench power supply
- IPA / distilled water
- Fine probes
- 3D printer

Worth adding:

- Thermal camera or USB thermal module
- Good micro tweezer set
- Current-limited battery adapter
- DJI battery breakout adapter
- Mini motor test jig
- Gimbal holding jig
- JST / board-to-board connector sample kit
- Fine-pitch calipers or optical measurement scale

## Future Drone Libre Hardware Targets

- Mini backpack interface board
- RC-N1 controller backpack / LilyGo mount
- Remote ID test module
- ADS-B receiver integration module
- GPS / compass external test adapter
- Bench power adapter for Mini airframe
- Motor phase resistance test fixture
- Replacement FC outline board for fit checks
- Carbon-nylon midframe experiment
