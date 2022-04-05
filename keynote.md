---
layout: default
---

# Keynote talk

## Speaker

{% assign speaker = site.data.keynote.speaker %}
![{{ speaker.name }}]({{ speaker.photo }})

### {{ speaker.courtesy_title }} {{ speaker.name }}, {{ speaker.affiliation }}, {{ speaker.country }}

{{ speaker.bio }}

{% assign talk = site.data.keynote %}
### {{ talk.title }}

{{ talk.abstract }}

