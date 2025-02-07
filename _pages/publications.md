---
layout: archive
title: "Publications"
permalink: /publications/
author_profile: true
---

{% include base_path %}

## Conference Proceedings

{% for paper in site.data.conference %}
- **{{ paper.title }}**  
  *{{ paper.authors }}*  
  _{{ paper.conference }}_  
  [View Paper]({{ paper.link }})
{% endfor %}
