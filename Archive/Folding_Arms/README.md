# Folding Arm Reference Notes

## Concepts Reviewed

Two folding-arm families were discussed during the archive session.

## 1. Mavic-Style Folding Arms

The VZ Mavic Clone project includes separate arms:

- Front right arm
- Front left arm
- Rear right arm
- Rear left arm

These parts were individually selectable in FreeCAD after STEP import, confirming useful assembly structure.

### Value

- Compact folded footprint
- Established Mavic-like packaging
- Separate arm geometry available for study
- Existing hinge placement data

### Concerns

- More complex geometry
- More proprietary-style packaging
- Less repairable than carbon tube arms

## 2. Horizontal Folding Carbon Tube Arms

A horizontal folding arm mechanism was reviewed from product photos. This style swings the arm around the side of the aircraft rather than folding vertically.

Observed features:

- Carbon tube arm compatibility
- Large hinge block
- Approximate hinge block length around 120 mm in product image
- Tube diameter callouts around 30 mm in product image
- Tube arm systems commonly used on 15 inch / 17 inch long-range FPV frames

### Value

- Stronger arm root
- Easier wiring path
- Easier repair
- Compatible with carbon tubes
- Suitable for larger Gondul-style aircraft

## Preferred Drone Libre Direction

The preferred direction is a hybrid approach:

```text
Carbon tube structure
+
Horizontal folding pivots
+
Mini / Mavic inspired nose and body shell
+
Open electronics stack
```

This combines the repairability of tube-frame aircraft with the clean packaging of a Mini-style airframe.

## Candidate Applications

### Mini Libre Alpha

- Mavic Clone folding geometry
- Open flight controller
- ESP32 companion module
- Remote ID
- Modified nose and electronics bay

### Gondul Alpha

- Carbon tube frame
- Horizontal folding hinges
- Phanvick/Gondul shell
- H743 flight controller
- companion electronics bay
- modular payload nose

## Future Work

1. Export individual Mavic Clone arms as STL/STEP working references.
2. Measure pivot geometry and arm sweep.
3. Compare Mavic-style vertical folding with horizontal tube folding.
4. Build a simplified hinge test coupon.
5. Decide whether Mini Libre uses printed pivots, purchased metal hinges, or carbon-tube hinge blocks.
