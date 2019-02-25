---
layout: default
title: Palestrantes QA Sampa Meeting
---

<div class="row"><div class="col s12"><h1 class="qasp-title">palestrantes</h1></div></div>
<div class="divider"></div>
<div class="row">
  <div class="col s12 center">
    <h5>Quer ser palestrante também?</h5>
    <a href="https://docs.google.com/forms/d/e/1FAIpQLSfEjY2cHsVzCYVOzAxFKceIFnAYYoqwCSH-SHPCiKmQ1tcbMQ/viewform" target="_blank" class="waves-effect waves-light btn blue lighten-1">
      <i class="material-icons right">lightbulb_outline</i>
      Inscreva-se aqui
    </a>
  </div>
</div>
<div class="row">
{% for speaker in site.data.speakers %}
  <div class="col xl3 l4 s12 qasp-speaker-card">
    <div class="card white grey-text text-darken-4">
      <div class="card-image">
        <a href="{{ speaker[1].link }}" target="_blank">
          <img src="/assets/img/speakers/{{ speaker[1].image }}">
        </a>
      </div>
      <div class="card-content valign-wrapper center-align">
        <span class="card-title center"><a class="blue-text text-lighten-1" href="{{ speaker[1].link }}" target="_blank"><h6>{{ speaker[1].name }}</h6></a></span>
      </div>
    </div>
  </div>
{% endfor %}
</div>
