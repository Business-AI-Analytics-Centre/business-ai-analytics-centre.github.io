---
title: Contact
permalink: /contact/
redirect_from:
  - /contact.html
excerpt: Contact the Business AI and Analytics Centre at Durham University Business School.
---

<div class="baiac-contact-layout">
  <section>
    <p class="baiac-eyebrow">Business AI and Analytics Centre (BAIAC)</p>
    <h2>Durham University<br>Business School</h2>
    <p>For enquiries about research, events or collaboration, please contact the Centre through Durham University Business School.</p>
    <a class="baiac-button baiac-button--solid" href="https://www.durham.ac.uk/business/">Visit Durham University Business School <span aria-hidden="true">↗</span></a>
  </section>
  <aside class="baiac-contact-details">
    {% for director in site.data.people %}
    {% if director.role == "Director" %}
    <div>
      <p class="baiac-card__label">Director</p>
      <h3>{% if director.website != empty %}<a href="{{ director.website | escape }}" rel="external">{{ director.name | escape }}</a>{% else %}{{ director.name | escape }}{% endif %}</h3>
      {% if director.affiliation != empty %}<p>{{ director.affiliation | escape }}</p>{% endif %}
    </div>
    {% endif %}
    {% endfor %}
    <div>
      <p class="baiac-card__label">Email</p>
      {% if site.centre_email != empty %}
      <p><a href="mailto:{{ site.centre_email | escape }}">{{ site.centre_email | escape }}</a></p>
      {% else %}
      <p>A Centre email address will be added when an approved address is available.</p>
      {% endif %}
    </div>
  </aside>
</div>

<p class="baiac-note">Durham University Business School’s official website provides current institutional information and contact routes.</p>

<section class="baiac-contact-form" aria-labelledby="contact-form-heading">
  <div>
    <p class="baiac-eyebrow">Get in touch</p>
    <h2 id="contact-form-heading">Microsoft Form coming soon</h2>
    <p>A contact form will be available here. Until then, please use Durham University Business School’s contact routes.</p>
  </div>
  <div class="baiac-form-placeholder" role="region" aria-label="Space reserved for the future Microsoft contact form">
    <p>Contact form space reserved</p>
  </div>
</section>
