# Failure Record - Saltwater Recovery

## Failure Identification

```text
Failure Name: Saltwater Recovery
Aircraft Model: DJI Mini / Mini 2 family
Subsystem: Entire aircraft, especially power board, connectors, motors, battery
Severity: High
Flight Safety Impact: High
Repairable: Sometimes
Donor Only: Often
```

## Description

Saltwater recovery aircraft have been exposed to conductive and corrosive contamination. Even if the aircraft powers on after drying, salt residue can continue damaging connectors, boards, motor bearings, solder joints, and flex cables.

Saltwater contamination should be treated as an active chemical/electrical failure, not simply as water exposure.

## Typical Symptoms

```text
Power-on behavior: No power, high current draw, intermittent power, or delayed failure
App error: May not connect, ESC error, gimbal error, battery error
Gimbal behavior: No movement, jittering, grinding, failed initialization
Motor behavior: Rough bearings, seized motor, ESC fault, phase imbalance
Current draw: May be excessive if contamination creates leakage/shorts
Physical evidence: White/green residue, salt crystals, corrosion at connectors
```

## Causes

```text
Impact: Possible
Water: Yes
Saltwater: Primary
Overcurrent: Possible secondary
Bad battery: Possible / likely if submerged
Firmware/update issue: Usually unrelated
Previous bad repair: Possible if only dried and powered without cleaning
Unknown: No
```

## Diagnostic Checks

1. Do not insert a known-good battery until main-bus resistance is checked.
2. Photograph aircraft before cleaning.
3. Inspect battery bay, terminals, and connectors.
4. Remove boards as needed for inspection.
5. Check main battery positive to ground resistance.
6. Check 5V and 3.3V rails for shorts.
7. Inspect ESC / power board under magnification.
8. Inspect motor bearings and phase resistance.
9. Inspect gimbal and camera flex connectors.
10. Power only through current-limited source after cleaning and drying.

## Cleaning Procedure

```text
Tools/materials:
  - Distilled water
  - 99% IPA
  - Soft brush
  - Compressed air / blower
  - Microscope
  - Current-limited bench supply

Steps:
  1. Photograph contamination.
  2. Remove battery.
  3. Disassemble to affected boards.
  4. Rinse salt contamination with distilled water where appropriate.
  5. Brush gently.
  6. Rinse with IPA.
  7. Dry thoroughly.
  8. Inspect under magnification.
  9. Recheck resistance.
  10. Power carefully with current limit.
```

## Example Aircraft

| Drone Libre ID | Nickname | Date | Notes |
|---|---|---|---|
| DL-002 | Davey Jones | TBD | Ocean recovery / no power after drying |

## Notes

Drying a saltwater aircraft without cleaning it is how you make tiny electronic jerky. The salt stays behind and keeps eating the aircraft.
