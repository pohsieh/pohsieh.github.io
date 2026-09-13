---
title: Visualization and Optimization of Continuum Robots
subtitle: Integration of Lie Group Kinematics and Evolutionary Algorithm
category: robotics
tag: Computational modelling
year: '2024'
order: 2
summary: An efficient modelling method for continuum robots that replaces manual modal-coefficient identification
  with an evolutionary algorithm.
cover: /assets/img/lie-group-p06-01.webp
hero: /assets/img/lie-group-p06-01.webp
instructor: June-Hao Hou
collaboration: ''
location: ''
publication: 'Preprint on arXiv: [arXiv:2410.14305](https://doi.org/10.48550/arXiv.2410.14305)'
research_type: Independent Design Research
video: 9UWLf1npNsw
keywords:
- Robot Modelling
- Lie Group
- Evolutionary Algorithm
figures:
- image: /assets/img/lie-group-p06-02.webp
  caption: 'Figure 2. Method: (a) input dataset, (b) evolutionary algorithm, (c) generated continuum robot
    model.'
  size: full
- image: /assets/img/lie-group-p06-04.webp
  caption: 'Fitness objectives: deviation MSE and TCP vector MSE.'
  size: half
- image: /assets/img/lie-group-p06-07.webp
  caption: Figure 7. Computational framework.
  size: half
- image: /assets/img/lie-group-p06-03.webp
  caption: Figure 3. Standard deviation graph.
  size: half
- image: /assets/img/lie-group-p06-05.webp
  caption: Figure 4. Fitness values graph.
  size: half
- image: /assets/img/lie-group-p06-06.webp
  caption: Figure 5. Standard deviation trendline.
  size: half
- image: /assets/img/lie-group-p06-08.webp
  caption: Figure 6. Fitness values trendline.
  size: half
- image: /assets/img/lie-group-p06-09.webp
  caption: 'Figure 8. Optimization process over three stages (light: target configuration, dark: optimized
    configuration over time).'
  size: full
---

## Abstract

Continuum robots, known for their flexibility and compliance, offer great potential in applications such as medical surgeries, inspections in confined spaces, and wearable devices. However, the complexity of their non-linear kinematics and the challenge of achieving effective control and digital modelling hinder their broader adoption.

This paper proposes a novel approach to continuum robot modelling by combining Lie group kinematics with an evolutionary algorithm. Instead of traditional methods that rely on manual identification of modal coefficients, this approach automates the process through an evolutionary optimization mechanism. The proposed method minimizes the deviations between simulated configurations and ideal shapes, improving efficiency and accuracy in robot design. Results show the effectiveness of this approach in reducing computational complexity, allowing for real-time modelling and control of continuum robots.

## Proposed method

The main concept of the proposed method starts with replacing the traditional modal coefficients identification process with an evolutionary algorithm, which is automated and accurate. First, a series of robot configurations are generated using fractional order control and physics-based simulations in Grasshopper. These configurations are set as the ideal shapes for the modal shape function s(x). The fitness objective of the evolutionary algorithm is to minimize the deviations between the shape derived from the modal shape function and the ideal ones: (1) minimize the deviation mean squared error, and (2) minimize the TCP vector mean squared error. Generation size 20, generation count 10, population size 200, crossover probability 90%.

## Results

The comparison between Generation 0 (the first generation) and Generation 9 (the last generation) highlights the effectiveness of the evolutionary algorithm in identifying the modal coefficients. Individuals from Generation 0 have a lower fitness value, showing less similarity to the ideal configuration; individuals from Generation 9 have been refined by the evolutionary algorithm with an improved fitness value.
