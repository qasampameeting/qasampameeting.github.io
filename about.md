---
layout: default
title: Sobre QA Sampa Meeting
---

<div class="container">
  <!-- ABOUT -->
  <div class="row"><div class="col s12"><h1 class="qasp-title">sobre</h1></div></div>
  <div class="divider"></div>
  <div class="row">
    <div class="col m8 s12">
      <p class="flow-text text-justify"> O QA Sampa Meeting surgiu da necessidade que sentimos em aprender sobre qualidade de software de forma PRÁTICA, colocando a mão na massa mesmo! </p>

      <p class="flow-text text-justify"> O objetivo não é assistir uma palestra, mas sim participarmos de workshops com 30minutos de teoria e 2 horas de hands on pra treinarmos e tirarmos nossas dúvidas. </p>

      <p class="flow-text text-justify"> É uma iniciativa sem fins lucrativos, totalmente GRATUITA, com os seguintes valores: contribuir com a comunidade de qualidade, incentivar/ensinar a busca autodidata de conhecimento e valorizar/fortalecer o papel da qualidade no desenvolvimento de software.</p>

      <p class="flow-text text-justify"> Desta forma, vamos conseguir ter um gostinho e aprender o básico de como executar algumas ferramentas que fazem parte do dia-a-dia dos profissionais que querem garantir a qualidade de um software. </p>

       <p class="flow-text text-justify"> Estes workshops são direcionados para qualquer profissional que trabalhe ou queira aprender sobre qualidade de software e não somente para QAs.</p>
    </div>
    <div class="col m4 s12">
      <div class="sponsors">
        <h5>Patrocínio</h5>
        <div class="logos">
          {% for sponsor in site.sponsors %}
            <a href="{{ sponsor[1] }}" target="_blank">
              <img src="/assets/img/sponsors/{{ sponsor[0] }}.png">
            </a>
          {% endfor %}
        </div>
      </div>
    </div>
  </div>
</div>
