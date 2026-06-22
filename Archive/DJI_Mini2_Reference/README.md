# DJI Mini 2 Reference Model

## Uploaded Reference

File observed during archive session:

- `DJI_Mini_2.stl`

## Initial Mesh Notes

The uploaded STL was treated as a reference model rather than a direct print candidate.

Initial approximate dimensions observed during review:

- Length: about 201.9 mm
- Width: about 160.0 mm
- Height: about 43.3 mm
- Mesh faces: about 109,466
- Mesh vertices: about 57,514
- Mesh status: not fully watertight, but suitable for dimensional reference

## Intended Use

This model is useful as a Mini-class reference for:

- Overall body proportions
- Arm placement
- Motor position reference
- Camera/gimbal envelope reference
- Folded-aircraft packaging study
- Mini Libre exterior proportion study

## Design Notes

This reference should not be used as a direct copied flight shell. The better workflow is:

1. Import the STL into FreeCAD.
2. Use it as a visual and dimensional reference.
3. Trace major geometry into clean parametric solids.
4. Replace proprietary features with Drone Libre geometry.
5. Build an original Mini Libre body around open electronics.

## Drone Libre Derivative Concepts

Candidate future derivative:

```text
Mini Libre Alpha
├── Mini-class exterior proportions
├── H743 flight controller
├── ESP32 companion module
├── ELRS receiver
├── Remote ID node
├── GPS / compass mount
└── modular camera or sensor bay
```

## Notes for Future Measurement

Key measurements to extract later:

- Motor-to-motor diagonal
- Front arm pivot spacing
- Rear arm pivot spacing
- Fuselage length
- Fuselage width
- Battery bay size
- Gimbal opening size
- Propeller clearance envelope
