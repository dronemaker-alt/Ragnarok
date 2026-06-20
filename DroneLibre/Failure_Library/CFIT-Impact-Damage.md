# Failure Record - CFIT / Impact Damage

## Failure Identification

```text
Failure Name: CFIT / Impact Damage
Aircraft Model: DJI Mini / Mini 2 family
Subsystem: Airframe, gimbal, motors, ESC board risk
Severity: Medium to High
Flight Safety Impact: High
Repairable: Often
Donor Only: Sometimes
```

## Description

Controlled Flight Into Terrain damage is caused by the aircraft impacting the ground or an object while under power. In small DJI aircraft, the gimbal and arms often absorb the obvious damage, while hidden damage may exist in motors, frame bosses, ESC circuits, and ribbon cables.

## Typical Symptoms

```text
Power-on behavior: May power on normally or fail due to secondary damage
App error: Gimbal error, motor error, IMU/compass error possible
Gimbal behavior: Grinding, no initialization, crooked horizon, yaw/roll/pitch failure
Motor behavior: Bearing noise, no spin, rough spin, phase imbalance
Current draw: Usually normal unless ESC/motor damaged
Physical evidence: Cracked shell, pulled screws, broken gimbal arm, prop damage
```

## Causes

```text
Impact: Primary
Water: Possible secondary depending on crash site
Saltwater: Possible secondary depending on crash site
Overcurrent: Possible if motor stalled during crash
Bad battery: Possible but not primary
Firmware/update issue: Usually unrelated
Previous bad repair: Possible
Unknown: Possible
```

## Diagnostic Checks

1. Photograph aircraft before repair.
2. Inspect shell, arm hinges, screw bosses, and motor mounts.
3. Check motor bearing feel and shaft/bell alignment.
4. Measure motor phase resistance.
5. Inspect gimbal arms and ribbon cable.
6. Check main bus resistance before applying power.
7. Power through current-limited source if available.
8. Record app errors and gimbal initialization behavior.

## Repair Procedure

```text
Parts required: Depends on impact location
Tools required: Microscope, precision drivers, meter, solder tools as needed
Steps:
  1. Document damage.
  2. Replace unsafe props.
  3. Repair/replace broken gimbal or frame parts.
  4. Verify motors electrically and mechanically.
  5. Confirm no main-bus short.
  6. Power up and record errors.
  7. Complete ground test before flight.
Post-repair checks: Motor test, gimbal initialization, IMU/compass status, controlled hover
```

## Example Aircraft

| Drone Libre ID | Nickname | Date | Notes |
|---|---|---|---|
| DL-001 | CFIT | TBD | Baseline CFIT example |
| DL-003 | Mini 2 Yaw Arm | TBD | Impact concentrated at gimbal yaw axis |

## Notes

Do not trust an aircraft just because it powers on after impact. The sneaky failures are motor bearings, cracked solder joints, damaged connectors, and gimbal ribbon damage.
