---
layout: default
title: Sobre QA Sampa Meeting
---

<div class="row"><div class="col s12"><h1 class="qasp-title">sobre</h1></div></div>
<div class="divider"></div>
<div class="row">
  <div class="col s12">
    <p class="flow-text text-justify"> O QA Sampa Meeting surgiu da necessidade que sentimos em aprender sobre qualidade de software de forma PRÁTICA, colocando a mão na massa mesmo! </p>

    <p class="flow-text text-justify"> O objetivo é participarmos de workshops com 6 horas, além de dojos, gincanas e hackers QA, com muita mão na massa e nada de palestra!</p>

    <p class="flow-text text-justify"> É uma iniciativa sem fins lucrativos, totalmente GRATUITA, com os seguintes valores: contribuir com a comunidade de qualidade, incentivar/ensinar a busca autodidata de conhecimento e valorizar/fortalecer o papel da qualidade no desenvolvimento de software.</p>

    <p class="flow-text text-justify"> Desta forma, vamos conseguir ter um gostinho e aprender o básico de como executar algumas ferramentas que fazem parte do dia-a-dia dos profissionais que querem garantir a qualidade de um software. </p>

     <p class="flow-text text-justify"> Estes workshops são direcionados para qualquer profissional que trabalhe ou queira aprender sobre qualidade de software e não somente para QAs.</p>
  </div>
</div>

<!-- Sponsors -->
<div class="row white teal-text center-align sponsors">
  <h5><strong>Patrocínio</strong></h5>
  <div class="hide-on-med-and-down">
    <div class="col s12 valign-wrapper center-align sponsors-logos">
      {% for sponsor in site.data.sponsors %}
          <a href="{{ sponsor[1] }}" target="_blank">
            <img style="max-height: 120px;" src="/assets/img/sponsors/{{ sponsor[0] }}.png">
          </a>
      {% endfor %}
    </div>
  </div>
  <div class="hide-on-large-only">
    <div class="col s12 valign-wrapper center-align sponsors-logos-vertical">
      {% for sponsor in site.data.sponsors %}
          <a href="{{ sponsor[1] }}" target="_blank">
            <img style="max-height: 200px;" src="/assets/img/sponsors/{{ sponsor[0] }}.png">
          </a>
      {% endfor %}
    </div>
  </div>
</div>
<!-- END Sponsors -->

<!-- Supporters -->
<div class="row white teal-text center-align supporters">
  <h5><strong>Apoio</strong></h5>
  <div class="hide-on-med-and-down">
    <div class="col s12 valign-wrapper center-align supporters-logos">
      {% for supporter in site.data.supporters %}
          <a href="{{ supporter[1] }}" target="_blank">
            <img style="max-height: 120px;" src="/assets/img/supporters/{{ supporter[0] }}.png">
          </a>
      {% endfor %}
    </div>
  </div>
  <div class="hide-on-large-only">
    <div class="col s12 valign-wrapper center-align supporters-logos-vertical">
      {% for supporter in site.data.supporters %}
          <a href="{{ supporter[1] }}" target="_blank">
            <img style="max-height: 200px;" src="/assets/img/supporters/{{ supporter[0] }}.png">
          </a>
      {% endfor %}
    </div>
  </div>
</div>
<!-- END Supporters -->
