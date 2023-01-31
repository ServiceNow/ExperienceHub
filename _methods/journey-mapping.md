---
    name: Journey Mapping
    stage: ["Understand"]
    outcomes: ["TransformProcess"]
    description: Visualize a user’s interactions across multiple channels with a solution from the beginning towards the achievement of a goal.
    order: 400
    layout: page
---
## Method Overview
Through this method, you create a timeline of touch points between the user, the application(s), and any people/organizations they interact with. The ideal time for journey mapping is when you want to identify users’ unmet needs and pain points, identify gaps and opportunities in their experience, and eliminate assumptions in how the process is experienced. This method is used to see the process or service from the users’ perspective. You can map out the current state of a process or envision an idealized future state via journey mapping.

## When to Use
* Need to identify unmet user needs and pain points
* Identify process gaps and opportunities to streamline
* Eliminate assumptions about how the process occurs
* Digitizing a manual, paper-based process 
* Replatforming a process onto ServiceNow
* Reviewing an existing process that has a negative NPS.

## Outcomes
* Visualizing the end-to-end customer experience 
* Creating alignment among internal teams of overall opportunities and gaps 

## Prerequisites
* Scope and clear objectives of the project
* Choose the right journey map type: current state, future state
* Primary user persona(s) and their goals identified
* Insights from user conversations or analytics to inform the map
* Workshop materials
* Understanding of user touch points with the product like actions, emotions, motivations, obstacles, and pain points

## Participants
Process owner, product manager, business analyst, design strategist, developer, and stakeholders

## Materials Needed
* Conference room, whiteboard, markers, butcher paper
* Or real-time collaboration whiteboarding tools such as Miro, or Mural

## Agenda

|Duration|Activity|
| -------- | ---------- |
|10 minutes	|Welcome and Agenda|
|90 minutes	|Current state journey mapping workshop|
|5 minutes	|Session wrap-up|

## What do you do after?
* Synthesize
* Capability Mapping/Sprint/Workshop

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
[Journey Mapping 101](https://www.nngroup.com/articles/customer-journey-mapping-process/)

[The 5 Steps of Successful Customer Journey Mapping](https://www.nngroup.com/articles/customer-journey-mapping-process/)

[Journey Mapping Course](https://www.interaction-design.org/courses/journey-mapping)

[How to Run a Journey-Mapping Workshop: A Step-by-Step Case Study](https://www.nngroup.com/articles/journey-mapping-workshop/)
