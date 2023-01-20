---
    layout: default
    title: Outcomes
    permalink: /outcomes
    description: When your employer invests in ServiceNow they are trying to move their business towards a specific outcome. The Experience Methods and Plays discussed on this site are organized by common outcomes our customers are trying to achieve to help you on your journey.
---
<p>{{page.description}}</p>
<div class="outcome-group">
{% for outcome in site.outcomes %}

  {% include outcome.html  outcome=outcome %}
{% endfor %}
</div>