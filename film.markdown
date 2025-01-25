---
layout: base
title: "FILM"
meta_description: "Gallery of the works of Martin Smeaton for film."
activeF: true
---

  <section>
    <ul id="gallery">
    {% for f in site.film_gallery %}
      {% if f.display != "false" %}
      <li>
        <a href="{{ f.permalink | relative_url }}">
          <img src="/assets/images/{{ f.img_small | relative_url }}" alt="{{ f.title }}">
          <p>{{ f.title }} - {{ f.meta_description }}</p>
        </a>
      </li>
      {% endif %}
    {% endfor %}
    </ul>
  </section>
