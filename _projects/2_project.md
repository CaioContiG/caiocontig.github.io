---
layout: page
title: Social Mobile Manipulator
description: Navigation of a Mobile Manipulator considering presence of humans.
img: assets/img/man_caio.jpg
importance: 1
category: current
---
My current Master's thesis focuses on *Social Navigation for Mobile Manipulators*. 

Experiment videos: [EXP1](https://www.youtube.com/watch?v=lLFQ12lf_go), [EXP2](https://www.youtube.com/watch?v=c8PtqI2iLMM), [EXP3](https://www.youtube.com/watch?v=tNo6pqw-BAA).

<div class="row justify-content-sm-center">
  <div class="col text-center">
    {% include figure.liquid path="assets/img/social_nav.gif" class="img-fluid rounded z-depth-1" %}
  </div>
  <div class="col text-center">
    {% include figure.liquid path="assets/img/not_social_nav.gif" class="img-fluid rounded z-depth-1" %}
  </div>
</div>
<div class="row">
  <div class="col text-center">
    <p style="font-size: 12px;">Simulation of a mobile manipulator transporting a bar-like object in an office-like environment.</p>
  </div>
</div>


Consider mobile manipulators as robots consisting of a mobile base and one or more robotic arms. In this research, we address the challenge of navigating a mobile manipulator *transporting an object* through environments with humans, aiming to minimize the discomfort that humans may experience.

<!--- In this problem, we cannot solely rely on the usual robot navigation criteria, where a robot is deemed successful if it avoids obstacles. When interacting with humans, robots must also consider human comfort to ensure a positive work environment and coexistence. Therefore, parameters such as speed, trajectory, and other characteristics need to be adjusted. A Social Robot may ensure human comfort during its navigation, for example, the Mobile Manipulator may navigate slowly when a human is nearby, and the arm may move lower to avoid sensitive areas, such as the eyes. -->

<!--- The problem starts to get even more interesting if we consider that the robotic arm is carrying a possible danger load, like a heavy pipe, glass or a knife. In those cases is paramount to develop techniques specificly to deal in ambiance with humans. Social Robotic Navigation is a  wide largely studied reasearch area, with several ramifications to the topic, considering mobile robots. With Mobile Manipulators, works in Social Robotics tends to "retract" arms and not consider its degrees of freedom, basically considering them as a mobile robot or the arms are there for gesture and not actual carrying loads. -->

<div class="row justify-content-sm-center">
  <div class="col">
    {% include figure.liquid path="assets/img/comfort_map.png" title="Comfort Map of the Environment" class="img-fluid rounded z-depth-1" %}
    <p style="font-size: 12px;" class="text-center">Contour Comfort Map visualization. The blue dot at (3,4) represents the human's position. Higher values indicate lower comfort levels.</p>
  </div>
  <div class="col">
    {% include figure.liquid path="assets/img/illustrative_social.png" title="Ground Vehicle Navigation Path" class="img-fluid rounded z-depth-1" %}
    <p style="font-size: 12px;" class="text-center">Socially-aware mobile manipulator transporting an object (ours).</p>
  </div>
  <div class="col">
    {% include figure.liquid path="assets/img/illustrative_nosocial.png" title="Aerial Vehicle Task Execution" class="img-fluid rounded z-depth-1" %}
    <p style="font-size: 12px;" class="text-center">Not-social mobile manipulator transporting an object (RRT*).</p>
  </div>
</div>

To solve the problem in a static environment (people do not move), we employ a Risk-RRT*-based algorithm that considers personal spaces given by [Kirby](https://www.ri.cmu.edu/pub_files/2010/5/rk_thesis.pdf). We succesfully tested our developed algorithm in 
several environments.

<!--
Full videos

- [Experiment 1](https://www.youtube.com/watch?v=lLFQ12lf_go);
- [Experiment 2](https://www.youtube.com/watch?v=c8PtqI2iLMM);
- [Experiment 3](https://www.youtube.com/watch?v=tNo6pqw-BAA).

-->

Currently, we are extending the work in three branches:

- Compare Risk-RRT* with a Reinforcement Learning Approach;
- Online algorithm for 2D environments, where people move;
- Extend to 3D environments. 
