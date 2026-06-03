---
layout: page
title: TriSplat
description: Simulation-ready feed-forward 3D scene reconstruction
img: assets/img/trisplat-pipeline.png
importance: 1
related_publications: true
---

TriSplat is a framework for simulation-ready 3D scene reconstruction from sparse unposed images. It converts 3D Gaussian-style point representations into oriented triangular surfels, allowing reconstructed scenes to be exported as meshes and used in downstream simulation environments.

My work focused on stable training for native triangular surfel representations. I designed and implemented strategies including normal warm-up, validity masking, opacity scheduling, and ambiguity annealing to reduce early orientation noise, insufficient coverage, and surface divergence.

I also helped connect reconstruction outputs to Unity and NVIDIA Isaac Sim, enabling collision handling, rigid-body dynamics, robotic grasping, and embodied AI simulation tasks.

<div class="row justify-content-sm-center">
  <div class="col-sm-10 mt-3 mt-md-0">
    {% include figure.liquid loading="eager" path="assets/img/trisplat-pipeline.png" title="TriSplat pipeline" class="img-fluid rounded z-depth-1" %}
  </div>
</div>
<div class="caption">
  TriSplat pipeline overview from the public project page.
</div>

Links: [paper](https://arxiv.org/abs/2605.26115), [project page](https://lhmd.top/trisplat/), [code](https://github.com/ziplab/TriSplat).
