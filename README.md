# EDITH — 5-DOF Robotic Arm CAD

**A SolidWorks mechanical CAD project featuring an articulated robotic arm, rotating base, and parallel gripper.**

---

## 1. Overview

EDITH is a robotic arm design project focused on the mechanical development of an articulated manipulator for object handling and pick-and-place applications.

The design, modelled in SOLIDWORKS, features a circular base assembly, articulated arm links, multiple mechanical joints, and a two-finger gripper. The project focuses on the arm's mechanical structure, joint arrangement, assembly design, and potential for future development.

This repository is dedicated exclusively to the **EDITH robotic arm CAD design**. It does not cover the complete mobile robot, embedded firmware, AI systems, or high-level robotics software.

## 2. CAD Design

The current design reference depicts the following mechanical components:

* **Circular base assembly:** The base structure supporting the arm and its mounting interface.
* **Shoulder assembly:** The joint connecting the base region to the first articulated link.
* **Upper arm link:** The primary structural link between the shoulder and elbow.
* **Elbow assembly:** The joint connecting the two principal arm links.
* **Forearm link:** The structural link connecting the elbow region to the wrist.
* **Wrist assembly:** The distal joint structure connecting the forearm to the gripper.
* **Parallel gripper:** Two opposing fingers intended for grasping and releasing objects.
* **Mechanical fasteners and brackets:** Components visible in the model that contribute to the assembly's construction.

The image in this repository represents the current visual CAD reference. Detailed dimensions, internal mechanisms, actuator specifications, and joint-motion characteristics must be established from the underlying CAD files and hardware specifications.

## 3. Intended Joint Configuration

The design is intended to follow a five-degree-of-freedom (5-DOF) articulated-arm configuration.

| Joint | Intended function            |
| ----- | ---------------------------- |
| J1    | Base rotation                |
| J2    | Shoulder movement            |
| J3    | Elbow movement               |
| J4    | Wrist movement               |
| J5    | Additional wrist orientation |

The parallel gripper is a separate end-effector mechanism and is not counted as one of the five arm degrees of freedom.

**Note:** The final joint axes, permitted ranges of motion, and independent actuation of all five joints must be verified against the actual assembly. The reference image alone does not establish these properties.

## 4. Software and File Formats

### CAD Software

* SOLIDWORKS

### Relevant CAD File Formats

| Extension        | Description                 |
| ---------------- | --------------------------- |
| `.SLDPRT`        | SOLIDWORKS part file        |
| `.SLDASM`        | SOLIDWORKS assembly file    |
| `.SLDDRW`        | SOLIDWORKS drawing file     |
| `.STEP` / `.STP` | Neutral CAD exchange format |

The repository should identify which files are actually available.

A complete native SOLIDWORKS assembly may reference multiple part files. A single STEP file can provide a convenient exchange model, but it may not preserve the original feature history, assembly mates, or motion definitions.

## 5. Repository Structure

The repository is intended to organize the arm's CAD model and associated documentation.

```text
EDITH-5DOF-Robotic-Arm-CAD/
├── README.md
├── Images/
│   └── EDITH_5DOF_Arm_Assembly_Reference.png
├── CAD/
│   ├── Assembly/
│   ├── Parts/
│   ├── Drawings/
│   └── Exports/
└── Documentation/
    ├── Mechanical_Design.md
    └── Design_Notes.md
```

This is a proposed directory structure. Individual folders and files should be included only when they exist in the repository.

## 6. Mechanical Design Considerations

The design may require further engineering work before it is ready for fabrication or physical operation.

Areas for future evaluation include:

* Joint geometry and mechanical limits.
* Actuator mounting interfaces.
* Link dimensions and material selection.
* Joint torque requirements.
* Gripper opening width and gripping force.
* Cable routing and moving-part clearance.
* Structural stiffness and component deformation.
* Mass distribution and centre of gravity.
* Mounting interface strength.

These are engineering considerations, not claims that the relevant analyses have already been completed.

## 7. Future Development

Potential future work includes the following.

### 7.1 CAD Refinement

* Finalize the dimensions of the mechanical components.
* Verify the joint arrangement and actuator interfaces.
* Refine the base, arm links, wrist, and gripper assemblies.
* Check assembly clearances and mechanical interference.
* Produce engineering drawings and a bill of materials.

### 7.2 Kinematic Analysis

* Define the coordinate frame for each joint.
* Develop forward and inverse kinematic models.
* Determine the reachable workspace.
* Establish joint limits.
* Evaluate self-collision and end-effector positioning.

### 7.3 Simulation Preparation

Once the mechanical geometry and physical properties are available, the model may be prepared for future robotics simulation using appropriate tools, such as ROS 2, RViz 2, Gazebo, and MoveIt 2.

This is a future development objective; the presence of these tools or a working simulation is not implied by the CAD reference alone.

### 7.4 Hardware Integration

Future physical implementation may involve selecting compatible actuators, integrating an embedded controller, routing electrical connections, and testing individual joints.

Actuator selection and payload capability must be established through engineering calculations and hardware specifications.

### 7.5 Manipulation Capabilities

Potential future applications include:

* Object grasping and release.
* Pick-and-place operations.
* Position-controlled manipulation.
* Camera-assisted object handling.
* Integration into a larger robotic system.

These are intended application areas, not verified capabilities of the current CAD model.

## 8. Design Status

The repository documents the mechanical CAD design of EDITH's robotic arm.

The following information should be documented as the design progresses:

* Actual dimensions and units.
* Verified joint configuration.
* Actuator models and specifications.
* Material assignments.
* Gripper specifications.
* Assembly completeness.
* Engineering calculations and simulation results.
* Manufacturing and testing status.

Any preliminary values should be identified as estimates or design targets rather than confirmed specifications.

## 9. Scope

This repository covers the **EDITH 5-DOF robotic arm and its gripper CAD design**.

The following are outside the scope of this repository:

* The four-wheel mobile robot chassis.
* Embedded firmware.
* AI and computer vision systems.
* High-level control software.
* The complete robot's system architecture.

These subsystems may be integrated into the broader EDITH project in the future.

## 10. Safety and Validation

A visual CAD model does not establish mechanical strength, actuator suitability, payload capacity, or safe operation.

Before physical implementation, the design should be evaluated for structural loads, joint torque, mechanical interference, actuator limits, electrical requirements, and applicable safety considerations.

No payload rating or performance specification should be published without supporting calculations, manufacturer data, or experimental validation.

---

**Project:** EDITH — 5-DOF Robotic Arm CAD
**Primary CAD software:** SOLIDWORKS
**Design focus:** Articulated arm, rotating base, wrist mechanism, and parallel gripper
**Development status:** Mechanical CAD development
