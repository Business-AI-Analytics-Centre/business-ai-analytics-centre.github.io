---
layout: splash
title: false
permalink: /
classes: wide
author_profile: false
---

<section class="baiac-hero">
  <div class="baiac-hero__inner">
    <p class="baiac-eyebrow">Durham University Business School</p>
    <h1>Business AI and<br>Analytics Centre</h1>
    <p class="baiac-hero__tagline">Advancing research in artificial intelligence, analytics, operations research, and data-driven decision making.</p>
    <nav class="baiac-hero__links" aria-label="Explore the Centre">
      <a class="baiac-button baiac-button--light" href="{{ '/research/' | relative_url }}">Research <span aria-hidden="true">→</span></a>
      <a class="baiac-button" href="{{ '/people/' | relative_url }}">People <span aria-hidden="true">→</span></a>
      <a class="baiac-button" href="{{ '/events/' | relative_url }}">Events <span aria-hidden="true">→</span></a>
      <a class="baiac-button" href="{{ '/contact/' | relative_url }}">Contact <span aria-hidden="true">→</span></a>
    </nav>
  </div>
</section>

<section class="baiac-section" aria-labelledby="themes-heading">
  <div class="baiac-section__heading">
    <p class="baiac-eyebrow">Research themes</p>
    <h2 id="themes-heading">Questions across disciplines</h2>
    <p>Our work examines the methods, organisations and decisions shaping data-informed business.</p>
  </div>
  <div class="baiac-grid baiac-grid--themes">
    <article class="baiac-card">
      <span class="baiac-card__number">01</span>
      <h3><a href="{{ '/research/#artificial-intelligence' | relative_url }}">Artificial Intelligence</a></h3>
      <p>Studying the development, adoption and governance of AI in organisational and economic settings.</p>
    </article>
    <article class="baiac-card">
      <span class="baiac-card__number">02</span>
      <h3><a href="{{ '/research/#analytics' | relative_url }}">Analytics</a></h3>
      <p>Investigating analytical methods and how evidence informs decisions in business and society.</p>
    </article>
    <article class="baiac-card">
      <span class="baiac-card__number">03</span>
      <h3><a href="{{ '/research/#operations-research' | relative_url }}">Operations Research</a></h3>
      <p>Applying mathematical and computational approaches to complex operational and strategic questions.</p>
    </article>
    <article class="baiac-card">
      <span class="baiac-card__number">04</span>
      <h3><a href="{{ '/research/#optimisation' | relative_url }}">Optimisation</a></h3>
      <p>Exploring models and methods for making choices under constraints, uncertainty and competing objectives.</p>
    </article>
    <article class="baiac-card">
      <span class="baiac-card__number">05</span>
      <h3><a href="{{ '/research/#information-systems' | relative_url }}">Information Systems</a></h3>
      <p>Understanding how digital systems shape organisations, work practices and relationships with technology.</p>
    </article>
  </div>
</section>

<section class="baiac-section baiac-section--tint" aria-labelledby="news-heading">
  <div class="baiac-section__heading">
    <p class="baiac-eyebrow">From the Centre</p>
    <h2 id="news-heading">News and updates</h2>
    <p>Announcements and research stories will be added as details are confirmed.</p>
  </div>
  <div class="baiac-grid baiac-grid--news">
    {% for item in site.data.news %}
    <article class="baiac-card baiac-news-card">
      <p class="baiac-card__label">{{ item.category }}</p>
      <h3>{{ item.title }}</h3>
      <p>{{ item.description }}</p>
    </article>
    {% endfor %}
  </div>
</section>

<section class="baiac-section" aria-labelledby="collaboration-heading">
  <div class="baiac-section__heading">
    <p class="baiac-eyebrow">Working together</p>
    <h2 id="collaboration-heading">Collaboration and exchange</h2>
    <p>We welcome thoughtful exchange across research, business and public life.</p>
  </div>
  <div class="baiac-grid baiac-grid--collaboration">
    <article class="baiac-card">
      <h3>Academic collaborators</h3>
      <p>We connect researchers across disciplines and institutions to develop shared questions and research.</p>
    </article>
    <article class="baiac-card">
      <h3>Industry engagement</h3>
      <p>Dialogue with organisations can ground research in current challenges and support exchange of expertise.</p>
    </article>
    <article class="baiac-card">
      <h3>Public sector partnerships</h3>
      <p>We are interested in evidence-informed conversations about the wider effects of AI and analytics.</p>
    </article>
  </div>
</section>

<section class="baiac-contact-strip">
  <div>
    <p class="baiac-eyebrow">Durham University Business School</p>
    <h2>Explore a research question with us.</h2>
  </div>
  <a class="baiac-button baiac-button--light" href="{{ '/contact/' | relative_url }}">Contact the Centre <span aria-hidden="true">→</span></a>
</section>
