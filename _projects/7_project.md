---
layout: page
title: DOP Related
description: Problems proposed related to the Dubins Orienteering Problem.
importance: 2
img: assets/img/dop_example.png
category: current
---
We proposed the [Variable-Speed Dubins Orienteering Problem](https://ieeexplore.ieee.org/document/10786481) and *Varying Rewards Dubins Orienteering Problem*.

The [Dubins Orienteering Problem (DOP)](https://ieeexplore.ieee.org/document/7847413) is based on the Orienteering Problem (OP) but considering non-holonomic vehicles. In the DOP we want to compute trajectories for a vehicle with curvature constraints, in which he needs to visit a subset of locations, where each location has a different reward. The objective is to maximize the amount of rewards collected within a given limited budget, being usually time or distance. 
<!--Imagine a game where you are in a kart and need to grab flags, each flag has a different score (previously known) and you only have 30 seconds, meaning you can't grab all flags but you need to get the maximum score possible.
-->

<div class="row justify-content-sm-center">
  <div class="col-sm-8 mt-3 mt-md-0">
    {% include figure.liquid path="assets/img/dop_example.png" title="example image" class="img-fluid rounded z-depth-1" %}
  </div>
  <p style="font-size: 12px;" class="text-center"> Illustrative example of the best computed trajectory for a VS-DOP instance with 30 vertices. Each vertex is assigned a unique reward, and the trajectory is optimized to vary the vehicle’s velocity to maximize the total rewards collected.
</p>
</div>

We proposed the *Variable-Speed Dubins Orienteering Problem* (VS-DOP) where we consider that the vehicle can change its speed during the trajectory, different from the original problem, which considers constant speed. We shown that the VS-DOP outputs better results than compared to the DOP, even if the velocity is maximum at all times. 

Our paper about the VS-DOP can be found [here](https://ieeexplore.ieee.org/document/10786481).

Currently, we are working on the VS-DOP with rewards that change over time. This means one must consider not only the positions but also the timing of reward collection to maximize the total rewards obtained.
<!-- We already tested this formulation without varying velocity using Genetic Algorithms but it didn't give a big impact. -->





