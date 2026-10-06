---
layout: home
permalink: /
---

<section class="hero">
  <div class="hero-inner">
    <p class="eyebrow">Durham University Business School</p>
    <h1>Business AI and<br>Analytics Centre</h1>
    <p class="hero-copy">The Business AI and Analytics Centre (BAIAC) brings together researchers, students, industry partners, and public-sector organisations interested in artificial intelligence, analytics, optimisation, and data-driven decision making.</p>
    <nav class="hero-actions" aria-label="Explore the Centre">
      <a class="button button-light" href="{{ '/research/' | relative_url }}">Research <span aria-hidden="true">→</span></a>
      <a class="button button-outline" href="{{ '/people/' | relative_url }}">People <span aria-hidden="true">→</span></a>
      <a class="button button-outline" href="{{ '/events/' | relative_url }}">Events <span aria-hidden="true">→</span></a>
      <a class="button button-outline" href="{{ '/contact/' | relative_url }}">Contact <span aria-hidden="true">→</span></a>
    </nav>
    <div class="hero-note" aria-hidden="true">
      <span class="note-line"></span>
      <span>Research · Collaboration · Impact</span>
    </div>
  </div>
  <div class="hero-art" aria-hidden="true">
    <div class="orbit orbit-one"></div>
    <div class="orbit orbit-two"></div>
    <div class="orbit orbit-three"></div>
    <span class="art-core">AI<br><small>×</small><br>BUSINESS</span>
    <span class="art-point point-one"></span>
    <span class="art-point point-two"></span>
    <span class="art-point point-three"></span>
    <span class="art-point point-four"></span>
  </div>
</section>

<section class="section-wrap news-section" aria-labelledby="about-heading">
  <div class="section-heading news-heading">
    <div>
      <div class="section-label"><span>01</span> About the Centre</div>
      <h2 id="about-heading">Connecting disciplines to address real questions</h2>
    </div>
  </div>
  <div class="intro-content">
    <div class="intro-text">
      <p>The Centre exists to bring people together to understand and apply AI and analytics to important business and public-sector questions.</p>
    </div>
    <div class="intro-text">
      <p>Our interdisciplinary work links business with computing, mathematics and engineering, connecting technical insight with organisational needs and public-sector applications. We focus on research and exchange with practical impact.</p>
    </div>
  </div>
</section>

<section class="home-cta" aria-labelledby="conversation-heading">
  <div class="home-cta-inner">
    <div>
      <p class="eyebrow">02 · Get in touch</p>
      <h2 id="conversation-heading">Start the Conversation</h2>
      <p>We welcome discussion with academics, doctoral students, businesses, public-sector organisations and technology partners.</p>
    </div>
    <a class="button button-outline" href="{{ '/contact/' | relative_url }}">Contact the Centre <span aria-hidden="true">→</span></a>
  </div>
</section>

<section class="section-wrap news-section" aria-labelledby="working-heading">
  <div class="section-heading news-heading">
    <div>
      <div class="section-label"><span>03</span> Working with the Centre</div>
      <h2 id="working-heading">Different ways to work together</h2>
    </div>
    <p>Engagement can take many forms, shaped around shared questions and goals.</p>
  </div>
  <div class="news-grid">
    <article class="news-card">
      <p class="card-index">RESEARCH</p>
      <h3>Collaborative research</h3>
      <p>Develop research with academic and industry partners, including projects that connect organisations with expertise across disciplines.</p>
    </article>
    <article class="news-card">
      <p class="card-index">EXCHANGE</p>
      <h3>Seminars and workshops</h3>
      <p>Share ideas, discuss emerging questions and bring researchers and practitioners together through seminars and workshops.</p>
    </article>
    <article class="news-card">
      <p class="card-index">LEARNING</p>
      <h3>Doctoral and executive learning</h3>
      <p>Explore PhD projects, executive education and industry partnerships that support learning and the exchange of expertise.</p>
    </article>
  </div>
</section>

<section class="section-wrap news-section" aria-labelledby="initiative-heading">
  <div class="section-heading news-heading">
    <div>
      <div class="section-label"><span>04</span> Featured initiative</div>
      <h2 id="initiative-heading">Microsoft AI Skills Centre of Excellence</h2>
    </div>
  </div>
  <article class="news-card">
    <p>The Durham University–Microsoft partnership brings together expertise, tools and support to help people develop practical, responsible and inclusive AI skills.</p>
    <a class="text-link" href="{{ '/microsoft-ai-skills-centre/' | relative_url }}">Explore the initiative <span aria-hidden="true">→</span></a>
  </article>
</section>

<section class="section-wrap news-section" aria-labelledby="themes-heading">
  <div class="section-heading news-heading">
    <div>
      <div class="section-label"><span>05</span> Research themes</div>
      <h2 id="themes-heading">A connected research community</h2>
    </div>
    <p>Our work spans AI, Analytics, Operations Research and Information Systems.</p>
  </div>
</section>

<section class="section-wrap news-section" aria-labelledby="news-heading">
  <div class="section-heading news-heading">
    <div>
      <div class="section-label"><span>06</span> From the Centre</div>
      <h2 id="news-heading">News and Events</h2>
    </div>
    <p>Updates, seminars and opportunities to meet the Centre.</p>
  </div>
  <div class="news-grid">
    {% for item in site.data.news %}
    <article class="news-card">
      <p class="card-index">{{ item.category }}</p>
      <h3>{{ item.title }}</h3>
      <p>{{ item.description }}</p>
    </article>
    {% endfor %}
    {% assign has_upcoming_events = false %}
    {% for event in site.data.events.upcoming %}
    {% unless event.placeholder %}
    {% assign has_upcoming_events = true %}
    <article class="news-card">
      <p class="card-index">UPCOMING EVENT</p>
      <h3>{{ event.title }}</h3>
      {% unless event.date == blank %}<p>{{ event.date }}{% unless event.location == blank %} · {{ event.location }}{% endunless %}</p>{% endunless %}
      <p>{{ event.description }}</p>
    </article>
    {% endunless %}
    {% endfor %}
    {% unless has_upcoming_events %}
    <article class="news-card">
      <p class="card-index">UPCOMING EVENTS</p>
      <h3>Meet and exchange with the Centre</h3>
      <p>Seminars, workshops and other events will be listed as details are confirmed.</p>
      <a class="text-link" href="{{ '/events/' | relative_url }}">View events <span aria-hidden="true">→</span></a>
    </article>
    {% endunless %}
  </div>
</section>
