---
titolo: Secondi piatti
layout: list
---

{% assign pages = site.pages | where:"categoria","secondo" | sort:"titolo" %}
{% for page in pages %}
- {{ page.name }} {{ page.url }}
{% endfor %}