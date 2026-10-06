---
title: Events
permalink: /events/
redirect_from:
  - /events.html
excerpt: Seminars, workshops and conversations hosted by the Business AI and Analytics Centre.
---

The Centre convenes talks, seminars and workshops to share research and exchange perspectives on artificial intelligence, analytics and business.

## Upcoming events

<div class="baiac-grid baiac-grid--events">
  {% for event in site.data.events.upcoming %}
  <article class="baiac-card baiac-event-card">
    <p class="baiac-card__label">{% if event.placeholder %}Example placeholder{% else %}Upcoming event{% endif %}</p>
    <h2>{{ event.title | escape }}</h2>
    {% if event.date != empty %}<p class="baiac-event-card__meta">{{ event.date | escape }}</p>{% endif %}
    {% if event.location != empty %}<p class="baiac-event-card__meta">{{ event.location | escape }}</p>{% endif %}
    <p>{{ event.description | escape }}</p>
    {% if event.url != empty %}<p><a class="text-link" href="{{ event.url | escape }}" target="_blank" rel="noopener noreferrer">Learn More <span aria-hidden="true">↗</span></a></p>{% endif %}
  </article>
  {% endfor %}
</div>

## Past events

<div class="baiac-grid baiac-grid--events">
  {% for event in site.data.events.past %}
  <article class="baiac-card baiac-event-card">
    <p class="baiac-card__label">{% if event.placeholder %}Example placeholder{% else %}Past event{% endif %}</p>
    <h2>{{ event.title | escape }}</h2>
    {% if event.date != empty %}<p class="baiac-event-card__meta">{{ event.date | escape }}</p>{% endif %}
    {% if event.location != empty %}<p class="baiac-event-card__meta">{{ event.location | escape }}</p>{% endif %}
    <p>{{ event.description | escape }}</p>
    {% if event.url != empty %}<p><a class="text-link" href="{{ event.url | escape }}" target="_blank" rel="noopener noreferrer">Conference details <span aria-hidden="true">↗</span></a></p>{% endif %}
  </article>
  {% endfor %}
</div>

<p class="baiac-note">The cards marked “Example placeholder” are prompts for site editors, not scheduled or completed events. Replace them with confirmed details or remove them when the programme is updated.</p>
