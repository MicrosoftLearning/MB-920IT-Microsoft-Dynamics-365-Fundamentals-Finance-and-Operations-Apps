---
title: Istruzioni online
permalink: index.html
layout: home
---

# Directory del contenuto

Di seguito sono elencati i collegamenti ipertestuali a ciascuno degli esercizi e delle demo dei lab.

## Lab

{% assign labs = site.pages | where_exp:"page", "page.url contains '/Instructions/Labs'" %}
| Modulo | Lab |
| --- | --- | 
{% for activity in labs  %}| {{ activity.lab.module }} | [{{ activity.lab.title }}{% if activity.lab.type %} - {{ activity.lab.type }}{% endif %}]({{ site.github.url }}{{ activity.url }}) |
{% endfor %}

## Demo

{% assign demos = site.pages | where_exp:"page", "page.url contains '/Instructions/Demos'" %}
| Modulo | Demo |
| --- | --- | 
{% for activity in demos  %}| {{ activity.demo.module }} | [{{ activity.demo.title }}]({{ site.github.url }}{{ activity.url }}) |
{% endfor %}
