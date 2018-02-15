---
layout: default
title: Palestrantes QA Sampa Meeting
---

<div class="speakers">
  <h1 class="pageTitle">palestrantes</h1>
  <div class="speakers-content">
    {% for speaker in site.speakers %}
      <div class="speaker">
        <div class="photo">
          <a href="{{ speaker.link }}" target="_blank"><img src="/assets/img/speakers/{{ speaker.image }}"></a>
        </div>
        <div class="text">
          <h5>
            <a href="{{ speaker.link }}" target="_blank">{{ speaker.name }}</a>
          </h5>
          <div class="description">
            {{ speaker.description }}
          </div>
        </div>
      </div>
    {% endfor %}
  </div>
  <div class="call-for-papers">
    <p>Quer ser palestrante também?</p>
    <a href="https://qasampameeting.typeform.com/to/Qxo6rT" target="_blank">Inscreva-se aqui</a>
  </div>
</div>
