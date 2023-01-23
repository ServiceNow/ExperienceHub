---
title: "Guides"
layout: page
permalink: /guides/
description: Putting the platform in context of experience goals.
---
<p>{{page.description}}</p>
<div class="outcome-group">
{% for guide in site.guides %}
    <a href="{{guide.url}}">{{ guide.title }}</a>
{% endfor %}
</div>