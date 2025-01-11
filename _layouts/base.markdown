---
title: "Martin Smeaton"
meta_description: "Gallery of the art of Martin Smeaton."
activeP: true
---
<!DOCTYPE html>
<html>
  <head>
    <meta charset="utf-8">
    <title>{{ page.title }}</title>
    {% include meta.markdown %}
    <link rel="stylesheet" href="{{ '/assets/css/normalize.css' | relative_url }}">
    <link rel="stylesheet" href="{{ '/assets/css/main.css' | relative_url }}">
    <link rel="stylesheet" href="{{ '/assets/css/responsive.css' | relative_url }}">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
  </head>
  <body>
    <header style="background:none;border:none;">
      <a href="{{ '/' | relative_url }}" id="logo_home" style="text-decoration:none;">
        <img src="{{ '/assets/images/logo.png' | relative_url }}" alt="Martin Smeaton Logo"/>
        <div id="name_home">
          <div id="logo_top"><h1>Martin Smeaton</h1></div>
          <h2>Martin Smeaton</h2>
        </div>
      </a>
      <div class="clearfix"></div>
      <nav>
        <ul>
          <li><a href="{{ '/gallery' | relative_url }}" {% if page.activeP %}class="selected"{% endif %}>GALLERY</a></li>
          <li><a href="{{ '/about' | relative_url }}" {% if page.activeA %}class="selected"{% endif %}>ABOUT</a></li>
          <li><a href="{{ '/contact' | relative_url }}" {% if page.activeC %}class="selected"{% endif %}>CONTACT</a></li>
        </ul>
      </nav>
    </header>
    <div id="wrapper">
      {{ content }}
      {% include silver.markdown %}
      <!-- stick footer-->
      <div class="push"></div>
    </div><!--/.wrapper-->
    <footer>
      <p>&copy; {{ 'now' | date: "%Y" }} Martin Smeaton</p>
      <a href="{{ '/contact' | relative_url }}"><img src="{{ '/assets/images/logo.png' | relative_url }}" alt="Martin Smeaton Logo" class="social-icon"></a>
    </footer>
    <!-- Google tag (gtag.js) -->
    <script async src="https://www.googletagmanager.com/gtag/js?id=G-117Y5TR08G"></script>
    <script>
      window.dataLayer = window.dataLayer || [];
      function gtag(){dataLayer.push(arguments);}
      gtag('js', new Date());
      gtag('config', 'G-117Y5TR08G');
    </script>
    <!-- End Google tag -->
  </body>
</html>
