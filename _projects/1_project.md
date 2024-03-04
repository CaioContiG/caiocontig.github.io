---
layout: page
title: UGV/UAV Path-Planning
description: Collaborative Unmanned Ground and Aerial vehicles Path Planning for Inventory Management in Warehouses.
img: assets/img/ugv_uav.png
importance: 1
#category: work
---
The project served as my final paper for graduation and got maximum grade for it. It led to a [publication](https://ieeexplore.ieee.org/document/9995748) entitled Collaborative UGV/UAV Path Planning for Inventory Management in Warehouses and received an award as one of the top 15 best papers at the [conference](https://fei.edu.br/robotica/lars-sbr/).

<div class="row justify-content-sm-center">
  <div class="col">
    {% include figure.liquid path="assets/img/ugv_uav_copp1.svg" title="example image" class="img-fluid rounded z-depth-1" %}
  </div>
    <div class="col">
    {% include figure.liquid path="assets/img/ugv_uav_copp2.svg" title="example image" class="img-fluid rounded z-depth-1" %}
  </div>
    <div class="col">
    {% include figure.liquid path="assets/img/ugv_uav_copp3.svg" title="example image" class="img-fluid rounded z-depth-1" %}
  </div>
  <p style="font-size: 12px;" class="text-center"> On the left, ground vehicle carries aerial vehicle. Middle, shows ground vehicle path with blue arrows and its stops in red circles. Right, shows the aerial vehicle path in one stop with red arrows, blue circles the shelves he need to visit. 
</p>
</div>

In this research we considered a collaborative system where one unmanned ground vehicle (UGV) transports one unmanned aerial vehicle (UAV) to certain spots in an warehouse, in those spots the aerial takes off and visit shelves nearby. The objective was to develop a technique to model this problem considering energy-limitations from both vehicles. The problem becomes a maximization problem to visit most shelves possible considering the energy restriction. We modelled based on the Orienteering Problem and solved using a hybrid algorithm between Genetic Algorithm and a Greddy one.


<div class="row justify-content-sm-center">
  <div class="col-sm-8 mt-3 mt-md-0">
    {% include figure.liquid path="assets/img/ugv_uav.png" title="example image" class="img-fluid rounded z-depth-1" %}
  </div>
  <p style="font-size: 12px;" class="text-center"> One possible solution encountered by our algorithm. Red circles are nodes where the ground vehicle stops, numbered by order of stopping. Red squares are shelves we want to visit, while the
small black squares are shelves we don't want to visit. Blue arrows are the path made by the ground vehicle. Red arrows the paths made by the aerial vehicle in each stop. Small black circles are aisle nodes where the robot is free to move but it will not stop there.  
</p>
</div>



## Abstract
The use of autonomous mobile robots in different applications has increased significantly over the past years, which can be executed individually or collaboratively, considering the use of Multi-Robot Systems (MRS), that presents several advantages but also raises many challenges. Specifically, when considering heterogeneous robots, it is paramount to develop techniques that respect individual restrictions and benefit the use of their different capabilities. In this paper, we consider a ground/aerial collaboration for inventory inspection in warehouse environments. The goal is to determine a set of optimized combined paths that maximize the number of shelves inspected. The problem is formulated as a dual Orienteering Problem (OP), where the budget of both vehicles is considered, and the rewards, which are related to the shelves that can be visited, are estimated by a greedy strategy. Results in simulated scenarios considering different aspects provide a thorough evaluation and validation of the methodology.
