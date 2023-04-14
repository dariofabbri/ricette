{% assign pages = site.pages | where:"categoria",page.categoria | sort:"titolo" %}
{% for page in pages %}
- [{{ page.titolo }}](/{{ site.github.repository_name }}{{ page.url }})
{% endfor %}