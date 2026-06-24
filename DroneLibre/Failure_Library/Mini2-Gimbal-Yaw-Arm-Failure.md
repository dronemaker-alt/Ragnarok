# Failure Record - Mini 2 Gimbal Yaw Arm Failure

## Failure Identification

```text
Failure Name: Mini 2 Gimbal Yaw Arm Failure
Aircraft Model: DJI Mini 2
Subsystem: Gimbal / camera system
Severity: Medium to High
Flight Safety Impact: Medium - aircraft may fly, but camera/gimbal unusable and loose parts can be a risk
Repairable: Often
Donor Only: Sometimes
```

## Description

The Mini 2 gimbal yaw axis is vulnerable during impact. A crash can fracture the yaw arm, damage the yaw motor mount, pull screws from bosses, or tear the gimbal ribbon cable.

This failure may leave the aircraft otherwise functional, making it a strong repair candidate if the frame, ESC board, and flight controller are healthy.

## Typical Symptoms

```text
Power-on behavior: Aircraft may power on normally
App error: Gimbal stuck, gimbal overload, camera/gimbal error
Gimbal behavior: No initialization, hanging camera, grinding, twitching, crooked camera
Motor behavior: Usually unaffected unless crash also damaged arms/motors
Current draw: Usually normal unless gimbal motor is stalled
Physical evidence: Broken yaw arm, visible fracture line, pulled screws, loose gimbal
```

## Causes

```text
Impact: Primary
Water: No unless secondary event
Saltwater: No unless secondary event
Overcurrent: Possible if gimbal motor stalls after damage
Bad battery: No
Firmware/update issue: No
Previous bad repair: Possible
Unknown: Possible
```

## Diagnostic Checks

1. Photograph gimbal from front, bottom, and side.
2. Inspect yaw arm fracture line.
3. Check gimbal ribbon cable under magnification.
4. Inspect yaw motor wiring and board connector.
5. Inspect gimbal mounting bosses and rubber dampers.
6. Check whether camera image appears in app.
7. Observe gimbal initialization only if loose parts cannot jam.
8. Check aircraft body for hidden impact damage.

## Repair Procedure

```text
Parts required:
  - Yaw arm or complete gimbal assembly
  - Gimbal ribbon cable if damaged
  - Mount screws / dampers as required
Tools required:
  - Precision drivers
  - Magnification
  - Fine tweezers
  - ESD-safe handling
Steps:
  1. Document original damage.
  2. Remove gimbal assembly as required.
  3. Inspect ribbon cable before flexing further.
  4. Replace broken yaw arm or full gimbal.
  5. Reinstall with correct dampers and screws.
  6. Power up and verify initialization.
  7. Confirm camera image and horizon behavior.
```

## Example Aircraft

| Drone Libre ID | Nickname | Date | Notes |
|---|---|---|---|
| DL-003 | Mini 2 Yaw Arm | TBD | Visible yaw-axis fracture |

## Notes

This failure is a good candidate for a dedicated photo guide because the damage is common, obvious, and repairable if the ribbon cable and camera module survive.
