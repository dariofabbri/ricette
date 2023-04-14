{{ site.pages }}

{{ site.pages | where: "categoria", "primo" }}

{{ site.pages | where: "categoria", "secondo" }}

{{ site.pages | where: "categoria", "primo" | sort: "titolo" }}

{{ site.pages | where: "categoria", "secondo" | sort: "titolo" }}


{% for item in site.pages | where: "categoria", "primo" | sort: "titolo" %}
- {{ item.name }} {{ item.url }}
{% endfor %}

{% for item in site.pages | where: "categoria", "secondo" | sort: "titolo" %}
- {{ item.name }} {{ item.url }}
{% endfor %}