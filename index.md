---
layout: default
---

## ¡Bienvenido al Mundo de la Ciberseguridad y el Hacking Ético!

<p style="text-align: justify;">
Mi objetivo es compartir mi pasión y conocimiento sobre ciberseguridad y hacking ético.Te guiaré a través de emocionantes aventuras autodidactas. Mi misión es fomentar la comprensión de las vulnerabilidades en los sistemas, explorar la mentalidad de los atacantes y aprender cómo proteger lo que más valoras. Acompáñame en este viaje, donde compartiré recursos, tutoriales y experiencias, juntos exploraremos este emocionante terreno de la ciberseguridad. ¡Vamos a comenzar esta emocionante travesía juntos!
</p>

<ul class="post-list">
    {%- for post in site.posts -%}
    <li>
    {%- assign date_format = site.minima.date_format | default: "%b %-d, %Y" -%}
    <span class="post-meta">{{ post.date | date: date_format }}</span>
    <h3>
        <a class="post-link" href="{{ post.url | relative_url }}">
        {{ post.title | escape }}
        </a>
    </h3>
    {%- if site.show_excerpts -%}
        {{ post.excerpt }}
    {%- endif -%}
    </li>
    {%- endfor -%}
</ul>