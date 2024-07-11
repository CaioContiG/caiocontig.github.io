---
layout: page
title: Multi-robots Navigation
description: Communication Backbone Reconfiguration with Connectivity Maintenance.
importance: 3
img: assets/img/hero-test.png
category: current
---

We consider a system with multi ground mobile robots where it is needed to maintain communication between the robots while moving. The scenario consists of a leader robot transmitting (wireless) an information to the next robot in line, which then passes it along to the subsequent robots until it reaches the base station. This line of robots, the formation, is called "backbone". The robots lose conection with each other based on line-of-sight. We want to be able to move robots between backbone configurations, without losing connection and use the least amount of robots possible.

<div class="row justify-content-sm-center">
  <div class="col-sm-8 mt-3 mt-md-0">
    {% include figure.liquid path="assets/img/mr_connect.png" title="example image" class="img-fluid rounded z-depth-1" %}
  </div>
  <p style="font-size: 12px;" class="text-center"> Example of one result of the navigation from one backbone configuration to another with a different number of robots. First backbone configuration is showed by the green dots, each robot corresponds to one dot. Last backbone configuration is showed by the blue dots. The path for each robot has distinct color lines. This result ensures that the robots will never lose connexion during and after the navigation.
</p>
</div>

We propose a simple and effective trajectory planning framework that tackles the design, deployment, and reconfiguration of a communication backbone by reframing the problem of networked multi-agent motion planning as a manipulator motion planning problem. Our approach works for backbones of variable configurations both in terms of the number of robots present and the distance between each robot. We are using the [Hero](https://verlab.github.io/hero_common/) platform to conduct the experimentation. Paper is on works.
