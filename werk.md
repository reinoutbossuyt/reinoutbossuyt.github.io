---
layout: default
title: "Portfolio Reinout Bossuyt"
description: "Enkele relevante projecten van mijn werk doorheen de jaren. Ontdek de verschillende voorbeelden."
---

<h1>Portfolio</h1>

<p class="lead">Relevante projecten van mijn werk doorheen de jaren.</p>

<div class="werken">
{% for werk in site.werken %}
  <a id="{{werk.slug}}"></a>
  <div class="werk">
    <div class="werk--info">
      <p class="werk--naam">{{werk.title}} <span class="label">{{werk.date | date: "%Y"}}</span></p>
      {{werk.content}}
      <p>&mdash; <strong>{{werk.stack}}</strong></p>
    </div>
    <div class="werk--afbeelding">
      <img src="/assets/img/{{werk.image}}" alt="{{werk.titel}}">
    </div>
  </div>
{% endfor %}
</div>

{% include contact.html %}
