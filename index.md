---
title: Online Hosted Instructions
permalink: index.html
layout: home
---

# Azure Stream Analytics Exercises

These hands-on exercises are designed to support training content on [Microsoft Learn](https://docs.microsoft.com/training/).

You'll need an Azure subscription in which you have administrative access to complete these exercises. For some exercises, you will also need a Power BI service subscription.

{% assign labs = site.pages | where_exp:"page", "page.url contains '/Instructions/Labs'" %}
| Exercise |
| --- | 
{% for activity in labs  %}| [{{ activity.lab.title }}{% if activity.lab.type %} - {{ activity.lab.type }}{% endif %}]({{ site.github.url }}{{ activity.url }}) |
{% endfor %}

