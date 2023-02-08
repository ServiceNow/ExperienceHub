---
    name: Card Sorting
    description: Learn how users expect content to be organized to align to your site taxonomy
    plays: []
    stage: ["Understand"]
    outcomes: ["DeliverSelfService"]
    order: 100
    output: true
    layout: page
    related: ["Tree Testing"]
---
## Method Overview
A key challenging when organizing large amounts of content or web pages in a application is deciding how to group related content in a coherent way. Often organizations map digital content to how their actual business is organized. Unfortunately, this does not always map to users’ mental model of the content they are trying to find. Card sorting is a generative exercise where participants provide their perspective of how content should be organized by physically placing content items into logical groupings.

## Outcomes
* Ideal content taxonomy based on users’ mental model


## Prerequisites
* Defined set of content items for the application

## Participants
Test participants should represent potential users of the site and have limited “inside knowledge” of the service providers. That means not including help desk staff or ServiceNow team members.

## Materials Needed
* An online card sorting tool such as OptimalSort, MUIQ, or UserZoom
* Teleconferencing tool if conducting a moderated test
* Index Cards if not using online tool (2 colors)

## Process
When conducting a card sort we recommend that you conduct a few moderated sessions (3-5) to get qualitative feedback and confirm the test is well structured. In addition, you should run 20+ users through unmoderated testing to get a large enough sample of data to make decisions.

#### There are two types of card sorts that you can use


**Closed Card Sort:** You know the categories within the taxonomy but want users' perspective of how to organize the content within those categories. A closed sort has predefined categories and users are only asked to put the content items into the category that makes the most sense.

**Open Card Sort:** You have a list of content items and want to see how users organize them into groups and how they name the groups. In an open sort, study participants get to name the categories.

### Closed Card Sort
1.	On each index card, write out one content item. If using an online tool, set up the content items following the tool’s instructions
2.	On a different color index card, write out your top level categories
3.	Ask each participant to group the content item cards under the category card that makes the most sense to them
4.	After each session, document the groups each participant created.
5.	In the moderated sessions, pay as much attention to what participants say while sorting as to how they sort. The qualitative insights are valuable.

### Open Card Sort
1.	On each index card, write out one content item. If using an online tool, set up the content items following the tool’s instructions
2.	Ask each participant to group the content item cards under the category card that makes the most sense to them
3.	Using a different color index card, ask participants to name each of groups they created in step #2.
4.	After each session, document the groups each participant created.
5.	In the moderated sessions, pay as much attention to what participants say while sorting as to how they sort. The qualitative insights are valuable.


## Synthesis
After all the sessions, your goal is to understand what are the most common ways participants grouped content. For each content item, you want to understand what group they were most often organized into. Online testing tools will make analysis easier as they’ll show the most common groupings and guide you through interpreting the results.

## Related Methods
{% assign methods = site.methods | where: "related", page.name %}
{% for method in methods %}
  {% include method.html  method=method %}
{% endfor %}

## Related Plays
{% assign outcomes = site.outcomes | where: "related", page.name %}
{% for outcome in outcomes %}
  {% include outcome.html  outcome=outcome %}
{% endfor %}

## Learn More
[Card Sorting 101 (Optimal Workshop)](https://www.optimalworkshop.com/learn/101s/card-sorting/)

[Card Sorting: Uncover Users' Mental Models for Better Information Architecture (NN Group)](https://www.nngroup.com/articles/card-sorting-definition/)
