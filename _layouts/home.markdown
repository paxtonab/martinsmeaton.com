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
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: Arial, sans-serif;
            background-color: #121212;
            color: white;
            line-height: 1.6;
        }

        .navbar {
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 1rem 2rem;
            background-color: #1e1e1e;
            position: sticky;
            top: 0;
            z-index: 1000;
        }

        .navbar a {
            color: white;
            text-decoration: none;
            margin: 0 1rem;
            font-size: 1rem;
        }

        .navbar a:hover {
            text-decoration: underline;
        }

        .hero {
            position: relative;
            text-align: center;
        }

        .hero img {
            width: 100%;
            height: auto;
            display: block;
        }

        .hero-text {
            position: absolute;
            top: 50%;
            left: 50%;
            transform: translate(-50%, -50%);
            text-align: center;
        }

        .hero-text h1 {
            font-size: 2.5rem;
            margin-bottom: 0.5rem;
        }

        .hero-text p {
            font-size: 1.2rem;
            margin-bottom: 1rem;
        }

        .hero-text a {
            display: inline-block;
            padding: 0.75rem 1.5rem;
            font-size: 1rem;
            color: white;
            background-color: #e63946;
            text-decoration: none;
            border-radius: 5px;
            transition: background-color 0.3s ease;
        }

        .hero-text a:hover {
            background-color: #d62828;
        }

        .footer {
            text-align: center;
            padding: 1rem 0;
            background-color: #1e1e1e;
            margin-top: 1rem;
        }

        .footer img {
            width: 50px;
            height: auto;
            margin-top: 0.5rem;
        }

        @media (max-width: 768px) {
            .hero-text h1 {
                font-size: 2rem;
            }

            .hero-text p {
                font-size: 1rem;
            }

            .hero-text a {
                padding: 0.5rem 1rem;
                font-size: 0.9rem;
            }

            .navbar a {
                font-size: 0.9rem;
            }
        }
    </style>
  </head>
  <body>

    <header class="navbar">
        <div class="logo">
            <a href="#">Martin Smeaton</a>
        </div>
        <nav>
            <a href="#film">Film</a>
            <a href="#projects">Projects</a>
            <a href="#cv">CV</a>
            <a href="#contact">Contact</a>
        </nav>
    </header>

    <section class="hero">
        <img src="{{ '/assets/images/martin-smeaton-home.png' | relative_url }}" alt="Sculpture">
        <div class="hero-text">
            <h1>Martin Smeaton</h1>
            <p>Commercial Figurative Sculptor</p>
            <a href="#work">Work</a>
        </div>
    </section>

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
