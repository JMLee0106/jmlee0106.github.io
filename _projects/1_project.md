---
layout: page
title: Robotic Simulation
description: dynamics & contact modeling, numerical solver, sim2real
img:
importance: 1
category: research
related_publications: false
---

Physics simulation is a fundamental tool for advancing robotic intelligence, enabling scalable data acquisition, training, and safe algorithm testing. 
A key challenge is achieving simulations that are both accurate and computationally efficient. 
Our focus involves various aspects like discrete-time dynamics, geometric and physical constraints, friction modeling, system sparsity, and efficient numerical algorithms.

### Variations of Augmented Lagrangian

The Augmented Lagrangian tackles constrained convex optimization by sequentially solving a series of subproblems. We extend this approach to handle robotic simulations involving contact. The first variation, Cascaded Newton-Based Augmented Lagrangian (CANAL), effectively handles multi-contact nonlinear complementarity conditions with high accuracy. This approach is particularly suited for contact-intensive manipulation tasks:
<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/research/canal.gif" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Boltnut assembly (left) and dish piling (right) simulation
</div>
The second variation, Subsystem-Based Alternating Direction Method of Multipliers (SubADMM), efficiently handles high-degree-of-freedom multibody dynamics with numerous constraints in a fast and scalable manner. Its inherently parallel computational structure is also well-suited for GPUs.
<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/research/subadmm.gif" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Particle pouring (left) and multibody haptic (right) simulation
</div>

### Contact Nodalization and Diagonalization

While deformable objects are generally considered challenging to simulate, they also have aspects that are simpler compared to rigid objects. For example, their higher degrees-of-freedom provide a larger feasible space, and constraints come in sparse and simple forms. Contact Nodalization and Diagonalization (COND) is designed to exploit these properties to enable real-time robotic simulation with deformable objects.
<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/research/cable.gif" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/research/softgrip.gif" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>

