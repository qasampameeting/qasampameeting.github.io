---
layout: default
title: Equipe QA Sampa Meeting
---

<div class="row"><div class="col s12"><h1 class="qasp-title">equipe</h1></div></div>
<div class="divider"></div>
<div class="row">
  {% for member in site.data.team %}
  <div class="col s12 m6 l4">
    <div class="card white grey-text text-darken-4">
      <div class="card-image">
        <a href="{{ member.link }}" target="_blank">
          <img src="/assets/img/team/{{ member.image }}">
        </a>
      </div>
      <div class="card-content center">
        <span class="card-title center"><strong><a class="blue-text text-lighten-1" href="{{ member.link }}" target="_blank">{{ member.name }}</a></strong></span>
        <p><a href="{{ member.link }}" target="_blank">{{ member.link_text }}</a></p>
      </div>
    </div>
  </div>
  {% endfor %}
</div>
