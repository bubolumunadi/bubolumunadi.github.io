---
layout: page
title: Hakkımda
permalink: /about/
---

Based on a true story 🃏

### Sertaç Öz

Sokakta Fotoğrafçı 📷🚶🏻 
Hava Yolları'nda Mühendis ✈️👔

### İletişim

    <footer id="footer">
      <p class="editor-link"><a href="cloudcannon:collections/_data/social.yml" class="button"><strong>&#9998;</strong> Update Social Icons</a></p>
      <ul class="icons">
        {% for account in site.data.social %}
					<li>
						<a {% if account.new_window %}target="_blank"{% endif %} href="{% include relative-src.html src=account.link %}" {% if account.social_icon %}class="icon fa-{{ account.social_icon | slugify }}"{% endif %}>
              <span class="label">{{ account.name }}</span>
						</a>
					</li>
				{% endfor %}
        {% if site.author.email %}
        <li>
          <a href="mailto:{{ site.author.email }}" class="icon fa-envelope-o">
            <span class="label">Email</span>
          </a>
        </li>
        {% endif %}
      </ul>

[sozphotography@hotmail.com](mailto:sozphotography@hotmail.com)
