---
layout: default
title: Eventos QA Sampa Meeting
---

<div class="row"><div class="col s12"><h1 class="qasp-title">eventos</h1></div></div>
{% for month_events in site.events %}
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
  <div class="col s12 m6 l4">
    <div class="card white grey-text text-darken-4">
      <div class="card-content">
        <span class="card-title"><h6><strong>{{ event.title }}</strong></h6></span>
        <p>
          {{ event.date }}
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