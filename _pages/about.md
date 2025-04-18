---
permalink: /
title: ""
excerpt: "About me"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

I'm a PhD Candidate in ECE department at the University of Michigan, co-advised by [Prof. Yun Jiang](https://medicine.umich.edu/dept/radiology/yun-jiang-phd) and [Prof. Jeffrey A. Fessler](https://web.eecs.umich.edu/~fessler/). My current research focuses on accelerated MRI reconstruction using self‑supervised deep learning methods. I’m also interested in quantitative MRI, sampling‑trajectory optimization, and more generally other inverse problems in signal processing. Outside of research, I enjoy (gravel) cycling, tennis, and road trips.

### News

{% for item in site.data.news %}
- **{{ item.date }}** – {% if item.url %}[{{ item.title }}]({{ item.url }}){% else %}{{ item.title }}{% endif %}
{% endfor %}

<!-- Ollie's image fixed at the bottom of the viewport -->
<div style="position: fixed; bottom: 0; left: 50%; transform: translateX(-50%); z-index: 100;">
  <img src="/images/ollie.jpg" alt="Ollie!" style="width: 200px; height: auto;" />
</div>
