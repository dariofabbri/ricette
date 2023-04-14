Site pages
{{ site.pages }}

Site pages filter primo
{{ site.pages | where:"categoria","primo" }}

Site pages filter secondo
{{ site.pages | where:"categoria","secondo" }}

Site pages filter primo sort
{{ site.pages | where:"categoria","primo" | sort:"titolo" }}

Site pages filter secondo sort
{{ site.pages | where:"categoria","secondo" | sort:"titolo" }}

Aaaaa
{% for item in site.pages | where: "categoria", "primo" | sort: "titolo" %}
- {{ item.name }} {{ item.url }}
{% endfor %}

Bbbbb
{% for item in site.pages | where: "categoria", "secondo" | sort: "titolo" %}
- {{ item.name }} {{ item.url }}
{% endfor %}