---
title: "Gravity Simulator"
date: 2023-04-22T17:54:42+01:00
draft: false
---

I decided to try adding some moving things to this site to make it more of a quasi-static site.

I've added a new section called simulations; a very ambitious action, as though I intend to add more than what's in there (I'm not sure that I do). Nonetheless, it has a little p5 js canvas thing I made that allows the user to play around with little planets, and see if they can get a stable solution for the 3 body problem!

In terms of the actual implementation, I decided to go with the straightforward approach.

The processing is split up into timesteps, and the positions and veclocities are updated on a first-order basis like so:

{{< latex_line tex = "\Delta \vec{r}_i=\vec{v}_i\Delta t" >}}
{{< latex_line tex = "\Delta \vec{v}_i=\sum_{j} \frac{m_j}{\left|\vec{r}_j-\vec{r}_i\right|^3}(\vec{r}_j-\vec{r}_i)\Delta t" >}}

Notably: This introduces chaos into hypothetically stable systems. Also, the timesteps are _not_ all of equal duration, although I'm not clever enough to know what specific problems that introduces. p5 js doesn't seem to allow mobile use? i don't know if that's actually true or maybe I didn't do it right; who knows? The site actually totally breaks for mobile users accessing the page so I've tried to block it for them.

[Anyway here it is!](/simulators/newtonian_gravity)


Also minor update, I got latex working!! So here are Maxwell's equations:

{{< latex_line tex = "\nabla\cdot\vec{E}=\frac{\rho}{\varepsilon_0}" >}}
{{< latex_line tex = "\nabla\cdot\vec{B}=0" >}}
{{< latex_line tex = "\nabla\times\vec{E}=-\frac{\partial\vec{B}}{\partial t}" >}}
{{< latex_line tex = "\nabla\times\vec{B}=\frac{1}{c^2}\frac{\partial\vec{E}}{\partial t}-\mu_0\vec{J}" >}}
