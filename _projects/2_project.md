---
layout: page
title: 3D Object Representation
description: computational algorithm, application to simulation and robotics
img: 
importance: 2
category: research
related_publications: false
---

3D object representation is an important topic in robotics, simulation, and graphics. Various representation schemes come with trade-offs and are typically designed for specific applications. Our focus is on representations tailored for robotics problems involving contact.

### Shape Abstraction via Differentiable Convex Geometries

Object representations are often derived from raw sensory data, such as images or point clouds, or transformed from dense, unstructured information. Shape abstraction refers to the process of converting these low-level representations into more structured and usable forms. We employ a differentiable convex representation as the foundational unit for this abstraction.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/research/abstraction_examples.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Examples of shape abstraction results using differentiable convex geometries
</div>

The abstraction results can be forwarded to  efficient contact computation algorithm and directly applied to physics simulation, planning, contact localization problems, and more.
<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/research/dsf_computation.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Efficient contact computation algorithm based on a hybrid of optimization and computational geometry.
</div>

### Differentiable Support Function

A key step in simulation and robotics is computing contact features—such as distance, contact points, and normals—from given object representations and poses. The Differentiable Support Function (DSF) is designed to handle a wide range of convex geometries while ensuring the differentiability of these contact features.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/research/dsf_examples.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Examples of geometries represented by differentiable support functions
</div>

Such properties of DSF can be utilized in gradient-based solution of diverse estimation and planning with contact. Here is an example:

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/research/dishplace.gif" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>



