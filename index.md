---
layout: default
title: "Reinout Bossuyt"
description: "Hallo, Ik ben Reinout. Ik hou ervan complexe zaken te verhelderen. Hoe kan ik je helpen?"
---

<div class="home">

<div class="home-info">

<section class="intro">
  <div>
  <p class="intro--text">Hallo,<br/>
  Ik ben <a href="/over">Reinout</a>.<br/>
  Ik hou ervan<br/>
  complexe zaken<br/>
  te verhelderen.</p>
  </div>
  <div class="image-small"></div>
</section>

<section class="jobs">
  <p class="jobs--text">Een goed geformuleerd probleem is al voor de helft opgelost. Dat is mijn motto. Bij deze opdrachten bracht ik mijn passie al in de praktijk:</p>
  <div class="accordion" id="accordionExample">
    {% for job in site.data.jobs %}
    <div class="accordion-item">
      <h2 class="accordion-header" id="headingOne">
        <button class="accordion-button" type="button" data-bs-toggle="collapse" data-bs-target="#collapse{{forloop.index}}" aria-expanded="true" aria-controls="collapseOne">
          {{job.naam}}
        </button>
      </h2>
      <div id="collapse{{forloop.index}}" class="accordion-collapse collapse" data-bs-parent="#accordionExample">
        <div class="accordion-body">
          <p class="job-beschrijving">{{job.beschrijving}}</p>
          <ul class="job-details">
            <li class="job-periode">
              <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24"><path fill="none" d="M0 0h24v24H0z"></path><path d="M12 22C6.47715 22 2 17.5228 2 12C2 6.47715 6.47715 2 12 2C17.5228 2 22 6.47715 22 12C22 17.5228 17.5228 22 12 22ZM12 20C16.4183 20 20 16.4183 20 12C20 7.58172 16.4183 4 12 4C7.58172 4 4 7.58172 4 12C4 16.4183 7.58172 20 12 20ZM13 12H17V14H11V7H13V12Z"></path></svg>
              {{job.periode}}
            </li>
            {% if job.case.naam %}
            <li class="job-case">
              <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24"><path fill="none" d="M0 0h24v24H0z"></path><path d="M15 4H5V20H19V8H15V4ZM3 2.9918C3 2.44405 3.44749 2 3.9985 2H16L20.9997 7L21 20.9925C21 21.5489 20.5551 22 20.0066 22H3.9934C3.44476 22 3 21.5447 3 21.0082V2.9918ZM13.529 14.4464C11.9951 15.3524 9.98633 15.1464 8.66839 13.8284C7.1063 12.2663 7.1063 9.73367 8.66839 8.17157C10.2305 6.60948 12.7631 6.60948 14.3252 8.17157C15.6432 9.48951 15.8492 11.4983 14.9432 13.0322L17.1537 15.2426L15.7395 16.6569L13.529 14.4464ZM12.911 12.4142C13.6921 11.6332 13.6921 10.3668 12.911 9.58579C12.13 8.80474 10.8637 8.80474 10.0826 9.58579C9.30156 10.3668 9.30156 11.6332 10.0826 12.4142C10.8637 13.1953 12.13 13.1953 12.911 12.4142Z"></path></svg>
              <strong>Relevant werk:</strong> <a href="{{job.case.link}}">{{job.case.naam}}</a>
            </li>
            {% endif %}
            {% if job.quote %}
            <li class="job-quote">
              <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24"><path fill="none" d="M0 0h24v24H0z"></path><path d="M21 3C21.5523 3 22 3.44772 22 4V18C22 18.5523 21.5523 19 21 19H6.455L2 22.5V4C2 3.44772 2.44772 3 3 3H21ZM20 5H4V18.385L5.76333 17H20V5ZM10.5153 7.4116L10.9616 8.1004C9.29402 9.0027 9.32317 10.4519 9.32317 10.7645C9.47827 10.7431 9.64107 10.7403 9.80236 10.7553C10.7045 10.8389 11.4156 11.5795 11.4156 12.5C11.4156 13.4665 10.6321 14.25 9.66558 14.25C9.12905 14.25 8.61598 14.0048 8.29171 13.6605C7.77658 13.1137 7.5 12.5 7.5 11.5052C7.5 9.75543 8.72825 8.18684 10.5153 7.4116ZM15.5153 7.4116L15.9616 8.1004C14.294 9.0027 14.3232 10.4519 14.3232 10.7645C14.4783 10.7431 14.6411 10.7403 14.8024 10.7553C15.7045 10.8389 16.4156 11.5795 16.4156 12.5C16.4156 13.4665 15.6321 14.25 14.6656 14.25C14.1291 14.25 13.616 14.0048 13.2917 13.6605C12.7766 13.1137 12.5 12.5 12.5 11.5052C12.5 9.75543 13.7283 8.18684 15.5153 7.4116Z"></path></svg>
              <strong>Wat zeggen anderen?</strong><br/>
              {{job.quote.tekst}}<br/>&mdash; {{job.quote.naam}}</li>
            {% endif %}
          </ul>
        </div>
      </div>
    </div>
    {% endfor %}
  </div>
  <p class="job-toevoegen-tekst"><a href="/over#contact" class="job-toevoegen">Jouw organisatie / bedrijf toevoegen?</a></p>
</section>

<section class="multi">
  <p class="multi--text">Kortom, ik hou ervan om veel verschillende dingen te doen. Ik ben er namelijk van overtuigd dat mijn kennis van de ene activiteit voordelen oplevert voor de andere.</p>
</section>

</div>

<div class="image-large">
</div>

</div>

{% include contact.html %}
