# EDITH 5-DOF Arm Design Notes

## Units

- All dimensions are in **millimeters (mm)**.

## Joint Axes (Implemented Geometry)

- **J1 Base yaw**: rotation about global Z-axis at base rotor.
- **J2 Shoulder pitch**: rotation about local Y-axis at shoulder shaft.
- **J3 Elbow pitch**: rotation about local Y-axis at elbow joint.
- **J4 Wrist pitch**: rotation about local Y-axis near forearm tip.
- **J5 Wrist roll**: rotation about local forearm/tool axis at wrist roll housing.

The gripper is modeled as a parallel mechanism attached to the wrist and is not an additional DOF.

## Key Implemented Dimensions

- Base radius: 45 mm
- Base height: 20 mm
- Turntable radius: 28 mm
- Shoulder mount block: 28 x 36 x 32 mm
- Upper arm length: 150 mm
- Forearm length: 130 mm
- Wrist pitch joint diameter: 24 mm
- Wrist roll housing diameter: 20 mm
- Gripper palm size: 14 x 32 x 24 mm
- Jaw size (each): 8 x 55 x 8 mm

## Provisional Items

The following are provisional and require downstream mechanical/electromechanical engineering before fabrication:

- Actuator/motor interfaces and mounting patterns
- Bearing/bushing selection and fit classes
- Fastener specifications
- Hard-stop ranges and collision clearances for full-motion operation
- Payload, torque, and stiffness performance
