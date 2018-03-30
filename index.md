---
layout: default
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

<div class="home" id="home">
  <div class="home-about">
    <div class="container">
      <div class="title">sobre</div>
      <div class="description">
        <div class="text">Evento para profissionais que desejam aprender sobre Qualidade de Software</div>
        <div class="photo"><a href="/about"><img src="/assets/img/home-about.jpg"></a></div>
      </div>
      <a class="more" href="/about">Saiba mais</a>
    </div>
  </div>

  <div class="home-speakers">
    <div class="container">
      <div class="title">palestrantes</div>
      <div class="description">
        <div class="text">Estas serão nossas inspirações para os próximos eventos</div>
        <div class="cards">
          {% for speaker in site.speakers limit: 3 %}
            <div class="speaker">
              <div class="photo">
                <a href="/speakers"><img src="/assets/img/speakers/{{ speaker.image }}"></a>
              </div>
              <div class="name">
                <a href="/speakers">{{ speaker.name }}</a>
              </div>
            </div>
          {% endfor %}
        </div>
      </div>
      <a class="more" href="/speakers">Saiba mais</a>
    </div>
  </div>

  <div class="home-events">
    <div class="container">
      <div class="title">eventos</div>
      <div class="description">
        <div class="text">Confira nossa agenda de eventos</div>
      </div>
      <a class="more" href="/events">Saiba mais</a>
    </div>
  </div>
</div>
