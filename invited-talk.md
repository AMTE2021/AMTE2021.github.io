---
layout: default
---

# Invited talk

## Speaker

{% assign speaker = site.data.invited_talk.speaker %}
![{{ speaker.name }}]({{ speaker.photo }})

### {{ speaker.courtesy_title }} {{ speaker.name }}, {{ speaker.affiliation }}, {{ speaker.country }}

{{ speaker.bio }}

{% assign talk = site.data.invited_talk %}
### {{ talk.title }}

{{ talk.abstract }}