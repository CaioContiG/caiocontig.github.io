---
layout: page
title: Social Mobile Manipulator
description: Navigation of a Mobile Manipulator considering presence of humans.
img: assets/img/man_caio.jpg
importance: 1
category: current
---
My current Master's thesis focuses on *Social Navigation for Mobile Manipulators*.

Consider mobile manipulators as robots consisting of a mobile base and one or more robotic arms. In this research, we address the challenge of navigating a mobile manipulator through environments with humans, aiming to minimize the discomfort that humans may experience.

<!--- In this problem, we cannot solely rely on the usual robot navigation criteria, where a robot is deemed successful if it avoids obstacles. When interacting with humans, robots must also consider human comfort to ensure a positive work environment and coexistence. Therefore, parameters such as speed, trajectory, and other characteristics need to be adjusted. A Social Robot may ensure human comfort during its navigation, for example, the Mobile Manipulator may navigate slowly when a human is nearby, and the arm may move lower to avoid sensitive areas, such as the eyes. -->

<!--- The problem starts to get even more interesting if we consider that the robotic arm is carrying a possible danger load, like a heavy pipe, glass or a knife. In those cases is paramount to develop techniques specificly to deal in ambiance with humans. Social Robotic Navigation is a  wide largely studied reasearch area, with several ramifications to the topic, considering mobile robots. With Mobile Manipulators, works in Social Robotics tends to "retract" arms and not consider its degrees of freedom, basically considering them as a mobile robot or the arms are there for gesture and not actual carrying loads. -->

<div class="row justify-content-sm-center">
    <div class="col-sm-5 mt-5 mt-md-0">
    {% include figure.liquid path="assets/img/social-region-patomak.png" title="example image" class="img-fluid rounded z-depth-1" %}
  </div>
    <div class="col-sm-5 mt-5 mt-md-0">
    {% include figure.liquid path="assets/img/resultadoRRT.png" title="example image" class="img-fluid rounded z-depth-1" %}
  </div>
  <p style="font-size: 12px;" class="text-center"> On left, Social Regions by <a href="https://ieeexplore.ieee.org/document/9995748" target="_blank"> Patomak et al.</a>, showing a region where people might feel comfortable or uncomfortable if a robot is there. On right, RRT* result for a simplified 2D Mobile Manipulator with a holonomic mobile base and a 2-link planar robotic arm, going from a starting point to an end point.
</p>
</div>

To solve the problem in a static environment (where people do not move), we employ a Risk-RRT*-based algorithm that considers personal spaces given by Kirby. We succesfully tested our developed algorithm in several environments, and we are currently working on an online algorithm for 2D environments.

We plan to extend this to 3D. For this task, we need to compute the degree of discomfort in three dimensions, as we currently only have a 2D representation. Since the literature lacks such approaches, we are developing our own method.