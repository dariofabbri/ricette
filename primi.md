{% for item in site.pages %}
- {{ item.name }} {{ item.url }}
{% endfor %}