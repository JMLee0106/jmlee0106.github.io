---
layout: page
title: Contact Manipulation
description: estimation, planning, and control through contact
img:
importance: 3
category: research
related_publications: false
---

Contact manipulation is an rising topic in robotics that involves solving various *inverse* problems related to contact. Our focus is on developing efficient and scalable methods for these problems, leveraging model-based optimization, sampling techniques, and integrating data-driven approaches.

### Contact Factor Graph

Graphical modeling is widely used to represent problems in a structured manner with a stochastic perspective. The Contact Factor Graph (CFG) framework enables versatile reasoning about contact interactions between objects through differentiable, compositional factor modeling and an efficient gradient-based inference algorithm.

Here is a simple illustrative example:
<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/research/cfg_overall.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/research/cfg_stack.gif" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Finding the distribution of stable placement configuration using CFG framework
</div>

### Shaping Solution Landscape

An often overlooked perspective in model-based approaches is the impact of a well-designed model on the entire solution process. A good model is not solely about accuracy; it also shapes a problem landscape that is easier to solve, guiding towards reasonable solutions more efficiently. We are exploring techniques to adapt models into "easier-to-solve" forms to address challenging problems. A notable example is homotopy-based narrow passage robot planning, which incrementally transforms the environment model.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/research/narrow.gif" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>