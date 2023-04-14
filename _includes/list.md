{% assign pages = site.pages | where:page.filtro-chiave,page.filtro-valore | sort:"titolo" %}
{% for page in pages %}
- [{{ page.titolo }}](/{{ site.github.repository_name }}{{ page.url }})
{% endfor %}