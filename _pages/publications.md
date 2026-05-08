---
layout: archive
title: "Publications"
permalink: /publications/
author_profile: true
---

{% include base_path %}

## Journal Articles

{% for paper in site.data.journals %}
- **{{ paper.title }}**  
  *{{ paper.authors }}*  
  _{{ paper.venue }}_, {{ paper.year }}{% if paper.ieee_url %}. [IEEE Xplore]({{ paper.ieee_url }}){% endif %}{% if paper.arxiv_id %}. [arXiv:{{ paper.arxiv_id }}](https://arxiv.org/abs/{{ paper.arxiv_id }}){% endif %}
{% endfor %}


## Preprints

{% for paper in site.data.preprints %}
- **{{ paper.title }}**  
  *{{ paper.authors }}*  
  _{{ paper.venue }}_, {{ paper.year }}{% if paper.arxiv_id %}. [arXiv:{{ paper.arxiv_id }}](https://arxiv.org/abs/{{ paper.arxiv_id }}){% endif %}
{% endfor %}


## Conference Proceedings

{% for paper in site.data.conference %}
- **{{ paper.title }}**  
  *{{ paper.authors }}*  
  _{{ paper.conference }}_  
{% endfor %}
