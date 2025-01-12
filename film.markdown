---
layout: base
title: "FILM"
meta_description: "Gallery of the works of Martin Smeaton for film."
activeF: true
---

  <section>
    <ul id="gallery">
    {% for f in site.film_gallery %}
      <li>
        <a href="{{ f.permalink | relative_url }}">
          <img src="{{ f.img_small | relative_url }}" alt="{{ f.title }}">
          <p>{{ f.title }}</p>
          <p>{{ f.meta_description }}</p>
        </a>
      </li>
    {% endfor %}
    </ul>
  </section>
