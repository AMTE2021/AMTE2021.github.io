---
layout: default
---

# Panel

## Moderator

{% assign mod = site.data.panel.moderator %}
* {{ mod.name }}, {{ mod.affiliation }}, {{ mod.country }}

## Panelists

{% for panelist in site.data.panel.panelists -%}
* {{ panelist.name }}, {{ panelist.affiliation }}, {{ panelist.country }}
{% endfor %}

## Panel's chosen questions

{% for question in site.data.panel.questions %}
* {{ question.q }}
    {%- if question.followups -%}
    {% for followup in question.followups %}
    * {{ followup }}
    {%- endfor -%}
    {%- endif -%}
{% endfor %}

## Outline

{% for item in site.data.panel.outline %}
* {{ item }}
{%- endfor -%}
