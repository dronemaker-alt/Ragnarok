# VZ Mavic Clone Reference Project

## Source Identification

Known reference page from the user's archive session:

- Title: `mavic clone 1.22 enlarge`
- Platform: Thingiverse
- Thing number observed: `5210659`
- Creator shown in browser screenshot: `thingiiC0`
- Page date shown: January 21, 2022

## Files Observed in Local Archive

The local folder contains both a complete assembly and individual components.

### STEP Files

- `MAVIC_CLONE.stp`
- `MAVIC_CLONE_PLEGADO.stp`

`Plegado` means folded, suggesting the project includes both deployed and folded configurations.

### Major STL Components Observed

- `BRAZO_DELANTERO_DERECHO.stl` — front right arm
- `BRAZO_DELANTERO_IZQUIERDO.stl` — front left arm
- `BRAZO_TRASERO_DERECHO.stl` — rear right arm
- `BRAZO_TRASERO_IZQUIERDO.stl` — rear left arm
- `CHASIS_MEDIO.stl` — center chassis
- `CUBIERTA_DELANTERA.stl` — front cover
- `CUBIERTA_TRASERA.stl` — rear cover
- `GIMBAL_HOLDER.stl`
- `NOSE_NAZA.stl`
- `SOPORTE_BATERIA.stl` — battery support
- `SOPORTE_LED_NAZA.stl`
- `SOPORTE_NAZA_LITE.stl`
- `REJILLA_VENTILACION_DER.stl`
- `REJILLA_VENTILACION_IZQ.stl`

## FreeCAD Import Notes

The `MAVIC_CLONE.stp` assembly was opened in FreeCAD 1.0.

Observed assembly items include:

- `CUERPO_ASS` — body assembly
- `CHASIS_MEDIO007` — center chassis instance
- `SOPORTE_BATERIA` — battery support
- `SOPORTE_NAZA_LITE` — NAZA Lite support
- `BRAZO_DELANTERO_DERECHO` — front right arm
- `BRAZO_TRASERO_DERECHO` — rear right arm
- `BRAZO_TRASERO_IZQUIERDO` — rear left arm
- `CUBIERTA_DELANTERA` — front cover
- `CUBIERTA_TRASERA` — rear cover
- multiple `INSERTO_ROSCA_M3x###` entries — M3 threaded inserts
- multiple `TORNILLO_M3x10` entries — M3 screws

## Engineering Value

This project is valuable because it preserves:

- Folding arm geometry
- Arm pivot architecture
- Battery support layout
- NAZA-era flight controller mounting
- Modular nose and cover geometry
- Separate component organization suitable for study in FreeCAD

## Drone Libre Use Cases

Possible uses for Drone Libre development:

1. Baseline folding-arm geometry study.
2. Donor mechanism for Mini Libre Alpha.
3. Reference for Mavic-style arm packaging.
4. Battery bay and electronics-bay layout reference.
5. Starting point for replacing NAZA mounts with H743 / ESP32 / ELRS / Remote ID hardware.

## Configuration Control

Recommended workflow:

1. Keep original STEP and STL files unchanged.
2. Save a FreeCAD copy as `MAVIC_CLONE_BASELINE.FCStd`.
3. Create a working derivative as `DRONELIBRE_MK1.FCStd`.
4. Modify only the working derivative.
5. Record every major geometry change in this folder.
