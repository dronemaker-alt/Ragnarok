# Legacy Printable Gimbal Archive

## Uploaded / Observed Files

The following files were uploaded during the archive session:

- `Mavic Modified Head for GPS and Compass v13.stl`
- `mavic_clone_gimbal_mini_split_v2.stl`
- `mavic_clone_gimbal_mini_split_v2_1.stl`
- `mavic_clone_gimbal2.stl`
- `mavic_clone_gimbal2_1.stl`
- `mavic_clone_gimbal2_2.stl`
- `mavic_clone_gimbal2_3.stl`

Reference images showed an assembled printed gimbal carrying an orange FPV-style camera.

## Observed Architecture

The gimbal concept appears to include:

- Base plate
- Yaw pivot housing
- Roll pivot tube
- Camera plate
- Printed cylindrical pivots
- Wire routing through or around pivot structures
- Low-profile installation under the fuselage

## Engineering Value

The key value is not necessarily the specific camera mount. The valuable parts are:

- Printable pivot architecture
- Low-profile underbody packaging
- Mechanical layout for camera stabilization
- Mounting strategy
- Wiring path concepts

## Drone Libre Use Cases

Potential future uses:

1. Mini Libre camera carrier reference.
2. Two-axis gimbal mechanism study.
3. Printable yaw/roll pivot geometry reference.
4. Modular sensor pod mount.
5. Lightweight payload articulation reference.

## Design Direction

For Drone Libre, the recommended path is to reuse the concept, not directly copy the old camera mount.

Candidate redesign:

```text
Aircraft body
   |
Yaw pivot
   |
Roll pivot
   |
Mini camera / sensor carrier
```

Possible payloads:

- Mini camera module
- FPV camera
- ToF sensor
- thermal sensor
- lightweight inspection camera

## Future Work

- Import each STL into FreeCAD.
- Determine how the gimbal pieces assemble.
- Measure pivot diameters and shaft clearances.
- Identify bearing or bushing requirements.
- Design a simplified Drone Libre gimbal using current sensors.
