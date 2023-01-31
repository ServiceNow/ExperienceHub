---
    name: Tree Testing
    description: Evaluate the taxonomy of information on a website.
    plays: ["UnderstandProcess"]
    stage: ["Ideate"]
    outcomes: ["TransformProcess","DeliverSelfService"]
    order: 200  
    layout: page
    related: ["Card Sorting"]
---
## Method Overview
One of the core capabilities of ServiceNow is to provide self-service to employees or customers to resolve issues, and request assets or services. Your portal users need to efficiently find the right information or catalog items to complete their self-service goals. To ensure easy navigation, tree-testing provides evidence of a user’s ability to complete tasks. Tree testing can be done with a moderator, observing, and asking questions or un-moderated with participants completing the test on their own time

## Outcomes
* Confidence in the currently defined information architecture of content items in an application
* Areas to improve the site’s navigability

## Prerequisites
* Defined information architecture for a site
* List of 3-5 common tasks users come to the site to perform.

## Participants
Test participants should represent potential users of the site and have limited “inside knowledge” of the service providers. That means not including help desk staff or ServiceNow team members.

## Materials Needed
* An online tree testing tool such as TreeJack, MUIQ, or UserZoom
* Teleconferencing tool if conducting a moderated test

## Process
When conducting a tree test we recommend that you conduct a few moderated sessions (3-5) to get qualitative feedback and confirm the test is well structured. IN addition, you should run 20+ users through unmoderated testing to get a large enough sample of data to make decisions.

### Moderated Tree Test
1.	Setup your tree testing tool with the site’s information architecture and common tasks.
2.	Run 1-2 pilot sessions with colleagues to make sure everything is set up correctly.
3.	Recruit and invite 5 participants to participate in moderated testing
4.	In each session, remind the participant that “This is a test of the system, not of you. There are no wrong answers. Your feedback is greatly appreciated.”
5.	Ask open ended questions about their behavior such as “Why did you choose that option?” or “What are you looking for right now?”
6.	Once all sessions are completed, use the testing tool’s Analysis capability to identify the outcomes of each task. You want to note:
7.	Which tasks were completed successfully? Most efficiently?
8.	Where was there bouncing (a participant went down one navigation path and had to go back and try again)?
9.	To build more confidence in your information architecture, you can invite more participants to take the test on their own time

### Unmoderated Tree Test
1.	Follow steps 1-2 above to prepare your test
2.	Send an email to a large group of participants inviting them to participate in the study. We suggest inviting 3x more people than you hope to get responses from
3.	Give them a reasonable amount of time to complete the study. We recommend no more than 2 weeks.
4.	Once all sessions are completed, use the testing tool’s Analysis capability to identify the outcomes of each task. You want to note:
5.	Which tasks were completed successfully? Most efficiently?
6.	Where was there bouncing (a participant went down one navigation path and had to go back and try again)?

## Synthesis 
Use the outcomes of your study to identify navigation areas of improvement. From the moderated sessions use the qualitative feedback as input into any changes you might recommend.

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
[Tree Testing 101 (Optimal Workshop)](https://www.optimalworkshop.com/learn/101s/tree-testing/?utm_source=google&utm_medium=cpc&utm_campaign=us-alpha-tree-testing&keyword=tree%20testing&matchtype=b&network=g&gclid=CjwKCAjwh4ObBhAzEiwAHzZYU0FdRcqsjYa27Jx4UhSviUmR83rPLSYuVsSPbCMOyQhXLa7YSsYyjRoCOrUQAvD_BwE)

[Tree Testing: Fast, Iterative Evaluation of Menu Labels and Categories (NN Group)](https://www.nngroup.com/articles/tree-testing/)
