---
layout: default
title: Eventos QA Sampa Meeting
---

<div class="events">
  <h1 class="pageTitle">eventos</h1>
  <div class="eventsContent">
    {% for event in site.events %}
      <div class="title">
        <div>{{ event[0] }}</div>
      </div>
      <div class="description">
        {{ event[1].date }}<br/>
        "{{ event[1].title }}"
      </div>
      <div class="eventLink">
        <a href="{{ event[1].link }}">{% if event[1].link %}inscreva-se aqui{% else %}inscrições em breve{% endif %}</a>
      </div>
    {% endfor %}
  </div>
</div>
