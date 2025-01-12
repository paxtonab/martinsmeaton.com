{% if page.index %}
<section style="clear:both; max-width: 740px; margin: 0px auto;">
    {% if page.activeF %}
    <p class="breadcrumbs"><a href="/film">FILM</a> > {{ page.title }}</p>
    {% else %}
    <p class="breadcrumbs"><a href="/projects">PROJECTS</a> > {{ page.title }}</p>
    {% endif %}
    <h3>{{ page.title }}</h3>
    <img src="{{ page.img | relative_url }}" alt="{{ page.title }}">
    {% if page.description %}
        <p>{{ page.description }}</p>
    {% else %}
        <p>{{ page.meta_description }}</p>
    {% endif %}
</section>
{% endif %}