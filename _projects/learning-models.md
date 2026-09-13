---
title: Comparative Evaluation of Learning Models
subtitle: for Bionic Robots
category: robotics
tag: Machine learning
year: '2024'
order: 4
summary: Evaluating machine-learning models for the model-free control of a tendon-driven bionic robot.
cover: /assets/img/learning-models-p03-01.webp
hero: /assets/img/learning-models-p03-01.webp
instructor: June-Hao Hou
collaboration: ''
location: ''
publication: Full paper, IEEE ISPACS 2024. [doi:10.1109/ISPACS62486.2024.10868337](https://doi.org/10.1109/ISPACS62486.2024.10868337)
  · [arXiv](https://doi.org/10.48550/arXiv.2407.02428)
research_type: Independent Design Research
video: ''
keywords:
- Model-Free Control
- Continuum Robot
- Learning-Based Method
figures:
- image: /assets/img/learning-models-p03-02.webp
  caption: 'Figures 1–4. Actual motions for N = 1–4 segments: α and β over time.'
  size: half
- image: /assets/img/learning-models-p03-03.webp
  caption: ''
  size: half
- image: /assets/img/learning-models-p03-04.webp
  caption: ''
  size: half
- image: /assets/img/learning-models-p03-05.webp
  caption: ''
  size: half
- image: /assets/img/learning-models-p04-01.webp
  caption: Figure 5. α deviations (β = 0).
  size: half
- image: /assets/img/learning-models-p04-02.webp
  caption: Figure 6. β deviations (α = 0).
  size: half
- image: /assets/img/learning-models-p04-03.webp
  caption: Figure 7. Methodology.
  size: full
- image: /assets/img/learning-models-p04-04.webp
  caption: 'Figure 8. Data collection: (a) inputs, pitch and yaw angles; (b) outputs, tendon length variations.'
  size: half
- image: /assets/img/learning-models-p04-06.webp
  caption: 'Figure 10. Transfer functions: (a) original, (b) proposed.'
  size: half
- image: /assets/img/learning-models-p04-05.webp
  caption: 'Figure 9. Training results: (a) gradient boosting, (b) lasso regression, (c) support vector,
    (d) recurrent neural network.'
  size: full
- image: /assets/img/learning-models-p04-07.webp
  caption: Figure 11. Robot performance before and after training.
  size: full
---

## Abstract

The control and modelling of bionic robot dynamics have increasingly adopted model-free control strategies using machine learning. Given the non-linear elastic nature of bionic robotic systems, learning-based methods provide reliable alternatives by using numerical data to establish a direct mapping from actuation inputs to robot trajectories without complex kinematic models. However, how developers should choose an appropriate learning model for their specific robot, and construct its transfer function, has not been thoroughly discussed.

This research trains four types of models — ensemble learning, regularization-based, kernel-based and neural network models — suitable for multi-input multi-output (MIMO) data and non-linear transfer function identification, and evaluates their (1) accuracy, (2) computation complexity and (3) performance in capturing biological movements.

## Research problem

For a tensegrity-based continuum robot with a fractional-order control algorithm, target yaw and pitch angles from −90° to 90° were inserted at 10° intervals, and the length variation of each tendon actuator was collected. Four conditions with different numbers of segments (N = 1–4) were tested. A noticeable deviation between the actual and desired motions was observed, indicating that the original transfer functions do not fully capture the non-linear dynamics of the tendon-driven robot.

## Method

Data collection uses physics simulations to capture robot motions (yaw and pitch) and the corresponding actuation parameters (tendon length variations L1, L2, L3). Eight learning models suitable for non-linear data are trained on the dataset and compared for accuracy and computation cost. Finally, the transfer function derived from each model is sent back to the robot simulation to validate the locomotion against biomimetic metrics.

## Results

Gradient boosting gave predictions most closely aligned with the actual values. Despite its lower accuracy, lasso regression had a markedly lower time cost, which makes it suitable for real-time applications.
