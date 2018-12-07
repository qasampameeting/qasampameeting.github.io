---
layout: home
title: QA Sampa Meeting
---

<div id="index-banner" class="parallax-container">
  <div class="section no-pad-bot">
    {% if site.data.events %}
      <div class="container">
        {% assign next_event = site.data.events.first[1].first %}
        <div class="row center">
          <a href="/events" id="download-button" class="btn-large waves-effect waves-light teal lighten-1">
            <i class="material-icons left">today</i>
            Próximo evento: {{ next_event.date | replace: "-", "/" }}
          </a>
        </div>
      </div>
    {% endif %}
  </div>
  <div class="parallax"><img src="assets/img/folks.jpg" alt="Unsplashed background img 1" style="transform: translate3d(-50%, 326.131px, 0px); opacity: 1;"></div>
</div>

<div class="container">
  <!-- ABOUT -->
  <div class="row">
    <div class="col s12"><h3><strong>sobre</strong></h3></div>
  </div>
  <div class="row">
    <div class="col s12 m6">
      <p class="flow-text">Evento para profissionais que desejam aprender sobre Qualidade de Software</p>
      <a href="/about" class="waves-effect waves-light btn"><i class="material-icons right">add</i>Saiba mais</a>
    </div>
    <div class="col s6 center hide-on-small-only">
      <a href="/about"><img src="/assets/img/home-about.jpg"></a>
    </div>
  </div>
  <div class="divider"></div>

  <!-- SPEAKERS -->
  <div class="row">
    <div class="col s12"><h3><strong>palestrantes</strong></h3></div>
  </div>
  <div class="row">
    <div class="col s12 m6">
      <p class="flow-text">Estas serão nossas inspirações para os próximos eventos</p>
      <a href="/speakers" class="waves-effect waves-light btn"><i class="material-icons right">add</i>Saiba mais</a>
    </div>
    {% for speaker in site.data.speakers limit: 3 %}
      <div class="col s2 hide-on-small-only">
        <div class="qasp-home-speaker-card card">
          <div class="card-image">
            <a href="/speakers">
              <img src="/assets/img/speakers/{{ speaker[1].image }}">
            </a>
          </div>
          <div class="card-content valign-wrapper">
            <a href="/speakers" class="teal-text">{{ speaker[1].name }}</a>
          </div>
        </div>
      </div>
    {% endfor %}
  </div>
  <div class="divider"></div>

  <!-- EVENTS -->
  <div class="row">
    <div class="col s12"><h3><strong>eventos</strong></h3></div>
  </div>
  <div class="row">
    <div class="col s12 m6">
      <p class="flow-text">Confira nossa agenda de eventos</p>
      <a href="/events" class="waves-effect waves-light btn"><i class="material-icons right">add</i>Saiba mais</a>
    </div>
  </div>
</div>