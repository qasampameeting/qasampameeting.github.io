---
layout: default
title: QA Sampa Meeting
---

<div class="home" id="home">
  <div class="next-event">
    <div class="container">
      <div class="call">Próximo evento</div>
      {% assign next_event = site.events.first[1].first %}
      <div class="event-title">{{ next_event.title }}</div>
        {% assign event_date = next_event.date | split: "-" %}
      <div class="date">
        <a href="/events">{{ event_date.first }} de {{ site.events.first[0] }} de {{ event_date.last }}</a>
      </div>
    </div>
  </div>

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
