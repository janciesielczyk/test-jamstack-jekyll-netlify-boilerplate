---
layout: page
title: Oferta
meta_description: |
  This sets the meta description in the head of the page. You can watch the 
  output in the browser or in the generated file _site/oferta.html.
permalink: /oferta
section: oferta
intro_paragraph: 
---

  <section>

    <ul>
      {% for shoe in site.shoes %}
        <li>
          <h4>{{ shoe.title }}</h4>
          {% for image in shoe.images %}
            <img src="{{ image.thumbnail }}">
          {% endfor %}
        </li>
      {% endfor %}
    </ul>
  
  </section>