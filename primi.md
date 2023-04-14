---
titolo: Primi piatti
layout: list
---

{% assign pages = site.pages | where:"categoria","primo" | sort:"titolo" %}
{% for page in pages %}
- [{{ page.titolo }}](/{{ site.github.repository_name }}/{{ page.url }})
{% endfor %}