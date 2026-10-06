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
    {% assign contact_leaders = "Neil Walton|Amir Michael|Kathy D. Wei" | split: "|" %}
    {% for contact_name in contact_leaders %}
    {% assign director = site.data.people | where: "name", contact_name | first %}
    <div>
      <p class="baiac-card__label">{% if contact_name == "Neil Walton" %}Director{% else %}Co-Director{% endif %}</p>
      <h3>{% if director.website != empty %}<a href="{{ director.website | escape }}" rel="external">{% if contact_name == "Amir Michael" %}Michael Amir{% elsif contact_name == "Kathy D. Wei" %}Kathy Wei{% else %}{{ director.name | escape }}{% endif %}</a>{% else %}{% if contact_name == "Amir Michael" %}Michael Amir{% elsif contact_name == "Kathy D. Wei" %}Kathy Wei{% else %}{{ director.name | escape }}{% endif %}{% endif %}</h3>
      {% if director.affiliation != empty %}<p>{{ director.affiliation | escape }}</p>{% endif %}
    </div>
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

<section class="conversation-section" aria-labelledby="conversation-heading">
  <div class="conversation-card">
    <div class="conversation-intro">
      <p class="eyebrow">Get involved</p>
      <h2 id="conversation-heading">Start the Conversation</h2>
      <p>The Business AI and Analytics Centre (BAIAC) welcomes engagement from academics, businesses, public-sector organisations, technology partners, students, and prospective collaborators.</p>
      <p>We are interested in conversations about artificial intelligence, analytics, organisational transformation, decision making, innovation, research collaboration, seminars, workshops, and the future of business.</p>
      <p>Whether you are exploring a collaborative research project, industry partnership, student opportunity, speaking engagement, or broader discussion about AI and analytics, we would be delighted to hear from you.</p>
    </div>
    <div class="conversation-grid">
      <article class="conversation-mini-card">
        <h3>Research Collaboration</h3>
        <p>Connect with researchers across accounting, analytics, information systems, finance, marketing, operations research and management.</p>
      </article>
      <article class="conversation-mini-card">
        <h3>Industry &amp; Public Sector</h3>
        <p>Explore partnerships, workshops, executive engagement and real-world applications of AI and analytics.</p>
      </article>
      <article class="conversation-mini-card">
        <h3>Students &amp; Early Career Researchers</h3>
        <p>Learn about doctoral opportunities, seminars, projects and research activities.</p>
      </article>
    </div>
    <div class="conversation-action">
      <a class="conversation-button" href="https://forms.cloud.microsoft/e/3YCY0jLvcc" target="_blank" rel="noopener noreferrer">Start the Conversation <span aria-hidden="true">→</span></a>
      <p class="conversation-note">All enquiries are reviewed by the Centre and directed to the most appropriate member of the BAIAC community.</p>
    </div>
  </div>
</section>
