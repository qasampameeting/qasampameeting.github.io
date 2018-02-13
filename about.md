---
layout: default
title: Sobre QA Sampa Meeting
---

<div class="about">
  <h1 class="pageTitle">sobre</h1>
  <div class="about-wrapper">
	  <div class="about-text">
		  <p class="intro">Para quem?</p>
		  <p>Profissionais que desejam aprender sobre qualidade de software ou que desejam ingressar na área</p>

		  <p class="intro">Por que?</p>
		  <p>Reunião mensal para nos conhecermos e conversarmos sobre um tema dentro da área de qualidade de software. Teremos a presença de um convidado experiente ou com um conteúdo bacana para nos apresentar de maneira bem informal. Cada um poderá levar seu notebook para interagirmos com o tema explorado. O tema será disponibilizado com duas semanas de antecedência para anotarmos nossas dúvidas e outros detalhes que desejarmos.</p>
		  <p>Muito café ou chá, conversa e troca de experiência e conhecimento!</p>
	  </div>

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
