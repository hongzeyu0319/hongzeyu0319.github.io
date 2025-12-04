---
permalink: /
title: ""
excerpt: "About me"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

I'm a PhD Candidate in ECE department at the University of Michigan, co-advised by [Prof. Yun Jiang](https://miitt-mri-jianglab.github.io/) and [Prof. Jeffrey A. Fessler](https://web.eecs.umich.edu/~fessler/). My research focuses on optimization and machine learning for inverse problems in medical imaging, with an emphasis on accelerated and quantitative MRI. In particular, I work on implicit neural representation and score-based diffusion models that combine MRI physics with deep learning priors. Outside of research, I enjoy (gravel) cycling, tennis, and photography.
### News

{% for item in site.data.news %}
- **{{ item.date }}** – {% if item.url %}[{{ item.title }}]({{ item.url }}){% else %}{{ item.title }}{% endif %}
{% endfor %}


<!-- Ollie: fixed at bottom on desktop, inline at bottom on small screens -->
<style>
  /* Give the main content some breathing room so Ollie doesn't cover it */
  .page__content {
    padding-bottom: 220px; /* roughly Ollie’s height */
  }

  .ollie-wrapper {
    position: fixed;
    bottom: 0;
    left: 50%;
    transform: translateX(-50%);
    z-index: 100;
  }

  /* On small screens: make Ollie normal, not fixed */
  @media (max-width: 768px) {
    .ollie-wrapper {
      position: static;
      transform: none;
      text-align: center;
      margin-top: 2rem;
    }
    .page__content {
      padding-bottom: 0;
    }
  }
</style>

<div class="ollie-wrapper">
  <img src="/images/ollie.jpg" alt="Ollie!" style="width: 200px; height: auto;" />
</div>
