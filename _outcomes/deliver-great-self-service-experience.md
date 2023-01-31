---
title: Deliver a Great Self-Service Experience
subtitle: Focus on your requestors expectations to deliver intuitive employee and customer journeys.
share-description: When creating a self-service destination to help customers and employees resolve issues and get back to value, it is critical to create clear paths to resolution. That means understanding how your users expect to explore content, provide information and get back to good. By following these methods and best practices, you will meet your users' needs with a delightful experience.
layout: page
permalink: /outcomes/deliver-great-self-service-experience
tags: ["Employee Center","Customer Service Management"]
related: ["Usability Testing", "Card Sorting","Tree Testing"]
---
{% assign outcome_methods = site.methods | where: "outcomes", "DeliverSelfService" | sort: "order" %}

Self Service on ServiceNow seems so simple, right? You assign a catalog or two, a knowledge base, upload a logo, do some light theming in the Branding Editor, and share the link with the world... 

From there, you reasonably expect to see volume to call center going down, the onsite technicians focused on the back log of tickets (not the people popping by their desks), and folks quickly getting back to work when problems arise. Unfortunately, it doesn't always work out that way. Employees or customers complain they can't find content, their requests go unfulfilled, and it’s made getting service worse. This is not a failure in the technology platform itself, but in the curation of content and workflows. It stems from a lack of understanding the users the site is built for; their knowledge level, the words they use, and the expectations they come with.

The importance of this grows as customers use the platform to deliver content through capabilities like Employee Center to supplant or augment their existing Intranet.

## What can we do differently?
If we take a step back from a focus on just the technical implementation and apply common human-centered design techniques, we can efficiently deliver an experience that meets the users needs. By creating a governance model that continues to apply these techniques as content evolves and user needs change, we can sustain that great experience over time.

## Understand
The journey begins by first understanding your users through interviews, surveys, and data analysis. By understanding their relationship with the current state of their service experience, you can define their mental model for interacting with a future self-service experience.

### Methods and Plays
<div class="method-group">
{% assign understand_methods = outcome_methods | where: "stage", "Understand" %}
{% for method in understand_methods %}
    {% include method.html  method=method %}
{% endfor %}
</div>

## Ideate
Once you've developed an understanding of your users needs, expectations, and challenges, it is time to explore how to best organize and present content and collect information from users. 

**Reference our [Service Portal Best Practices](/best-practices/service-portal.md) article to ground yourself in recommended approaches to your implementation.**

### Methods and Plays
<div class="method-group">
{% assign ideate_methods = outcome_methods | where: "stage", "Ideate" %}
{% for method in ideate_methods %}
    {% include method.html  method=method %}
{% endfor %}
</div>

## Create
Armed with a strong understanding of your users’ expectations, language and points of friction you can start tackling the various decisions that go into delivering your self-service experience

They include:

**When a user is trying to find a piece of content…**
-	How do you name catalog items, knowledge articles and other content?
-	How is that content organized on the site? What do you name the categories or topic areas?

**When a user opens an item that has a form to fill out…**
-	How many questions do you ask them?
-	What questions do you ask them? Do they the information to answer those questions?
-	What field types do you use to capture information?

**If using virtual agent…**
-	What can a user type to get to the information they need?
-	What questions are you asking them within the conversation?
-	Are they getting enough feedback to move forward?

### Methods and Plays
<div class="method-group">
{% assign create_methods = outcome_methods | where: "stage", "Create" %}
{% for method in create_methods %}
    {% include method.html  method=method %}
{% endfor %}
</div>