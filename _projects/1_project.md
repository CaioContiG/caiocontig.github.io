---
layout: page
title: UGV/UAV Cooperation
description: Collaborative Unmanned Ground and Aerial vehicles Path Planning for Inventory Management in Warehouses.
img: assets/img/12.jpg
importance: 1
category: work
related_publications: einstein1956investigations, einstein1950meaning
---
This project served as my final paper for graduation and got maximum grade for it. It led to a [publication](https://ieeexplore.ieee.org/document/9995748) entitled Collaborative UGV/UAV Path Planning for Inventory Management in Warehouses and received an award as one of the top 15 best papers at the [conference](https://fei.edu.br/robotica/lars-sbr/).

In this research we considered a collaborative system where one ground vehicle transports one aerial vehicle to certain spots in an warehouse, in those spots the aerial takes off and visit shelves nearby. The objective was to develop a technique to model this problem considering energy-limitations from both vehicles, becoming a maximization problem to visit most shelves possible considering the energy restriction. We modelled based on the Orienteering Problem and solved using a hybrid algorithm between Genetic Algorithm and a Greddy one.

## Abstract
The use of autonomous mobile robots in different applications has increased significantly over the past years, which can be executed individually or collaboratively, considering the use of Multi-Robot Systems (MRS), that presents several advantages but also raises many challenges. Specifically, when considering heterogeneous robots, it is paramount to develop techniques that respect individual restrictions and benefit the use of their different capabilities. In this paper, we consider a ground/aerial collaboration for inventory inspection in warehouse environments. The goal is to determine a set of optimized combined paths that maximize the number of shelves inspected. The problem is formulated as a dual Orienteering Problem (OP), where the budget of both vehicles is considered, and the rewards, which are related to the shelves that can be visited, are estimated by a greedy strategy. Results in simulated scenarios considering different aspects provide a thorough evaluation and validation of the methodology.

To give your project a background in the portfolio page, just add the img tag to the front matter like so:

    ---
    layout: page
    title: project
    description: a project with a background image
    img: /assets/img/12.jpg
    ---

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/1.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/3.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/5.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Caption photos easily. On the left, a road goes through a tunnel. Middle, leaves artistically fall in a hipster photoshoot. Right, in another hipster photoshoot, a lumberjack grasps a handful of pine needles.
</div>
<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/5.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    This image can also have a caption. It's like magic.
</div>

You can also put regular text between your rows of images.
Say you wanted to write a little bit about your project before you posted the rest of the images.
You describe how you toiled, sweated, *bled* for your project, and then... you reveal its glory in the next row of images.


<div class="row justify-content-sm-center">
    <div class="col-sm-8 mt-3 mt-md-0">
        {% include figure.html path="assets/img/6.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm-4 mt-3 mt-md-0">
        {% include figure.html path="assets/img/11.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    You can also have artistically styled 2/3 + 1/3 images, like these.
</div>


The code is simple.
Just wrap your images with `<div class="col-sm">` and place them inside `<div class="row">` (read more about the <a href="https://getbootstrap.com/docs/4.4/layout/grid/">Bootstrap Grid</a> system).
To make images responsive, add `img-fluid` class to each; for rounded corners and shadows use `rounded` and `z-depth-1` classes.
Here's the code for the last row of images above:

{% raw %}
```html
<div class="row justify-content-sm-center">
    <div class="col-sm-8 mt-3 mt-md-0">
        {% include figure.html path="assets/img/6.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm-4 mt-3 mt-md-0">
        {% include figure.html path="assets/img/11.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
```
{% endraw %}
