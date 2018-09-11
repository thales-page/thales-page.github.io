---
layout: default
title: Sapere
description: Book Notes
keywords: Wiki
permalink: /wiki/
---

<div class="wikilist">
    {% for wiki in site.wiki %}
    <div class="overview">
        <div class="date">{{ wiki.date | date: "%b %d, %Y" }}</div>
        <div class="detail"><a href="{{ site.url }}{{ wiki.url }}">{{ wiki.title }}</a></div>
    </div>
    {% endfor %}
</div>
<!--{% include pagination.html %}>


<!-- <ul>
{% for wiki in site.wiki %}
{% if wiki.title != "Wiki Template" %}
<li><a href="{{ site.url }}{{ wiki.url }}">{{ wiki.title }}</a></li>
{% endif %}
{% endfor %}
</ul> -->
