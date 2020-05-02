---
layout: page
title: talks
permalink: /talks/
description: 
---

 {% if site.talks  %}
  {% assign talks = site.talks | reverse %}
{% for talk in talks %}
{% if talk.inline %}
 * <i>{{ talk.date | date: "%b %-d, %Y" }}, at {{ talk.place }}</i>:   {{ talk.content | remove: '<p>' | remove: '</p>' }}
 {% else %}

 {% endif %}
{% endfor %}
{% endif %}
    


