---
layout: default
---

# Accepted papers

{% for paper in site.data.papers -%}
## {{ paper.title }}

{% comment %}
{% if paper.url %}
URL: {{ paper.url }}
{% endif %}

{% if paper.doi %}
DOI: {{ paper.doi }}
{% endif %}

{% if paper.pdf %}
PDF:

[![PDF](/assets/pdf.png)]({{ paper.pdf }})
{% endif %}

{% if paper.slides %}
Slides:

[![Slides](/assets/slides.png)]({{ paper.slides }})
{% endif %}
{% endcomment %}

**_Authors_**: {{ paper.authors | join: ", " }}

**_Abstract_**: {{ paper.abstract }}

{% endfor %}
