---
layout: default
title: Equipe QA Sampa Meeting
---

<div class="row"><div class="col s12"><h1 class="qasp-title">equipe</h1></div></div>
<div class="divider"></div>
<div class="row">
  {% for member in site.team %}
  <div class="col s12 m6 l4 xl3">
    <div class="card white grey-text text-darken-4">
      <div class="card-image">
        <a href="{{ member.link }}" target="_blank">
          <img src="/assets/img/team/{{ member.image }}">
        </a>
      </div>
      <div class="card-content center">
        <span class="card-title center"><strong><a class="teal-text" href="{{ member.link }}" target="_blank">{{ member.name }}</a></strong></span>
        <p>{{ member.role }}</p>
        <p><a href="{{ member.link }}" target="_blank">{{ member.link_text }}</a></p>
      </div>
    </div>
  </div>
  {% endfor %}
</div>
