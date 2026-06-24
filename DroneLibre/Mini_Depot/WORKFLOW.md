# Mini Depot Workflow

This is the standard intake, repair, and test process for DJI Mini / Mini 2 aircraft entering the Drone Libre bench.

## 1. Intake Record

Create one record per aircraft in `Mini_Depot/Intake_Records/`.

Required fields:

```text
Drone Libre ID:
Nickname:
Model:
Serial Number:
Source:
Purchase Price:
Date Received:
Included Items:
Reported Failure:
Observed Failure:
Accident Classification:
Initial Disposition:
```

Suggested accident classifications:

- CFIT - Controlled Flight Into Terrain
- Water Recovery
- Saltwater Recovery
- Flyaway / Runaway
- Update Failure
- Electrical Failure
- Gimbal Damage
- Unknown

## 2. Initial Visual Inspection

Photograph before repair.

Required photos:

- Top shell
- Bottom shell
- Front
- Rear
- Left arm
- Right arm
- Gimbal closeup
- Battery bay
- Serial label
- Any corrosion or impact marks

Inspection checklist:

```text
Frame cracks:
Arm damage:
Motor damage:
Prop damage:
Gimbal damage:
Ribbon cable damage:
Battery latch condition:
Battery terminal condition:
Evidence of water/corrosion:
Evidence of previous repair:
Missing screws/covers:
```

## 3. No-Power Electrical Safety Check

Before connecting a known-good battery:

1. Remove damaged battery.
2. Inspect battery bay and terminals.
3. Check resistance from main battery positive to ground.
4. Check obvious shorts on 5V and 3.3V rails if accessible.
5. Inspect ESC / power board for burned MOSFETs, cracked inductors, missing components, and corrosion.

Do not apply power if the main bus is shorted.

## 4. Controlled Power-Up

Preferred sequence:

1. Bench supply with current limit if an adapter is available.
2. Start with conservative current limit.
3. Watch for excessive current draw.
4. Check regulator outputs.
5. Check for heat with finger test / thermal camera if available.
6. Only then test with a good battery.

## 5. ESC and Motor Checks

For each motor:

```text
Motor Position:
Physical condition:
Bearing feel:
Bell wobble:
Shaft damage:
Thread condition:
Phase A-B resistance:
Phase B-C resistance:
Phase A-C resistance:
Notes:
```

Compare all three phase readings. A motor with one odd reading is suspect. A motor with crunchy bearings is a donor or replacement candidate, not a flight part.

## 6. Gimbal Checks

Common Mini / Mini 2 crash failures:

- Broken yaw arm
- Torn ribbon cable
- Pulled mounting bosses
- Camera module damage
- Bent gimbal frame
- Initialization failure

Record:

```text
Yaw axis condition:
Roll axis condition:
Pitch axis condition:
Ribbon cable condition:
Camera module condition:
Gimbal board condition:
Initialization behavior:
```

## 7. Corrosion Recovery

For saltwater or unknown water exposure:

1. Photograph before cleaning.
2. Disassemble enough to expose affected boards.
3. Remove shields only when needed and when tools allow.
4. Rinse contaminated areas with distilled water.
5. Follow with 99% IPA.
6. Dry thoroughly before power.
7. Re-check resistance from main battery positive to ground.
8. Inspect under magnification.

Saltwater aircraft get a separate corrosion note even if they power on. Salt is a tiny white demon with a soldering iron. Treat accordingly.

## 8. Software / Binding / Functional Checks

Record:

```text
Powers on:
Controller bind status:
App connection:
Firmware version:
Error codes:
GPS lock:
Compass status:
IMU status:
Camera image:
Gimbal movement:
Motor spin test:
```

## 9. Ground Test

Before flight:

- Props off motor test
- Props on restrained idle check if appropriate
- GPS lock check
- Gimbal initialization
- Compass / IMU status
- Battery status
- Return-to-home settings

## 10. Flight Test

First flight profile:

1. Low hover.
2. Yaw left/right.
3. Small forward/back/side translations.
4. Gentle climb/descent.
5. RTH check only when safe.
6. Land and inspect motors, battery, and frame.

Record flight result in `Mini_Depot/Flight_Test_Records/`.
