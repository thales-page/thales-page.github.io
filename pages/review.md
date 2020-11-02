---
layout: default
title:  Book Reviews
description: Book Notes
keywords: review
permalink: /review/
---

<div class="reviewlist">
    {% for review in site.review reversed%}
    <div class="overview">
        <div class="date">{{ review.date | date: "%b %d, %Y" }}</div>
        <div class="detail"><a href="{{ site.url }}{{ review.url }}">{{ review.title }}</a></div>
    </div>
    {% endfor %}
</div>
<!--{% include pagination.html %}>


<!-- <ul>
{% for review in site.review %}
{% if review.title != "Review Template" %}
<li><a href="{{ site.url }}{{ review.url }}">{{ review.title }}</a></li>
{% endif %}
{% endfor %}
</ul> -->
