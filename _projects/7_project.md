---
layout: page
title: DOP Related
description: Problems proposed related to the Dubins Orienteering Problem.
importance: 2
img: assets/img/dop_example.png
category: current
---

The Dubins Orienteering Problem (DOP) is based on the Orienteering Problem (OP) but considering non-holonomic vehicles, such as fixed-wings drones. The OP is similar to the Travelling Salesman Problem (TSP) combined with the Knapsack.

In the DOP we want to compute trajectories for a vehicle with curvature constraints, in which he needs to visit a subset of locations provided, where each location has a different reward. The objective is to maximize the amount of rewards collected within a given limited budget, being usually time or distance. Imagine a game where you are in a kart and need to grab flags, each flag has a different score (previously known) and you only have 30 seconds, meaning you can't grab all flags but you need to get the maximum score possible.

<div class="row justify-content-sm-center">
  <div class="col-sm-8 mt-3 mt-md-0">
    {% include figure.liquid path="assets/img/dop_example.png" title="example image" class="img-fluid rounded z-depth-1" %}
  </div>
  <p style="font-size: 12px;" class="text-center"> Illustrative example of the best computed trajectory for a VS-DOP instance with 30 vertices. Each vertex is assigned a unique reward, and the trajectory is optimized to vary the vehicle’s velocity to maximize the total rewards collected.
</p>
</div>

We recently proposed the Variable-Speed Dubins Orienteering Problem (VS-DOP) where we consider that the vehicle can change its speed during the trajectory, different from the original problem, which considers constant speed. We shown that the VS-DOP outputs better results than compared to the DOP, even if the velocity is maximum at all times. The paper was sent and we are waiting for the result.

Currently we want to work on the VS-DOP with the rewards changing in time, meaning that ones need to consider not only the positions but also in what time you are collecting the reward, to be able to maximize the amount of rewards collected. We already tested this formulation without varying velocity using Genetic Algorithms but it didn't give a big impact. Right now, we are studing applying the variying speed and trying new approaches to solving the new proposed problem..





