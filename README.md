# EDITH-CAD: 5-DOF Articulated Arm + Parallel Gripper

This repository contains the **mechanical CAD deliverables** for EDITH's articulated robotic arm.

## Scope

Included in this repository:
- 5-DOF articulated robotic arm mechanical CAD
- Separate parallel gripper mechanism

Not included:
- Mobile base/chassis
- Electronics, firmware, ROS 2, or software stacks

## Primary CAD Deliverable (SOLIDWORKS-compatible)

- **Complete assembled STEP file**: `CAD/assemblies/EDITH_5DOF_Arm_Parallel_Gripper.step`

This STEP assembly is the primary file intended for import/opening in SOLIDWORKS.

## Repository Layout

- `CAD/assemblies/` — final assembly model files
- `CAD/BOM/` — bill of materials
- `CAD/docs/` — joint, units, and dimension notes

## Assembly Definition

The assembly is modeled as a compact 5-DOF arm with these rotational joints:
1. **J1 Base yaw** (rotating base)
2. **J2 Shoulder pitch**
3. **J3 Elbow pitch**
4. **J4 Wrist pitch**
5. **J5 Wrist roll**

The **parallel gripper** is implemented as a separate end-effector mechanism and is **not counted** as an extra arm DOF.

## Units and Dimension Policy

- Modeling units: **millimeters (mm)**
- Implemented dimensions are documented in `CAD/docs/design_notes.md`
- Values marked **provisional** are concept-level values for geometry/interfaces only

## Deliverable Status

| Deliverable | Status | Path / Notes |
|---|---|---|
| Complete assembled STEP model | ✅ Generated | `CAD/assemblies/EDITH_5DOF_Arm_Parallel_Gripper.step` |
| Native SOLIDWORKS assembly/parts (`.SLDASM`, `.SLDPRT`) | ⚠️ Not generated in this environment | Not available from this cloud environment |
| Engineering drawings | ⚠️ Incomplete | Not generated in this cloud environment |
| Bill of Materials | ✅ Generated | `CAD/BOM/EDITH_5DOF_Arm_BOM.csv` |

## Validation and Limitations

- This repository contains a real STEP assembly model (not STL-only substitution).
- No torque, payload, or structural validation claims are made.
- Actuator interfaces and performance-critical dimensions are marked provisional in documentation.
