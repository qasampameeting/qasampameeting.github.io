---
layout: default
title: Eventos QA Sampa Meeting
---

<div class="events">
  <h1 class="pageTitle">eventos</h1>
  <div class="events-content">
    {% for month_events in site.events %}
      <div class="title">
        <div>{{ month_events[0] }}</div>
      </div>
      {% for event in month_events[1] %}
        <div class="description">
          {{ event.date }}<br/>
          "{{ event.title }}"
        </div>
        <div class="event-link">
          <a href="{{ event.link }}" {% if event.link %}target="_blank"{% endif %}>{% if event.link %}inscreva-se aqui{% else %}inscrições em breve{% endif %}</a>
        </div>
      {% endfor %}
    {% endfor %}
  </div>
</div>
