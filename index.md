---
layout: home
title: QA Sampa Meeting
---

<div id="index-banner" class="parallax-container">
  <div class="section no-pad-bot">
    <div class="container">
      {% assign next_event = site.events.first[1].first %}
      {% assign event_date = next_event.date | split: "-" %}
      <div class="row center">
        <a href="/events" id="download-button" class="btn-large waves-effect waves-light teal lighten-1">
          Próximo evento: {{ event_date.first }} de {{ site.events.first[0] }} de {{ event_date.last }}
        </a>
      </div>
    </div>
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
    {% for speaker in site.speakers limit: 3 %}
      <div class="col s2 hide-on-small-only">
        <div class="card">
          <div class="card-image">
            <a href="/speakers">
              <img src="/assets/img/speakers/{{ speaker.image }}">
            </a>
          </div>
          <div class="card-content center">
            <a href="/speakers">{{ speaker.name }}</a>
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