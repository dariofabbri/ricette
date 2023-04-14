{% for item in site.pages | where: "categoria", "primo" %}
- {{ item.name }} {{ item.url }}
{% endfor %}