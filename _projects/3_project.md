---
layout: page
title: Multi-robots communication
description: Communication Backbone Reconfiguration with Connectivity Maintenance.
importance: 2
img: assets/img/mr_connect.png
#category: work
---

It is considered a system with mobile multi-robots where it is needed to maintain communication between the robots while moving. The system "formation" is called backbone, the "head" robot must have connexion, in this work based on distance, with the robot before, and this last one with the robot before, until the last "tail" robot. Overall, imagine we want to send the data collected from the first robot to de last passing trough several in the middle, while moving, without losing connexion.

<div class="row justify-content-sm-center">
  <div class="col-sm-8 mt-3 mt-md-0">
    {% include figure.liquid path="assets/img/mr_connect.png" title="example image" class="img-fluid rounded z-depth-1" %}
  </div>
  <p style="font-size: 12px;" class="text-center"> Example of one result of the navigation from one backbone configuration to another with a different number of robots. First backbone configuration is showed by the green dots, each robot corresponds to one dot. Last backbone configuration is showed by the blue dots. The path for each robot has distinct color lines. This result ensures that the robots will never lose connexion during and after the navigation.
</p>
</div>

We propose a simple and effective trajectory planning framework that tackles the design, deployment, and reconfiguration of a communication backbone by reframing the problem of networked multi-agent motion planning as a manipulator motion planning problem. 
Our approach works for backbones of variable configurations both in terms of the number of robots present and the distance between each robot. 

In this project, which is current being developed, I am mainly responsible to set up the simulation, real tests and conduct the experimentation for validation of the algorithm. We are using the [Hero](https://verlab.github.io/hero_common/) platform to conduct the experimentation. Paper is on works.
