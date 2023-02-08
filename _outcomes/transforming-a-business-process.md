---
title: Transforming a Business Process
subtitle: Apply methods to understand and evolve the current state
share-description: When migrating and existing business process to ServiceNow you can follow this play to drive understanding of the current state, ideate how to best leverage the platform to improve the efficiency and usability of the process and validate that the solution will resonate with users and stakeholders.
layout: page
---
When you are looking at an existing business process that you want to digitize (e.g. the existing process is mostly offline) or migrate (move off an existing solution to ServiceNow), success comes from learning about the current state, the needs and challenges the users experience, and the goals of the business. With those insights, you can then ideate on how to realize the transformation with the ServiceNow platform.

This play guides you through the methods to understand how the process occurs today, where it can be better and then to envision the solution on ServiceNow.


## Understand
The first stage of the process is learn about your users and the current state process. The best method of doing this is to get right to the source by talking to an observing the users.

### Learn from your users
Business processes are nothing without the users that interact along the way. It is important to understand how their expectations and behaviors shape the outcomes of the process.
<div class="method-group">
{% assign play_methods = site.methods | where: "outcomes", "TransformProcess" | sort: "order" %}

{% assign understand_methods = play_methods | where: "stage", "Understand" %}

{% for method in understand_methods %}

{% include method.html  method=method %}
{% endfor %}
</div>

### Ideate
Once you have a strong understanding of the users and their relationship with the process, you are ready to start imagining a better future. The activities below will along you to focus on the future with limited time spent on "how it used to be".
<div class="method-group">
{% assign ideate_methods = play_methods | where: "stage", "Ideate" %}

{% for method in ideate_methods %}

{% include method.html method=method %}
{% endfor %}
</div>
