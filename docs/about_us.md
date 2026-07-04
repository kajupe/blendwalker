---
title: About Us
layout: default
nav_order: 9995
author_footer: false
authors: 
  - key: kaj
    role: Project Manager
  - key: fioh
    role: Project Manager
---

# About Us
{: .fs-9 .no_toc }
Learn more about the people who helped make this page
{: .fs-6 .fw-300 }

---

## PROJECT MANAGERS
Project Managers are the people who look at submissions from contributors and ensure the page retains a high quality standard. They're often also contributors themselves! 

<br>

{% if page.authors %}
{% for author_item in page.authors %}
{% if author_item.role == "Project Manager" %}
{% assign author = site.data.authors[author_item.key] %}
{% if author %}
<div id="about_{{ author_item.key }}" style="padding-bottom:3rem;">
    <div style="display:flex !important; align-items:center; gap:1rem;">
        <img src="{{ author.avatar | relative_url }}" alt="{{ author.name }}" class="author-profile-pic no-lightbox">
        <p style="font-size:1.5rem; margin:0rem; ">{{ author.name }}</p>
    </div>
    <span class="about-bio">{{ author.bio }}</span>
    {% if author.links %}
    <div class="about-links" style="font-size: 1rem; margin-top: 0.5rem;">
    {% for link in author.links %}
        <a href="{{ link.url }}">
        {{ link.label }}
        </a>
        {% unless forloop.last %}
        <span style="color: #ccc;">|</span>
        {% endunless %}
    {% endfor %}
    </div>
    {% endif %}
</div>
{% endif %}
{% endif %}
{% endfor %}
{% endif %}

---

## CONTRIBUTORS
Contributors from the community have generously offered their time to write something for the benefit of all! Want to write something too? [Learn how!](./contributing)

<br>

{% if page.authors %}
{% for author_item in page.authors %}
{% if author_item.role == "Contributor" %}
{% assign author = site.data.authors[author_item.key] %}
{% if author %}
<div id="about_{{ author_item.key }}" style="padding-bottom:3rem;">
    <div style="display:flex !important; align-items:center; gap:1rem;">
        <img src="{{ author.avatar | relative_url }}" alt="{{ author.name }}" class="author-profile-pic no-lightbox">
        <p style="font-size:1.5rem; margin:0rem; ">{{ author.name }}</p>
    </div>
    <span class="about-bio">{{ author.bio }}</span>
    {% if author.links %}
    <div class="about-links" style="font-size: 1rem; margin-top: 0.5rem;">
    {% for link in author.links %}
        <a href="{{ link.url }}">
        {{ link.label }}
        </a>
        {% unless forloop.last %}
        <span style="color: #ccc;">|</span>
        {% endunless %}
    {% endfor %}
    </div>
    {% endif %}
</div>
{% endif %}
{% endif %}
{% endfor %}
{% endif %}