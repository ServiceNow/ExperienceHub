---
    name: Usability Testing
    description: Observe users interacting with a prototype or production instance to see where they encounter friction
    plays: ["UnderstandProcess"]
    stage: ["Ideate"]
    outcomes: ["TransformProcess","DeliverSelfService"]
    order: 400  
    layout: page
--- 
## Method Overview
Usability testing is critical to including users in the process of building a solution on ServiceNow. Testing provides you with real evidence of the effectiveness of your team’s solution. By asking real users to complete actual tasks and observing their behavior you’ll identify issues with the solution and learn about their behavior. 

A usability test requires a facilitator to meet 1 on 1 with each participant and ask them to complete a series of tasks in the actual application, or a prototype. Ideally, a second observer is watching the interactions and taking notes of issues and behaviors. After all sessions are completed, the observations are synthesized for review and planning.

*There is plenty of research on the right number of participants to include in your study but a general rule of thumb is to:*

> “Once the rate of discovering new issues slows, you’ve tested with enough users.”

## Outcomes
* Better understanding of users’ behavior when completing the assigned tasks
* Improved user experience if the observed issues are addressed

## Prerequisites
* List of 3-5 common tasks users come to the site to perform.
* An interactive prototype (can be paper, design mockups) or the actual application (ideally in a non-production environment).

## Participants
Test participants should represent potential users of the site and have limited experience with the solution they will be interacting with. 

## Materials Needed
* Teleconferencing – if participants are remote or to allow observer to take notes from another room
* Interactive prototype or application

## Process 
1.	Prepare for the test by drafting a Facilitator’s Guide that helps the facilitator introduce the study and present the tasks
2.	Pilot the test with at least 1 person to ensure the tasks are clear and the prototype does not have any functional bugs.
3.	Work with stakeholders to recruit at least 5 participants for the initial round of testing.
4.	When the test begins, remind the participant that this is a test of the system, not the user so there are no wrong answers. Your goal is to get them talking aloud, describing what they are doing.
5.	During each session, the observer documents issues, behaviors, and any other insights that may help improve the overall experience.
6.	After all sessions are complete, aggregate the notes to see what issues were most common across the participants
7.	Prioritize the issues based on frequency of occurrence and impact to task success.

## Synthesis
Review the issues with the project team and identify remediation plans to improve the overall user experience. Once you make changes to the mockup or solution, rerun the usability study with new participants.

## Related Methods
{% assign methods = site.methods | where: "related", "Usability Testing" %}
{% for method in methods %}
  {% include method.html  method=method %}
{% endfor %}

## Related Plays
{% assign outcomes = site.outcomes | where: "related", "Usability Testing" %}
{% for outcome in outcomes %}
  {% include outcome.html  outcome=outcome %}
{% endfor %}

## Learn More
[Usability Testing 101 (Nielsen Norman Group)](https://www.nngroup.com/articles/usability-testing-101/)
[Checklist for Moderating a Usability Test (Nielsen Norman Group)](https://www.nngroup.com/articles/usability-checklist/)
[10 Golden Rules of Facilitation (MeasuringU)](https://measuringu.com/10-golden-rules-of-facilitation/)

