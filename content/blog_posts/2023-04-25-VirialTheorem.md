---
title: "Virial Theorem Dilema (Resolution)"
date: 2023-04-25T10:07:30+01:00
draft: false
tags: ["physics"]
---

### Resolution of problem posed

[Problem statement.](/blog_posts/2023-04-23-virialtheorem)

Many thanks to Dr. Paul Watts for helping me out with this.

The key to this problem was, as I suspected, that I was misinterpretting the chevrons.

Specifically, this assertion is wrong:
{{< latex_line tex="e\langle\cos\theta\rangle=0" >}}

Here, I saw that we were averaging a cosine function over a whole period, and took it to therefore be zero. What I failed to consider, however, was that the argument does _not_ scale linearly with time, why should it! (Unless it were a circle). If one writes the argument in terms of time, the average gives the expected answer.
