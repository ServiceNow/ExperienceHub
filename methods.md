---

title: "Experience Enablement - Methods"
layout: default
permalink: /methods/
---
Methods are the specific activies that will help you learn, explore and create great experiences with ServiceNow. Methods are the items that make up plays which serve specific business outcomes.

## Method Categories
We organize methods into 3 different categories
- Understand - Techniques to learn more about your users, business processes and more
- Ideate - Techniques to generate and validate ideas for how to solve a business problem
- Create - Techniques to create the artifacts to feed your implementation

{% assign understand_methods = site.methods | where: "stage", "Understand" %}
{% assign create_methods = site.methods | where: "stage", "Create" %}
{% assign ideate_methods = site.methods | where: "stage", "Ideate" %}
## Understand
<div class="method-group">
{% for method in understand_methods %}
  {% include method.html  method=method %}
{% endfor %}
</div>

## Ideate
<div class="method-group">
{% for method in ideate_methods %}
  {% include method.html  method=method %}
{% endfor %}
</div>

## Create
<div class="method-group">
{% for method in create_methods %}
  {% include method.html  method=method %}
{% endfor %}
</div>