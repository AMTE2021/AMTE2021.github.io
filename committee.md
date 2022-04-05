---
layout: default
---

# Organizing Committee

{% for member in site.data.organizing_committee -%}
* {{ member.name }}, {{ member.affiliation }}, {{ member.country }}
{% endfor %}

# Program Committee 

{% for member in site.data.program_committee -%}
* {{ member.name }}, {{ member.affiliation }}, {{ member.country }}
{% endfor %}
