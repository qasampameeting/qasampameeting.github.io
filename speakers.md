---
layout: default
title: Palestrantes QA Sampa Meeting
---

<div class="row"><div class="col s12"><h1 class="qasp-title">palestrantes</h1></div></div>
<div class="divider"></div>
<div class="row">
  <div class="col s12 center">
    <h5>Quer ser palestrante também?</h5>
    <a href="https://qasampameeting.typeform.com/to/Qxo6rT" target="_blank" class="waves-effect waves-light btn">
      <i class="material-icons right">lightbulb_outline</i>
      Inscreva-se aqui
    </a>
  </div>
</div>
<div class="row">
{% for speaker in site.data.speakers %}
  <div class="col m3 s12">
    <div class="card white grey-text text-darken-4">
      <div class="card-image">
        <a href="{{ speaker.link }}" target="_blank">
          <img src="/assets/img/speakers/{{ speaker.image }}">
        </a>
      </div>
      <div class="card-content">
        <span class="card-title center"><a class="teal-text" href="{{ speaker.link }}" target="_blank"><h6>{{ speaker.name }}</h6></a></span>
      </div>
    </div>
  </div>
{% endfor %}
