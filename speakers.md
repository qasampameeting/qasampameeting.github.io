---
layout: default
title: Palestrantes QA Sampa Meeting
---

<div class="speakers">
  <h1 class="pageTitle">palestrantes</h1>
  <div class="speakersContent">
    {% for speaker in site.speakers %}
      <div class="speaker">
        <div class="photo">
          <a href="{{ speaker.link }}"><img src="/assets/img/speakers/{{ speaker.image }}"></a>
        </div>
        <div class="text">
          <h5>
            <a href="{{ speaker.link }}">{{ speaker.name }}</a>
          </h5>
          <div class="description">
            {{ speaker.description }}
          </div>
        </div>
      </div>
    {% endfor %}
  </div>
</div>
