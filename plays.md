---
    layout: default
    title: Plays
    permalink: /plays
    description: Plays provide a set of methods that help you with a learning goal.
---
<h1>{{page.title}}</h1>
<p>{{page.description}}</p>
<div class="play-group">
{% for play in site.plays %}

  <a href="{{ play.url }}">{{ play.title }}</a>
{% endfor %}
</div>