---
layout: default
title: Eventos QA Sampa Meeting
---

<div class="row"><div class="col s12"><h1 class="qasp-title">eventos</h1></div></div>
{% for month_events in site.data.events %}
<nav class="teal">
  <div class="nav-wrapper">
    <div class="row">
      <div class="col s12">
        <h5>{{ month_events[0] }}</h5>
      </div>
    </div>
  </div>
</nav>
<div class="row">
{% for event in month_events[1] %}
  <div class="col s12 l6 xl4">
    <div class="card white grey-text text-darken-4 qasp-event-card">
      <div class="card-image">
        <img src="/assets/img/events/thumbs/{{ event.image }}" class="responsive-img">
        <span class="card-title flow-text"><strong>{{ event.title }}</strong></span>
      </div>
      <div class="card-content">
        <p class="valign-wrapper">
          <i class="material-icons">today</i>
          {{ event.date | replace: "-", "/" }}
        </p>
        <p class="valign-wrapper">
          <i class="material-icons">person</i>
          <a href="{{ site.data.speakers | map: event.speaker[0] | map: "link" }}" target="_blank">
            {{ site.data.speakers | map: event.speaker[0] | map: "name" }}
          </a>
        </p>
        <p class="valign-wrapper">
          {% if event.speaker[1] %}
            <i class="material-icons">person</i>
            <a href="{{ site.data.speakers | map: event.speaker[1] | map: "link" }}" target="_blank">
            {{ site.data.speakers | map: event.speaker[1] | map: "name" }}
            </a>
          {% else %}
            <br>
          {% endif %}
        </p>
        <p class="valign-wrapper">
          <i class="material-icons">location_on</i>
          {% if event.place.map_link %}
            <a href="{{ event.place.map_link }}" target="_blank">
              {{ event.place.name }}
            </a>
          {% else %}
            {{ event.place.name }}
          {% endif %}
        </p>
      </div>
      <div class="card-action">
        <a href="{{ event.link }}" {% if event.link %}target="_blank"{% endif %} class="waves-effect waves-light btn">
          <i class="material-icons right">lightbulb_outline</i>
          {% if event.link %}inscreva-se aqui{% else %}inscrições em breve{% endif %}
        </a>
      </div>
    </div>
  </div>
{% endfor %}
</div>
{% endfor %}