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
- **{{ item.date }}** – {% if item.url %}{{ item.title | replace: "arXiv", "<a href='" | append: item.url | append: "'>arXiv</a>" }}{% else %}{{ item.title }}{% endif %}
{% endfor %}


<!-- Ollie at the bottom of the page content -->
<style>
  .ollie-wrapper {
    text-align: center;
    margin-top: 4rem;   /* space above Ollie */
    margin-bottom: 0.5rem;
  }
</style>

<div class="ollie-wrapper">
  <img src="/images/ollie.jpg" alt="Ollie!" style="width: 200px; height: auto;" />
</div>
