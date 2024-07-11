---
layout: page
title: Social Mobile Manipulator
description: Navigation of a Mobile Manipulator considering presence of humans.
img: assets/img/man_caio.jpg
importance: 1
category: current
---
My current Master's thesis focuses on Mobile Manipulators, which are robots consisting of a mobile base with a robotic arm mounted on top. In this research, we address the challenge of navigating a Mobile Manipulator through environments with humans, classifying this work under Social Robotics.

In this problem, we cannot solely rely on the usual robot navigation criteria, where a robot is deemed successful if it avoids obstacles. When interacting with humans, robots must also consider human comfort to ensure a positive work environment and coexistence. Therefore, parameters such as speed, trajectory, and other characteristics need to be adjusted. A Social Robot may ensure human comfort during its navigation, for example, the Mobile Manipulator may navigate slowly when a human is nearby, and the arm may move lower to avoid sensitive areas, such as the eyes.

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

We are currently testing a RRT* based algorithm to consider social norms in 2D using MatLab. We plan to extend for 3D, use a non-holonomic base and test decoupled (compute arm and base movement separetely) algorithms, consider groups of people and run on a real mobile-manipulator present in our laboratory.