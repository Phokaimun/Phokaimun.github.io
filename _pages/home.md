---
layout: splash
permalink: /
---

<div class="feature__wrapper">
  {% for event in site.data.events %}
    {% include event_card.html
      title=event.title
      date=event.date
      location=event.location
      description=event.description
    %}
  {% endfor %}
</div>
