---
layout: page
title: Reflexões
---

Textos sobre rotina, sentimentos, quedas, recomeços e silêncio.

---
layout: page
title: Reflexões
permalink: /reflexoes/
---

Aqui ficam meus textos de rotina, quedas, recomeços e silêncio.

{% assign reflexoes = site.categories.reflexoes %}
{% if reflexoes %}
  <ul>
    {% for post in reflexoes %}
      <li>
        <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
        <small> — {{ post.date | date: "%d/%m/%Y" }}</small>
      </li>
    {% endfor %}
  </ul>
{% else %}
  <p>Ainda não há posts aqui.</p>
{% endif %}
