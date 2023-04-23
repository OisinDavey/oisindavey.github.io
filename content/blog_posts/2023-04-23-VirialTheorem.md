---
title: "Virial Theorem dilema"
date: 2023-04-23T10:24:24+01:00
draft: false
tags: ["physics"]
---


In class we learned that the total energy of a two-body system was given by the following:
{{< latex_line tex="E=-\frac{k}{2a}\text{, where $a$ is the semi-major axis}" >}}

When I saw this, I figured that this result followed from the virial theorem based on how it looks vaguely like the half-potential.

The following is taken from the [virial theorem wikipedia page](https://en.wikipedia.org/wiki/Virial_theorem#Special_case_of_power-law_forces):
> For gravitational attraction, n equals −1 and the average kinetic energy equals half of the average negative potential energy:
{{< latex_line tex="\langle T\rangle_\tau=-\frac12\langle V_\text{TOT}\rangle_\tau." >}}

However consider instead this application of the Virial theorem:
> The energy is constant, so the energy equals the average energy.
{{< latex_line tex="E=\langle T+V\rangle=\langle T\rangle+\langle V\rangle=\frac12\langle V\rangle=-\frac12\langle\frac{k}{r}\rangle=-\frac k2\langle\frac{1+e\cos\theta}{\alpha}\rangle=-\frac{k}{2\alpha}\left(\langle1\rangle+e\langle\cos\theta\rangle\right)=-\frac{k}{2\alpha}" >}}
{{< latex_line tex="\text{Where, here, $\alpha$ is the semi-latus rectum}" >}}

These two quantities are only equal for circular orbits, so clearly I'm missunderstanding the usage of the Virial theorem.
It's also possible that I'm misusing the chevrons for averages. Maybe I'm using an arithmetic mean but they're something else?

Any help is appreciated.
