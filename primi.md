{% for item in site.pages | where: "categoria", "primo" | sort: "titolo" %}
- {{ item.name }} {{ item.url }}
{% endfor %}

{% for item in site.pages | where: "categoria", "secondo" | sort: "titolo" %}
- {{ item.name }} {{ item.url }}
{% endfor %}