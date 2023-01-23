---
title: "Experience Enablement - Best Practices"
layout: default
permalink: /best-practices/
description: Based on internal research and industry insights, ServiceNow provides a set of Best Practices for how to use platform capabilities to deliver a great experience to your users.
---
<p>{{page.description}}</p>
<div class="outcome-group">
{% for practice in site.best-practices %}
    <a href="{{practice.url}}">{{ practice.title }}</a>
{% endfor %}
</div>