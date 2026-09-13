---
title: Robotic 3D-Printed Ceramics
subtitle: Merging Crafts with Digital Fabrication
tag: Digital fabrication · Robotics
year: 2023–2024
order: 7
summary: 'Robotic clay extrusion: end-effector design, toolpath computation, material experiments and
  ceramics processing.'
cover: /assets/img/ceramics-p10-06.webp
hero: /assets/img/ceramics-p09-01.webp
instructor: Shih-Yuan Wang
collaboration: Hsin Chen, Yi-Ting Lo, Glazeshome
publication: ''
research_type: Collective Design Research and Implementation
video: ''
keywords:
- 3D Printing
- Ceramics
- Robotics
- Toolpath
- Digital Fabrication
figures:
- image: /assets/img/ceramics-p09-02.webp
  caption: 'Figure 1. Approach: (a) wedging, (b) 3D printing with a robotic arm, (c) glaze and firing.'
  size: full
- image: /assets/img/ceramics-p09-03.webp
  caption: 'Figure 2. Robotic setup: end effector for clay extrusion (stepper motor, syringe, motor controller,
    linear slide rail).'
  size: half
- image: /assets/img/ceramics-p10-02.webp
  caption: Figure 4. From computation to robotic operation.
  size: half
- image: /assets/img/ceramics-p09-04.webp
  caption: 'Figure 3. Computational design (top) and 3D-printing result (bottom): rotation, expansion,
    gradient ellipse, radius with Perlin noise.'
  size: full
- image: /assets/img/ceramics-p10-03.webp
  caption: Figure 5. Exploration of material and form.
  size: full
- image: /assets/img/ceramics-p10-05.webp
  caption: 'Figure 6. Ceramics processing: bisque firing (700–900 °C), glaze, glaze firing (1200 °C).'
  size: half
- image: /assets/img/ceramics-p10-04.webp
  caption: ''
  size: half
- image: /assets/img/ceramics-p10-06.webp
  caption: Figure 7. Final production.
  size: full
---

## Overview

3D printing with robotic arms is increasingly applied in digital fabrication, where robotic manipulation allows precise control of manufacturing quality. While most 3D-printing practice uses traditional building materials such as concrete, this project explores clay extrusion.

The work covers the mechanical design of the end effector, toolpath computation, material experiments and final ceramics processing, with a focus on a design-to-fabrication workflow for small-scale 3D-printed ceramics. The trial-and-error process produced robust hardware and software settings that can be applied to other clay-based projects and related 3D-printing research.

## Experimental result

Four toolpath types were tested: rotation, expansion, gradient ellipse and randomized radius. The expansion case gave the best quality, both during printing and after ceramics processing. The rotation and randomized-radius cases showed some shrinkage after processing, possibly from thermal or humidity instability. The gradient ellipse collapsed during printing, likely because of excessive overhang in the toolpath.
