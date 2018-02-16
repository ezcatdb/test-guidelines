---
layout: entry
title: Enzyme reaction annotation guidelines
---

## Entities

{% assign sorted = site.entity | sort: 'order' %}
{% for i in sorted %}
- [{{ i.title }}]({{ i.url | remove_first:'/' }}){% if i.shortdef %}: {{ i.shortdef }}{% endif %}
{% endfor %}

## Events

{% assign sorted = site.event | sort: 'order' %}
{% for i in sorted %}
- [{{ i.title }}]({{ i.url | remove_first:'/' }}){% if i.shortdef %}: {{ i.shortdef }}{% endif %}
{% endfor %}

## Relations

{% assign sorted = site.relation | sort: 'order' %}
{% for i in sorted %}
- [{{ i.title }}]({{ i.url | remove_first:'/' }}){% if i.shortdef %}: {{ i.shortdef }}{% endif %}
{% endfor %}

## Attributes

{% assign sorted = site.attribute | sort: 'order' %}
{% for i in sorted %}
- [{{ i.title }}]({{ i.url | remove_first:'/' }}){% if i.shortdef %}: {{ i.shortdef }}{% endif %}
{% endfor %}
