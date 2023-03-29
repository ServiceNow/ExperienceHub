---
    name: Challenges and Opportunities
    stage: ["Understand"]
    outcomes: ["TransformProcess"]
    description: Identify what is working well and holding you back from achieving a stated goal.
    order: 100
    layout: page
    related: ["How Might We"]
---
## Overview
A fun and engaging workshop where participants identify what is helping or hindering your team’s ability to achieve stated goal. In the workshop, participants identify the "winds" that move you closer to the goal and the “anchors” that hold you back.

## Outcomes
* Critical issues preventing your team from goal achievement
* Alignment to ServiceNow products and/or capabilities to resolve

## Participants
You want an equal representation of participants to shed light on the user, business, and technical reasons for the success or failure. We recommend 5-15 participants for this workshop.


## Materials & environment
### In Person Session
* Sticky notes, Permanent markers
* Dry erase markers
* Butcher wall paper or white board
* Large conference room – so participants can walk around and interact with materials
* Voting dots

### Virtual Session
* Online white board collaboration tool (Miro, Mural, Figjam, etc)
* Template for the workshop
  	
## Process

### Before you start
1. Identify your goal, or specific solution that you will be talking about. Consider the [Long Term Goal](./long-term-goal) method if the goal is not clear.
2. Set up your online collaboration space, or in person conference room.
3. The facilitator will present the stated long term goal to all participants
4. Each participant documents 3-5 "winds" that currently help the organization achieve the presented goal. **5 minutes**
5. Each participant documents 3-5 "anchors" that currently *prevent* the organization from achieving the presented goal. **5 minutes**
6. In groups of no more than FOUR, share your winds and anchors. **10 minutes**
7. Each group should vote on their Top 3 anchors. **5 minutes**
8. Select 1 representative from each group to share their anchors on the main whiteboard.
9. After all groups have shared, work with the presenters to find logical groupings of anchors. **5 minutes**
10. Give each participant 3 voting dots and ask them to vote on their TOP 3 anchor groups. *They can vote on one group multiple times*
11. The items with the most votes are the challenges that you should focus on first

## Synthesis
You can use the anchors to inspire ideation. We suggest reframing the challenges into [How Might We...](./how-might-we) statements first.

## Related Methods
{% assign methods = site.methods | where: "related", "Challenges and Opportunities" %}
{% for method in methods %}
  {% include method.html  method=method %}
{% endfor %}

## Related Plays
{% assign outcomes = site.outcomes | where: "related", "Challenges and Opportunities" %}
{% for outcome in outcomes %}
  {% include outcome.html  outcome=outcome %}
{% endfor %}

## Learn More
- (The "Anchors and Winds" approach)[https://www.curiositytank.com/blog/the-anchors-and-wind-approach]
- (The Hot Air Balloon retrospective in 9 steps)[https://conceptboard.com/blog/hot-air-balloon-retrospective-template/]
- (Hot Air Balloon)[https://thefacilitationhub.com/tools/hot-air-balloon-planning/]