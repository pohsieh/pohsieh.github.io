---
title: A Multimedia Framework for Continuum Robots
subtitle: Systematic, Computational, and Control Perspectives
tag: Robotics · HRI
year: '2024'
order: 3
summary: A unified system for the design, simulation and control of continuum robots, in both digital
  and physical environments.
cover: /assets/img/continuum-framework-p05-01.webp
hero: /assets/img/continuum-framework-p05-01.webp
instructor: June-Hao Hou
collaboration: ''
publication: Full paper, IEEE ISPACS 2024. [doi:10.1109/ISPACS62486.2024.10868720](https://doi.org/10.1109/ISPACS62486.2024.10868720)
  · [arXiv](https://doi.org/10.48550/arXiv.2409.14708)
research_type: Independent Design Research
video: ''
keywords:
- Human–Computer Interaction
- System Architecture
- Dynamics
- Control Strategy
figures:
- image: /assets/img/continuum-framework-p05-02.webp
  caption: Figure 2. System architecture.
  size: full
- image: /assets/img/continuum-framework-p05-03.webp
  caption: Figure 3. Physics-based simulation.
  size: half
- image: /assets/img/continuum-framework-p05-04.webp
  caption: Figure 4. Computational framework.
  size: half
---

## Abstract

Continuum robots, which often rely on interdisciplinary and multimedia collaborations, have been increasingly recognized for their potential to revolutionize the field of human–robot interaction (HRI) in varied applications due to their adaptive, responsive, and flexible characteristics. Despite their promise, the lack of an integrated framework poses significant challenges for both users and developers, resulting in inefficiency and complexity during preliminary developments.

This paper introduces a unified framework for bionic robotics that addresses these challenges by integrating system architecture, dynamics computation, and control strategy. The proposed method allows for efficient modelling and quick preview of the results in both digital and physical environments, which can enhance the quality of robot developments.

## Dynamics computation

The framework integrates the computational and mechatronic system. In terms of simulation, it uses polyline objects and mesh objects to represent the tendon actuators and rigid components respectively, which reduces the computation complexity and achieves a responsive modelling method. By quickly viewing the simulated dynamics and deformation of continuum robots when applying tensile forces, users can make adjustments to reach their ideal robot configuration or locomotion.

## Control strategy

The versatility of continuum robots depends on the manipulation of the actuators’ length variations. The simulation results, manipulated from a control panel, demonstrate the effectiveness of the framework. By inserting the control function, users can control the robot’s movement by defining the ideal yaw and pitch angles (α and β).
